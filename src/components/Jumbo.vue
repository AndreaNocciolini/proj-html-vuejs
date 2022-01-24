<template>
    <div class="jumbo-container d-flex position-relative">
        <!-- <div class="description-container d-flex flex-column justify-content-center align-items-start ms-5">
            <p> Always the best way you need it</p>
            <h1>THE BEST BUSINESS CONSULTING</h1>
            <div><button>READ MORE</button><i class="fas fa-play"></i></div>
        </div> -->
        <div class="jumbo-description float-start positione-relative">
            <div class="description-container ms-5">
            <p> Always the best way you need it</p>
            <h1>THE BEST BUSINESS CONSULTING</h1>
            <div><button class="me-3">READ MORE</button><i class="fas fa-play"></i></div>
        </div>
        </div>
        <div class="jumbo-img float-end">
            <img src="../assets/images/portrait-of-young-architect-woman-on-meeting-KFZCE3A.jpg" alt="">
        </div>
    </div>
</template>

<script>
export default {
    name: 'Jumbo'
}
</script>

<style lang="scss" scoped>
    .jumbo-container {
        width: 100%;
        color: var(--tx-white-1);
        background-color: var(--bg-dark-3);
        .jumbo-description {
            width: 35%;
            .description-container {
                width: 20%;
                position: absolute;
                top: 50%;
                right: 60%;
                font-size: larger;
            }
        }
        .jumbo-img {
            width: 70%;
            img {
                max-width: 100%;
            }
        }
        // background-image: url('../assets/images/portrait-of-young-architect-woman-on-meeting-KFZCE3A.jpg');
        // background-size: contain;
        // background-repeat: no-repeat;
        // background-position: right;
        
        // .description-container {
        //     width: 30%;
        // }
    }
    .fas.fa-play{
        color: var(--tx-white-1);
        font-size: 0.5em;
        border: 1px solid var(--tx-white-1);
        padding: 1.5em;
        border-radius: 50%;
    }
</style>