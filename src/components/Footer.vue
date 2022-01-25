<template>
  <footer>
      <div class="links-container">
          <div class="logo">
              <img src="../assets/images/logotype-2-139x23.png" alt="">
          </div>
      </div>  
  </footer>
</template>

<script>
export default {
    name: "Footer",
}
</script>

<style lang="scss" scoped>
    footer{
        width: 100%;
        background-color: var(--bg-dark-3);
        .links-container {
            width: 88%;
            margin: 0 auto;
        }
    }
</style>