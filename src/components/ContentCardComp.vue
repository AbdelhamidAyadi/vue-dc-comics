<template>
     <div class="card">
       <img :src="thumb" :alt="series">
       <p>
         {{ series }}
       </p>
     </div>
</template>

<script>
export default {
  name: 'ContentCardComp',
  props:{
    thumb: String,
    series: String
  }
  
  
}
</script>


<style scoped lang="scss">
.card{
  width: calc( 100% / 6 );
  padding: 20px  10px;
  img{
    width: 100%;
  }
  p{
    color: white;
    text-transform: uppercase;
    padding: 5px 0;
    font-weight: bold;
  }
}

</style>
