<template>
  <div class="wrap d-flex flex-column min-vh-100">
    <Header />
    <main class="flex-fill">
      <router-view />
    </main>
    <TheFooter />
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import TheFooter from '@/components/TheFooter.vue'

export default {
  components: {
    Header,
    TheFooter,
  },
}
</script>