<template>
  <div class="content">
      <div class="container">
          <div class="nav">
          <ul>
              <li><h3>{{ navName1 }}</h3></li>
              <li v-for="(item, i) in comics" :key="i"><a :href="item.link">{{ item.text }}</a></li>
               <ul>
              <li><h3>{{ navName4 }}</h3></li>
              <li v-for="(ob, m) in shop" :key="m"><a :href="ob.link">{{ ob.text }}</a></li>
          </ul>
          </ul>
          <ul>
              <li><h3>{{ navName2 }}</h3></li>
              <li v-for="(obj, n) in dc" :key="n"><a :href="obj.link">{{ obj.text }}</a></li>
          </ul>
          <ul>
              <li><h3>{{ navName3 }}</h3></li>
              <li v-for="(obj, n) in sites" :key="n"><a :href="obj.link">{{ obj.text }}</a></li>
          </ul>
          </div>
          <div class="logo"><img src="../assets/img/dc-logo-bg.png" alt=""></div>
      </div>
  </div>
</template>

<script>
/* eslint-disable */
export default {
name: 'FooterNav',
data (){
    return {
        navName1: 'dc comics',
        navName2: 'dc',
        navName3: 'sites',
        navName4: 'shop',
        comics: [
            {
                link: '#',
                text: 'Characters'
            },
            {
                link: '#',
                text: 'Comics'
            },
            {
                link: '#',
                text: 'Movies'
            },
            {
                link: '#',
                text: 'TV'
            },
            {
                link: '#',
                text: 'Games'
            },
            {
                link: '#',
                text: 'Videos'
            },
            {
                link: '#',
                text: 'News'
            },
        ],
        dc: [
            {
                link: '#',
                text: 'Terms of Use'
            },
            {
                link: '#',
                text: 'Privacy Policy (New)'
            },
            {
                link: '#',
                text: 'Ad Choices'
            },
            {
                link: '#',
                text: 'Advertising'
            },
            {
                link: '#',
                text: 'Jobs'
            },
            {
                link: '#',
                text: 'Subscriptions'
            },
            {
                link: '#',
                text: 'CPSC Certificates'
            },
            {
                link: '#',
                text: 'Ratings'
            },
            {
                link: '#',
                text: 'Shop Help'
            },
            {
                link: '#',
                text: 'Contact Us'
            },
            
        ],
        sites: [
            {
                link: '#',
                text: 'DC'
            },
            {
                link: '#',
                text: 'DC UNIVERSE INFINITE'
            },
            {
                link: '#',
                text: 'DC Kids'
            },
            {
                link: '#',
                text: 'DC Shop'
            },
            {
                link: '#',
                text: 'MAD Magazine'
            },
        ],
        shop: [
            {
                link: '#',
                text: 'Shop DC'
            },
            {
                link: '#',
                text: 'Shop DC Collectibles'
            },
        ]
    }
}
}
</script>

<style scoped lang="scss">
.logo {
    img {
        position: relative;
right: -100px;
top: -96px;
width: 85%;
    }
}
.nav {
    display: flex;
}
.container {
    display: flex;
    justify-content: space-between;
}

h3 {
    padding: 1rem 0;
    color: #fff;
    text-transform: uppercase;
}

li {
    display: block;
    margin: 0 .5rem;
    a {
        color: gray;
        font-size: 8px;
        text-decoration: none;
    }
}
.content {
    background-image: url('../assets/img/footer-bg.jpg');
    background-size:contain;
    height:19rem;
    padding: 1rem 0;
    overflow: hidden;
}
</style>