<template>
  <div class="my-container pt-4 pb-2 d-flex justify-content-between align-items-end">
    <div class="terms-of-use">
      <h6>Terms of use</h6>
      <h6>Privacy enviromental policy</h6>
    </div>
    <div class="copyright">
      <h6>Copyright &copy; 2020 Plhox consulting. All rights reserved.</h6>
    </div>
  </div>
</template>

<script>
export default {
    name: 'BottomFooter'
}
</script>

<style lang="scss" scoped>
  .my-container {
    width: 88%;
    margin: 0 auto;
    background-color: var(--bg-dark-3);
    color: var(--tx-grey-6);
    h6 {
      font-size: 0.8em;
    }
  }

</style>