<template>
  <main-container>
    <template v-slot:header>
      <TheHeader />
    </template>
    <main>
      <router-view />
    </main>
    <template v-slot:footer>
      <TheFooter />
    </template>

  </main-container>
</template>

<script>
import TheHeader from '@/components/TheHeader.vue'
import TheFooter from '@/components/TheFooter.vue'
import MainContainer from '@/components/MainContainer.vue';

export default {
  components: {
    MainContainer,
    TheHeader,
    TheFooter,
  },
}
</script>