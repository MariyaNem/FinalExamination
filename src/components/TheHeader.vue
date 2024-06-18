<template>
  <nav class="navbar navbar-expand-lg navbar-light ">
    <div class="container">
      <a class="navbar-brand logo" href="/"><img src="../assets/images/icons/dentlogo.png" alt="logo"></a>

      <div class="collapse collapse-fontsize navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">

          <li class="nav-item menu-link" v-for="(menu, index) in headerMenuList" :key="index">
            <router-link class="nav-link active" aria-current="page" :to="menu.path">
              {{ menu.name }}
            </router-link>
          </li>
        </ul>
        <div class="headerIcons">
          <a href="https://vk.com/" target="_blank"><img src="../assets/images/icons/vk-logo.png" alt="" /></a>
          <a href="https://www.youtube.com/" target="_blank"><img src="../assets/images/icons/youtube.png" alt="" /></a>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data() {
    return {
      headerMenuList: [
        { name: 'о нас', path: '/о нас' },
        { name: 'услуги', path: '/услуги' },
        { name: 'акции', path: '/акции' },
        { name: 'врачи', path: '/врачи' },
        { name: 'записаться', path: '/записаться' },
      ]
    }
  }
}
</script>

<style lang="scss">
@import '../assets/layouts/index.scss';

.navbar {
  height: 90px;

}

.navbar-nav {
  height: 90px;
}

.logo {
  padding-right: 150px;
}

.collapse-fontsize {
  font-size: 20px;
}

.menu-link {
  padding: 25px 20px;

  &:hover {
    background: $menuColor;
  }
}

.headerIcons {
  a {
    margin-right: 20px;
  }
}
</style>