<template>
  <div class="content">
      <div class="container">
          <ul>
              <li class="obj-fit" v-for="(obj, i) in nav" :key="i"><img :src="obj.img" :class="{lol: obj.shop}" :alt="obj.text"><a :href="obj.link">{{ obj.text }}</a></li>
          </ul>
      </div>
  </div>
</template>

<script>
/* eslint-disable */
import dcComics from '../assets/img/buy-comics-digital-comics.png'
import sub from '../assets/img/buy-comics-subscriptions.png'
import merc from '../assets/img/buy-comics-merchandise.png'
import shop from '../assets/img/buy-comics-shop-locator.png'
import visa from '../assets/img/buy-dc-power-visa.svg'

export default {
name: 'FooterHead',
data () {
    return {
        nav: [
            {
                link: '#',
                img: dcComics,
                text: 'digital comics'
            },
            {
                link: '#',
                img: merc,
                text: 'dc mercahandise'
            },
            {
                link: '#',
                img: sub,
                text: 'subscription'
            },
            {
                link: '#',
                img: shop,
                text: 'comic shop locator',
                shop: true
            },
            {
                link: '#',
                img: visa,
                text: 'dc power visa'
            },
        ]
    }
}
}
</script>

<style scoped lang="scss">
@import '../assets/styles/partials/_variables.scss';

.lol {
    height: calc(3rem + 15px);
}

ul {
    display: flex;
    justify-content: center;   
    padding: 1rem 0; 
}

li {
    display: flex;
    align-items: center;
    margin: 0 1rem;
    img {
        width: 3rem;
        height: 3rem;
    }
    a {
        display: inline-block;
        text-decoration: none;
        text-transform: uppercase;
        color: #fff;
        font-weight: bold;
        font-size: .6rem;
        margin: 0 0 0 .4rem;
    }
}
.content {
    height: 6rem;
    background-color: $nav-color;
}
</style>