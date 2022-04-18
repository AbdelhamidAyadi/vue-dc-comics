<template>
  <div class="container">

    <div>
      <h3>
        SIGN-UP NOW!
      </h3>
    </div>
    <div class="container2">
      <h4>
        FOLLOW US
      </h4>
      <img src=".././assets/img/footer-facebook.png" alt="logo facebook">
      <img src=".././assets/img/footer-twitter.png" alt="logo facebook">
      <img src=".././assets/img/footer-youtube.png" alt="logo facebook">
      <img src=".././assets/img/footer-pinterest.png" alt="logo facebook">
      <img src=".././assets/img/footer-periscope.png" alt="logo facebook">
    </div>

  </div>
</template>

<script>
export default {
  name: 'SocialComp',

}
</script>


<style scoped lang="scss">
.container{
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px 10%;
  background-color: #303030;

  h3{
    border: #0282f9 2px solid;
    color: white;
    padding: 10px;
  }
}
.container2{
  display: flex;
  align-items: center;

  img{
    padding: 0 5px;
  }
  h4{
    padding: 0 10px;
    color: #0282f9;
  }
}
</style>
