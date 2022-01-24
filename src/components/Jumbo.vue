<template>
    <div class="my-container d-flex">
        <div class="description-container d-flex flex-column justify-content-center align-items-start ms-5">
            <p> Always the best way you need it</p>
            <h1>THE BEST BUSINESS CONSULTING</h1>
            <div><button>READ MORE</button><i class="fas fa-play"></i></div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Jumbo'
}
</script>

<style lang="scss" scoped>
    .my-container {
        height: 100vh;
        width: 100%;
        background-image: url('../assets/images/portrait-of-young-architect-woman-on-meeting-KFZCE3A.jpg');
        background-size: contain;
        background-repeat: no-repeat;
        background-position: right;
        background-color: #22213d;
        .description-container {
            width: 30%;
        }
    }
    .fas.fa-play{
        color: white;
        font-size: 0.5em;
        border: 1px solid white;
        padding: 1.5em;
        border-radius: 50%;
    }
</style>