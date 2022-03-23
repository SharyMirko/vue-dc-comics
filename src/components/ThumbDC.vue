<template>
  <div class="thumbler">
    <img :src="thumb" :alt="series">
    <span>{{ series }}</span>
  </div>
</template>

<script>
/* eslint-disable */
export default {
  name: 'ThumbDC',
  props: {
    thumb: String,
    price: String,
    series: String,
    type: String
  }
}
</script>

<style lang="scss" scoped>
.thumbler {
  display: inline-block;
  width: 150px;
  img {
    width: 150px;
    height: 150px;
  }
  color: white;
  span {
    display: block;
  }
  margin: .5rem ;
  text-align: left;
}
</style>>
