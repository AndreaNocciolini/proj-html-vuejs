<template>
  <div class="my-container">
      <div class="title d-flex align-items-center justify-content-around">
          <h5>TESTIMONIALS</h5>
      </div>
      <div class="description d-flex flex-row-reverse text-end mb-3">
          <h3>WHAT'S THE COSTUMERS SAY ABOUT OUR WORK</h3>
      </div>
      <div class="comments-section d-flex flex-row-reverse">
          <div class="comments-container row row-cols-4">
              <div class="comments col p-5" v-for="(element, index) in commentsArray" :key="index">
                  <p>{{element.text}}</p>
                  <h4>{{element.author}}</h4>
                  <h5>{{element.company}}</h5>

              </div>
          </div>
      </div>

  </div>
</template>

<script>
export default {
    name: 'Testimonials',
    props: [
        'commentsArray',
    ]
}
</script>

<style lang="scss" scoped>
    .my-container {
        width: 100%;
        height: 100vh;
        background-color: var(--bg-dark-3);
        .title,
        .description {
            width: 100%;
            color: var(--tx-white-1);
            h3 {
                width: 30%;
            }
        }
        .comments-section {
            width: 100%;
            .comments-container {
                width: 90%;
                background-color: var(--bg-white-1);
            }
        }
    }
</style>