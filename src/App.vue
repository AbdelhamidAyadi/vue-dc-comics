<template>
  <div class="container">
    <header>
      <div class="logoContainer">
        <LogoComp/>
      </div>
      <div class="navBarContainer">
        <NavComp/>
      </div>
    </header>
    <main>
      <ContentComp/>
    </main>


  </div>
</template>

<script>
import LogoComp from './components/LogoComp.vue'
import NavComp from './components/NavComp.vue'
import ContentComp from './components/ContentComp.vue'



export default {
  name: 'App',
  components: {
    LogoComp,
    NavComp,
    ContentComp,
  }
}
</script>

<style lang="scss">
*{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

header{
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 10%;
  
  height: 70px;
  .logoContainer,
  .navBarContainer
  {
    height: 100%;
   
  }
  
}
//Main part 
main{
  background-color: black;
  padding: 0 10%;
}
</style>
