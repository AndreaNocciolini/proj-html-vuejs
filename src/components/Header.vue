<template>
  <header>
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
        height: 50px;
        width: 100%;
        background-color: rgb(148, 0, 0, 0.8);
        .header-logo img{
            width: 30%;
        }
        .header-menu {
            width: 30%;
            ul {
            margin: auto;
            li a {
                color: white;
                text-decoration: none;
                }
            li:hover::before,    
            .first-link::before {
                content: '';
                width: 100%;
                height: 2px;
                background-color: white;
                display: block;
                margin-bottom: 1.5em;
                }
            
            }
        }
    }
</style>