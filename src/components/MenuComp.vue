<template>
  <div>
    
    <ul>
      <li v-for="(element ,index) in menu" :key=" index " ><img :src="`/img/${element.img}`" :alt="element.name"><a :href="element.url">{{element.name}}</a></li>
    </ul>
  
  </div>
</template>

<script>
export default {
  name: 'MenuComp',
  data(){
    return{
      menu:[
        {
        name:'DIGITAL COMICS',
        url:'/digital_comics',
        img:'buy-comics-digital-comics.png'
        },
        {
        name:'DC MERCHANDISE',
        url:'/dc_merchandise',
        img:'buy-comics-merchandise.png'
        },
        {
        name:'SUBSCRIPTION',
        url:'/subscription',
        img:'buy-comics-subscriptions.png'

        },
        {
        name:'COMIC SHOP LOCATOR',
        url:'/comic_shop_locator',
        img:'buy-comics-shop-locator.png'
        },
        {
        name:'DC POWER VISA',
        url:'/dc_power_visa',
        img:'buy-comics-shop-locator.png'
        },
        
      ]
    }
  },

  
  
}
</script>


<style scoped lang="scss">
div{
  padding: 50px 10%;
  background-color: #0282f9;

  ul{
    list-style: none;
    display: flex;
    justify-content: space-between;


    li{
      display: flex;
      align-items: center;

      img{
        height: 80px;
      }
      a{
        text-decoration: none;
        color:white ;
        padding-left: 10px;
        font-weight:lighter;
        font-size: 0.8rem;
        &:hover{
          color:black;
        }
      }
    }
  }
}
</style>
