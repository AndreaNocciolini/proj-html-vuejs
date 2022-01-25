<template>
  <div class="my-container p-4">
      <div class="divider">
      </div>
      <div class="project-container">
          <div class="title">
              <h5>PROJECT</h5>
          </div>
          <div class="description d-flex align-items-center justify-content-between">
              <h2>OUR EXPERTS TRUSTED CONSULTANTS HELP CLIENTS</h2>
              <div class="button-container d-flex justify-content-evenly">
                  <button><i class="fas fa-arrow-left"></i></button>
                  <button><i class="fas fa-arrow-right"></i></button>
              </div>   
          </div>
          <div class="slider row row-cols-3">
              <div class="col">
                  <img src="../../assets/images/DRY-1-790x592.jpg" alt="">
              </div>
              <div class="col">
                  <img src="../../assets/images/221bf0b7-8134-43bb-936a-5acbe42db64a-790x592.jpg" alt="">
              </div>
              <div class="col">
                  <img src="../../assets/images/z1el4c4p-790x592.jpg" alt="">
              </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'Projects',
    // PROPS DA USARE PER FARE CICLO FOR SU IMMAGINI************************************
    props: [
        'projectsImgArray',
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
        .project-container {
            width: 88%;
            margin: 0 auto;
            .description {
                h2 {
                    width: 60%;
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
                }
            }
        }
    }
</style>