<template>
  <div class="container">
    <header>
      <div class="logoContainer">
        <LogoComp />
      </div>
      <div class="navBarContainer">
        <NavComp />
      </div>
    </header>
    <main>
      <ContentComp />
      <MenuComp />
    </main>
    <footer>
      <FooterComp />
      <SocialComp />
    </footer>


  </div>
</template>

<script>
  import LogoComp from './components/LogoComp.vue'
  import NavComp from './components/NavComp.vue'
  import ContentComp from './components/ContentComp.vue'
  import MenuComp from './components/MenuComp.vue'
  import FooterComp from './components/FooterComp.vue'
  import SocialComp from './components/SocialComp.vue'



  export default {
    name: 'App',
    components: {
      LogoComp,
      NavComp,
      ContentComp,
      MenuComp,
      FooterComp,
      SocialComp
    },
    
  }
</script>

<style lang="scss">
  * {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  }

  header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 0 10%;

    height: 70px;

    .logoContainer,
    .navBarContainer {
      height: 100%;

    }

  }

  //Main part 
</style>