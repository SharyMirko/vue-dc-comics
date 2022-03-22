<template>
  <div class="content">
      <div class="container">
          <p>--> Content goes here </p>
      </div>
  </div>
</template>

<script>
/* eslint-disable */
export default {
name: 'Content'
}
</script>

<style scoped lang="scss">
@import '../assets/styles/partials/_variables.scss';
.content {
    height: 8rem;
    background-color: $content-bg;
    p {
        font-size: 2rem;
        color: #fff;
        padding-top: 1rem;
    }
}
</style>