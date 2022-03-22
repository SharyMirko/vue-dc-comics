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
                text: 'mercahandise'
            },
            {
                link: '#',
                img: 'link',
                text: 'ddsfd'
            },
            {
                link: '#',
                img: 'link',
                text: 'ddsfd'
            },
            {
                link: '#',
                img: 'link',
                text: 'ddsfd'
            },
        ]
    }
}
}
</script>

<style scoped lang="scss">
@import '../assets/styles/partials/_variables.scss';
.content {
    height: 6rem;
    background-color: $nav-color;
}
</style>