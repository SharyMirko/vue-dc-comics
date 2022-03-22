<template>
<header>
    <div class="container">
        <div class="nav">
        <img src="@/assets/img/dc-logo.png" alt="DC Logo">
        <ul>
            <li @click="navIndex = index" v-for="(link, index) in nav" :key="index" :class="{active: navIndex == index}"><a :href="link.link">{{ link.text }}</a></li>
        </ul>
        </div>
    </div>
</header>
</template>

<script>
/* eslint-disable */
export default {
name: 'HeaderDC',
data () {
    return {
     navIndex: 1,
     nav: [
   {
       link: '#',
       text: 'characters'
   },
   {
       link: '#',
       text: 'comics'
   },
   {
       link: '#',
       text: 'movies'
   },
   {
       link: '#',
       text: 'tv'
   },
   {
       link: '#',
       text: 'games'
   },
   {
       link: '#',
       text: 'collectibles'
   },
   {
       link: '#',
       text: 'videos'
   },
   {
       link: '#',
       text: 'fans'
   },
   {
       link: '#',
       text: 'news'
   },
   {
       link: '#',
       text: 'shop'
   },
         ]
     }
 }
}
</script>

<style scoped lang="scss">
@import '../assets/styles/partials/variables';

ul {
    height: 100%;
    line-height: 3;
}

li {
    display: inline-block;
    padding: 1rem 0;
    margin: 0 1rem;
    height: 100%;
    a {
        display: inline-block;
        text-decoration: none;
        text-transform: uppercase;
        color: $nav-color;
        font-weight: bold;
        font-size: .6rem;
    }
    &.active {
        border-bottom: .3rem solid $nav-color;
    }
}

.nav {
    height: 5rem;
    display: flex;
    justify-content: space-between;
    align-items: center;
    img {
        width: 4rem;
    }
}

</style>