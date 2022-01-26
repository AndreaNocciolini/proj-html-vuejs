<template>
  <div class="my-container position-relative">
      <div class="img-container">
          <img src="../../assets/images/business-people-working-together-on-project-and-B3MZ4TX.jpg" alt="">
      </div>
      <div class="description-container position-absolute top-50 start-50 translate-middle position-absolute">
          <h2>LET'S TALK ABOUT WORK</h2>
          <p>A wonderful serenity has taken possession Far far away, behind the word mountains</p>
          <button>GET STARTED</button>
      </div>
  </div>
</template>

<script>
export default {
    name:'LetsTalk'
}
</script>

<style lang="scss" scoped>
    .my-container {
        width: 100%;
        .img-container {
            img {
                width: 100%;
            }
        }
        .description-container {
            color: var(--tx-white-1);
            width: 30%;
            text-align: center;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: space-around;
            button {
                color: var(--tx-white-1);
                background-color: var(--bg-dark-3);
                padding: 1em 3em;
                border: none;
            }
        }
    }
</style>