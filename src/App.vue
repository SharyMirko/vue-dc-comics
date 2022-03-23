<template>
  <div id="app">
    <HeaderDC />
    <Content />
    <FooterDC />
  </div>
</template>

<script>
/* eslint-disable */
import HeaderDC from './components/HeaderDC.vue'
import Content from './components/Content.vue'
import FooterDC from './components/FooterDC.vue'

export default {
  name: 'App',
  components: {
    HeaderDC,
    Content,
    FooterDC
  }
}
</script>

<style slang="scss">
@import './assets/styles/style.scss';
</style>
