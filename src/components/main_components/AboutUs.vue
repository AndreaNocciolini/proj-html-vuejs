<template>
  <div class="about-us-container position-relative d-flex">
    <div class="about-us-img-container position-relative">
        <img src="../../assets/images/business-people-working-together-on-project-and-5FHSKBL.jpg" alt="">
    </div>
    <div class="about-us-description d-flex justify-content-center flex-column w-50 p-4">
        <h5><span class="me-3"></span>ABOUT US</h5>
        <h2>WE MAKE YOUR STRATEGY WORK</h2>
        <p>When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a...When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a</p>
    </div>
    <div class="get-started-container position-absolute d-flex justify-content-around">
        <div class="get-started-title p-3">
            <h3>WE HELP TO DELIVER THE BUSINESS CASE</h3>
        </div>
        <div class="get-started-description p-3">
            <p>When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a</p>
        </div>
        <div class="get-started-button position-absolute">
            <button class="p-2">Get Started</button>
        </div>
    </div>
  </div>
</template>
 <!--//RESTART FROM HERE*************************************************POLISH AND IMPROVE LAYOUT!!!!!-->
<script>
export default {
    name: 'AboutUs',
}
</script>

<style lang="scss" scoped>
.about-us-container {
    width: 100%;
    .about-us-img-container {
        img {
            width: 100%;
        }
    }
    .about-us-description {
        background-color: var(--bg-dark-3);
        width: 30%;
        color: var(--tx-white-1);
        h5{
            width: 65%;
            font-size: 1em;
            span {
            display: inline-block;
            width: 10%;
            height: 2px;
            background-color: var(--bg-green-1);
            }
        }
        h2{
            width: 85%;
            font-size: 3.5em;
            font-weight: 900;
        }
        p {
            width: 65%;
            color: var(--tx-grey-2);
            font-size: 0.9em;
        }
    }
    .get-started-container {
        background-color: var(--bg-green-1);
        width: 90%;
        bottom: 0;
        padding: 2em;
        transform: translate(0, 50%);
        .get-started-title {
            width: 30%;
            font-weight: 700;
        }
        .get-started-description {
            width: 30%;
            color: var(--tx-grey-2);
        }
        .get-started-button {
            bottom: 0;
            right: 0;
            button {
                color: var(--tx-white-1);
                background-color: var(--bg-red-1);
                padding: 1em 3em;
                border: 0;
                font-size: 0.7em;
            }
        }
    }
}
</style>