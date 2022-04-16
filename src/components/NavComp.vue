<template>
  <div>
   <ul>
     <li v-for="(element, index) in navBar " :key="index" :class="[element.active ? 'active' : 'notActive']" ><a :href="element.url">{{element.name}}</a></li>
   </ul>
  </div>
</template>

<script>
export default {
  name: 'NavComp',
  data(){
    return{
      navBar:[
        {
        name:'CHARACTERS',
        url:'/characters'
        },
        {
        name:'COMICS',
        url:'/comics',
        active: true
        },
        {
        name:'MOVIES',
        url:'/movies'
        },
        {
        name:'TV',
        url:'/tv'
        },
        {
        name:'GAMES',
        url:'/games'
        },
        {
        name:'COLLECTIBLES',
        url:'/collectibles'
        },
        {
        name:'VIDEOS',
        url:'/videos'
        },
        {
        name:'FANS',
        url:'/fans'
        },
        {
        name:'NEWS',
        url:'/news'
        },
        {
        name:'SHOP',
        url:'/shop'
        },
      ]
    }
  },

}
</script>


<style scoped lang="scss">
li{
  list-style-type:none;
  padding: 0 10px;
  display: flex;
  align-items: center;
  a{
    text-decoration: none;
    color: rgb(70, 70, 70);
    font-weight: bold;
    font-size: 0.8rem;

  }
}
ul{
  display: flex;
  padding: 0;
  margin: 0;
  height: 100%;

}
div{
  height: 100%; 
}
.active{
  border-bottom: 5px solid rgb(77, 148, 255);
  a{
    color: rgb(77, 148, 255);
  }
}

</style>
