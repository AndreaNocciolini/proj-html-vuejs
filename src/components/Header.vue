<template>
  <header class="fixed-top">
      <div class="header-container d-flex justify-content-around align-items-center">
          <div class="header-logo">
              <img src="../assets/images/logotype.png" alt="">
          </div>
          <div class="header-menu d-flex align-items-center">
              <ul class="list-unstyled d-flex w-100 align-items-end justify-content-around">
                  <li class="first-link"><a href="">Home</a></li>
                  <li><a href="">About</a></li>
                  <li><a href="">Projects</a></li>
                  <li><a href="">Services</a></li>
                  <li><a href="">Blog</a></li>
                  <li><a href="">Contact</a></li>
              </ul>
          </div>
      </div>
  </header>
</template>

<script>
export default {
    name: "Header",
}
</script>

<style lang="scss" scoped>
    .header-container {
        -webkit-text-stroke: 0.15px black;
        height: 50px;
        width: 100%;
        background-color: var(--bg-white-2);
        .header-logo img{
            width: 30%;
        }
        .header-menu {
            width: 30%;
            ul {
            margin: auto;
            li a {
                color: var(--tx-white-1);
                text-decoration: none;
                }
            li:hover::before,    
            .first-link::before {
                content: '';
                width: 100%;
                height: 2px;
                background-color: var(--bg-white-1);
                display: block;
                margin-bottom: 1.5em;
                }
            
            }
        }
    }
</style>