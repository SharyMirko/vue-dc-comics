<template>
<div class="content">
      <div class="container">
          <div class="button">SING-UP NOW!</div>
          <div class="social">
              <span>follow us</span>
              <img src="../assets/img/footer-facebook.png" alt="facebook">
              <img src="../assets/img/footer-periscope.png" alt="periscope">
              <img src="../assets/img/footer-pinterest.png" alt="pintarest">
              <img src="../assets/img/footer-twitter.png" alt="twitter">
              <img src="../assets/img/footer-youtube.png" alt="youtube">
          </div>
      </div>
  </div>
</template>

<script>
/* eslint-disable */

export default {
name: 'FooterSocial'
}
</script>

<style scoped lang="scss">

.social {
    display: flex;
    align-items: center;
    span {
        text-transform: uppercase;
font-weight: bold;
color: white;
margin-right: 1rem;
    }
    img {
        margin: 0 .3rem;
        &:hover {
            filter: invert(37%) sepia(51%) saturate(4075%) hue-rotate(194deg) brightness(99%) contrast(110%);
        }
    }
}

.container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 100%;
}
.content {
    background-color: #303030;
    height: 7.65rem;
}
.button {
    padding: .5rem;
    border: 2px solid #0282F9;
    color: #fff;
}

</style>