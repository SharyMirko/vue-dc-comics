<template>
  <div id="app">
    <HeaderDC />
    <Content />
  </div>
</template>

<script>
import HeaderDC from './components/HeaderDC.vue'
import Content from './components/Content.vue'

export default {
  name: 'App',
  components: {
    HeaderDC,
    Content
  }
}
</script>

<style slang="scss">
@import './assets/styles/style.scss';
</style>
