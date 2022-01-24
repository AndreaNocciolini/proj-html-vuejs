<template>
  <div class="about-us-container position-relative d-flex">
    <div class="about-us-img-container position-relative">
        <img src="../../assets/images/business-people-working-together-on-project-and-5FHSKBL-1390.jpg" alt="">
        <div class="red-filter position-absolute w-100 h-100"></div>
    </div>
    <div class="about-us-description d-flex justify-content-center flex-column w-50 p-4">
        <h5>ABOUT US</h5>
        <h2>WE MAKE YOUR STRATEGY WORK</h2>
        <p>When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a...When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a</p>
    </div>
    <div class="get-started-container position-absolute d-flex justify-content-around">
        <div class="get-started-title w-25">
            <h3>WE HELP TO DELIVER THE BUSINESS CASE</h3>
        </div>
        <div class="get-started-description w-25">
            <p>When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a</p>
        </div>
        <div class="get-started-button position-absolute">
            <button class="p-2">Get Started</button>
        </div>
    </div>
  </div>
</template>

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
        .red-filter {
            background-color: var(--bg-red-2);
            top: 0;
            left: 0;
            opacity: 0.7;
        }
    }
    .about-us-description {
        background-color: var(--bg-dark-3);
        width: 30%;
        h5,
        h2,
        p {
            color: var(--tx-white-1);
            width: 65%;
        }
    }
    .get-started-container {
        background-color: var(--bg-green-1);
        width: 90%;
        bottom: 0;
        padding: 2em;
        transform: translate(0, 50%);
        .get-started-button {
            bottom: 0;
            right: 0;
            button {
                color: var(--tx-white-1);
                background-color: var(--bg-red-1);
                border: 0;
                font-size: small;
            }
        }
    }
}
</style>