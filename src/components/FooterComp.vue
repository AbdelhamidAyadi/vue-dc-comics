<template>
  <div>
    
      <div class="container1">
        <div class="container2">
          <div class="container3">
            <h3>DC COMICS</h3>
            <ul>
              <li v-for="(element,index) in dcComics" :key="index"><a :href="element.url">{{element.name}}</a></li>
            </ul>
            <h3>SHOP</h3>
            <ul>
              <li v-for="(element,index) in shop" :key="index"><a :href="element.url">{{element.name}}</a></li>
            </ul>
          </div>
          <div class="container3">
            <h3>DC</h3>
            <ul>
              <li v-for="(element,index) in dc" :key="index"><a :href="element.url">{{element.name}}</a></li>
            </ul>
          </div>
          <div class="container3">
            <h3>SITES</h3>
            <ul>
              <li v-for="(element,index) in sites" :key="index"><a :href="element.url">{{element.name}}</a></li>
            </ul>
          </div>
        </div>
        <div class="logo_background">

        </div>
      </div>

  </div>
</template>

<script>
  export default {
    name: 'FooterComp',
    data() {
      return {
        dcComics: [{
            name: 'Characters',
            url: '/characters'
          },
          {
            name: 'Comics',
            url: '/comics'
          },
          {
            name: 'Movies',
            url: '/movies'
          },
          {
            name: 'TV',
            url: '/tv'
          },
          {
            name: 'Games',
            url: '/games'
          },
          {
            name: 'Videos',
            url: '/videos'
          },
          {
            name: 'News',
            url: '/news'
          },
        ],
        shop: [{
            name: 'Shop DC',
            url: '/shop_dc'
          },
          {
            name: 'Shop DC Collectibles',
            url: '/shop_dc_collectibles'
          },
        ],
        dc: [{
            name: 'Terms Of Use',
            url: '/terms_of_use'
          },
          {
            name: 'Privacy Policy (New)',
            url: '/privacy_policy'
          },
          {
            name: 'Ad Choises',
            url: '/ad_choises'
          },
          {
            name: 'Advertising',
            url: '/advertising'
          },
          {
            name: 'Jobs',
            url: '/privacy_policy'
          },
          {
            name: 'Subscriptions',
            url: '/subscriptions'
          },
          {
            name: 'Talent Workshops',
            url: '/talent_workshops'
          },
          {
            name: 'CPSC Certificates',
            url: '/cpsc_certificates'
          },
          {
            name: 'Ratings',
            url: '/ratings'
          },
          {
            name: 'Shop Help',
            url: '/shop_help'
          },
          {
            name: 'Contact Us',
            url: '/contact_us'
          },
        ],
        sites: [{
            name: 'DC',
            url: '/dc'
          },
          {
            name: 'MAD Magazine',
            url: '/mad_magazine'
          },
          {
            name: 'DC Kids',
            url: '/dc_kids'
          },
          {
            name: 'DC Universe',
            url: '/dc_universe'
          },
          {
            name: 'DC Power Visa',
            url: '/dc_power_visa'
          },
        ],

      }
    }

  }
</script>


<style scoped lang="scss">
  .container1 {
    display: flex;
    background-image: url('.././assets/img/footer-bg.jpg');
    
  }

  .container2 {
    display: flex;
    
    padding: 50px 10%;
    

    ul {
      list-style-type: none;
    }

    h3 {
      color: white;
      padding: 15px 0;
    }

    a {
      text-decoration: none;
      color: rgb(189, 189, 189);

      &:hover{
        color:#0282f9;
      }
    }
  }

  .container3 {
    margin-left: 50px;
  }

  .logo_background {
    flex-grow: 1;
    background-image: url('.././assets/img/dc-logo-bg.png');
    background-repeat: no-repeat;
  }
</style>