<template>
  <div class="my-container d-flex align-items-center justify-content-space-around p-5 mt-5 mb-5">
    <div class="consultants-container">
      <h4 class="consultants-title">OUR CONSULTANTS CAN HELP YOU <span></span></h4>
      <div class="row row-cols-2">
        <div v-for="(element, index) in consultantsArray" :key="index" class="col d-flex align-items-start justify-content-around p-4">
          <div class="icon-container h-100 me-3">
            <i :class="element.icon"></i>
          </div>
          <div class="description-container">
            <h5 class="w-100">{{element.title}}</h5>
            <p class="w-50">{{element.description}}</p>
          </div> 
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'Consultants',
    props: [
      'consultantsArray',
    ]
}
</script>

<style lang="scss" scoped>
  .my-container {
    width: 100%;
    .consultants-container{
      height: 10%;
      margin: 0 auto;
      width: 80%;
      height: 80%;
      .consultants-title span {
        display: inline-block;
        width: 60%;
        height: 2px;
        background-color: var(--bg-green-1);
        border-radius: 1px;
      }
      .row {
        height: 90%;
        .icon-container {
          font-size: 1.5em;
          i {
            padding: 0.4em;
            border: 1px solid var(--tx-white-1);
            border-radius: 50%;
            color: var(--bg-white-1);
            background-color: var(--bg-red-1);
          }
        }
      }
      .description-container {
        h5 {
          font-weight: 900;
        }
        p {
          font-size: 0.8em;
          color: var(--tx-grey-2);
        }
      }
    }
  }
</style>