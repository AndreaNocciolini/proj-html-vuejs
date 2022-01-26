<template>
  <div class="my-container">
      <div class="blog-container">
        <div class="title">
          <h5><span class="me-3"></span>BLOG</h5>
        </div>
        <div class="description d-flex justify-content-between">
            <div class="text">
                <h2>THE RECENT NEWS YOU MUST READ IT</h2>
            </div>
            <div class="button d-flex">
                <button>VIEW ALL</button>
            </div>
        </div>
        <div class="articles row row-cols-2">
            <div v-for="(element, index) in articlesArray" :key="index" class="col p-3 position-relative">
                <img src="../../assets/images/startup-business-people-and-strategy-board-PAJ3P9K-1390x1042.jpg" alt="">
                <div class="content-articles position-absolute">
                    <h4>{{element.date}}, by {{element.author}}</h4>
                    <h2>{{element.title}}</h2>
                    <p>{{element.content}}</p>
                </div>
            </div>
        </div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'Blog',
    props: [
        'articlesArray',
    ]

}
</script>

<style lang="scss" scoped>
    .my-container {
        width: 100%;
        padding-bottom: 20em;
        color: var(--tx-white-1);
        background-color: var(--bg-dark-3);
        .blog-container {
            width: 90%;
            margin: 0 auto;
            .title{
                h5 {
                    font-size: 1em;
                    span {
                        display: inline-block;
                        width: 3%;
                        height: 2px;
                        background-color: var(--bg-green-1);  
                    }
                }
            }
            .description {
                .text {
                    h2{   
                        font-weight: 900;
                        font-size: 2.5em;
                    }
                }
                button {
                    padding: 1em 3em;
                    font-size: 0.8em;
                    background-color: var(--bg-green-1);
                    border: 0;
                }
            }
            .articles {
                .col {
                    img {
                        width: 100%;
                    }
                    .content-articles {
                        top: 80%;
                        left: 40%;
                        background-color: var(--bg-white-1);
                        color: var(--tx-dark-4);
                        padding: 2em;
                    }
                } 
            }
        }
    }
</style>