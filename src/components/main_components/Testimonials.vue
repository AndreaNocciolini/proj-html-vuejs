<template>
  <div class="my-container">
      <div class="title d-flex align-items-center justify-content-around">
          <h5>TESTIMONIALS<span></span></h5>
      </div>
      <div class="description d-flex flex-row-reverse text-end mb-3">
          <h3>WHAT'S THE COSTUMERS SAY ABOUT OUR WORK</h3>
      </div>
      <div class="comments-section d-flex flex-row-reverse">
          <div class="comments-container row row-cols-4 position-relative">
              <div class="comments col p-5 me-2" v-for="(element, index) in commentsArray" :key="index" :class="element.bg_img">
                  <p>{{element.text}}</p>
                  <h4>{{element.author}}</h4>
                  <h6>{{element.company}}</h6>

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
        .title{
            color: var(--tx-white-1);
            font-size: 1em;
            h5{
                width: 100%;
                text-align: center;
                position: relative;
            }
            span {
                display: inline-block;
                width: 3%;
                height: 2px;
                background-color: var(--bg-green-1);
                position: absolute;
                right: 6%;
                top: 90%;
            }
        }
        .description {
            width: 94%;
            color: var(--tx-white-1);
            h3 {
                width: 50%;
                font-size: 2.5em;
                font-weight: 900;
            }
        }
        .comments-section {
            width: 100%;
            .comments-container {
                width: 90%;
                background-color: var(--bg-white-1);
                .comments {
                    transition: all .3s linear;
                    p{
                        color: var(--tx-grey-1);
                        font-size: 0.9em;
                    }
                    h5 {
                        color: var(--tx-dark-3);
                    }
                    h6 {
                        color: var(--tx-grey-1);
                        font-size: 0.7em;
                    }
                }
                .comment-0:hover{
                    background-image: url(../../assets/images/oliver-ragfelt-488196-2.jpg);
                }
                .comment-1:hover{
                    background-image: url(../../assets/images/12679.jpg);
                }
                .comment-2:hover{
                    background-image: url(../../assets/images/oliver-ragfelt-488196-unsplash.jpg);
                }
                .comment-0:hover,
                .comment-1:hover,
                .comment-2:hover{
                    cursor: pointer;
                    background-size: contain;
                    box-shadow: 5px -5px 0px 0px black inset, 5px 5px 0px 0px black inset;
                    h4 {
                        color: var(--tx-white-1);
                    }
                }
            }
        }
    }
</style>