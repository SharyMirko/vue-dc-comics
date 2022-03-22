<template>
  <div class="content">
      <div class="container">
          <ul>
              <li v-for="(obj, i) in nav" :key="i"><img :src="obj.img" :alt="obj.text"><a :href="obj.link">{{ obj.text }}</a></li>
          </ul>
      </div>
  </div>
</template>

<script>
/* eslint-disable */
export default {
name: 'FooterHead',
data () {
    return {
        nav: [
            {
                link: '#',
                img: '../assets/img/buy-comics-digital-comics.png',
                text: 'digital comics'
            },
            {
                link: '#',
                img: '../assets/img/buy-comics-merchandise.png',
                text: 'dc mercahandise'
            },
            {
                link: '#',
                img: '../assets/img/buy-comics-subscriptions.png',
                text: 'subscription'
            },
            {
                link: '#',
                img: '../assets/img/buy-comics-shop-locator.png',
                text: 'comic shop locator'
            },
            {
                link: '#',
                img: '../assets/img/buy-dc-power-visa.svg',
                text: 'dc power visa'
            },
        ]
    }
}
}
</script>

<style scoped lang="scss">
@import '../assets/styles/partials/_variables.scss';

li {
    display: inline-block;
}
.content {
    height: 6rem;
    background-color: $nav-color;
}
</style>