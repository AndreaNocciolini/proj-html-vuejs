<template>
  <div class="my-container">
      <div class="divider">
      </div>
      <div class="project-container">
          <div class="title">
              <h5><span class="me-3"></span>PROJECT</h5>
          </div>
          <div class="description d-flex align-items-center justify-content-between">
              <h2>OUR EXPERTS TRUSTED CONSULTANTS HELP CLIENTS</h2>
              <div class="button-container d-flex justify-content-evenly">
                  <button><i class="fas fa-arrow-left"></i></button>
                  <button><i class="fas fa-arrow-right"></i></button>
              </div>   
          </div>
          <div class="slider row row-cols-3">
              <div class="col position-relative" v-for="(element, index) in projectsArray" :key="index">
                  <img :src="element.src" alt="">
                  <div class="img-hover position-absolute">
                      <div class="product-container">
                        <h3>{{element.company}}</h3>
                        <h6>{{element.product_category}}</h6>
                      </div>
                      <div class="button-container">
                          <button id="button-hover">+</button>
                      </div>
                  </div>
              </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'Projects',
    props: [
        'projectsArray',
    ]
}
</script>

<style lang="scss" scoped>
    .divider{
        height: 15em;
    }
    .my-container {
        background-color: var(--bg-dark-3);
        color: white;
        padding-bottom: 10em;
        .project-container {
            width: 88%;
            margin: 0 auto;
            .title{
                font-size: 1em;
                span{
                    display: inline-block;
                    width: 3%;
                    height: 2px;
                    background-color: var(--bg-green-1);    
                }
            }
            .description {
                h2 {
                    width: 60%;
                    font-size: 2.2em;
                    font-weight: 900;
                }
                .button-container {
                    width: 5%;
                    button {
                    color: var(--tx-white-1);
                    background-color: var(--bg-dark-1);
                    font-size: 0.6em;
                    padding: 0.8em;
                    border: none;
                    }
                }
            }
            .slider {
                .col {
                    img {
                        width: 100%;
                    }
                    .img-hover {
                        display: none;
                        width: 93%;
                        height: 100%;
                        top: 0;
                        right: 3.5%;
                        background-color: var(--bg-red-1);
                        opacity: 0.85;
                        box-shadow: 0px 0px 0px 5px #000000;
                        button {
                            border: none;
                            font-size: 2em;
                            padding: 0.2em 0.7em;
                            color: var(--tx-white-1);
                            background-color: var(--bg-dark-1);
                        }
                    }
                    &:hover .img-hover{
                        display: flex;
                        align-items: flex-end;
                        justify-content: space-between;
                        padding: 1em;
                    }
                }
            }
        }
    }
</style>