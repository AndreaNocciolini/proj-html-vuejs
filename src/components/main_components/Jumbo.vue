<template>
    <div class="jumbo-container d-flex position-relative">
        <div class="jumbo-bg position-relative">
        </div>
        <div class="description-container ms-5">
                <h6><span></span>ALWAYS THE BEST WAY U NEED IT</h6>
                <h1>THE BEST BUSINESS CONSULTING</h1>
                <div><button id="button-hover" class="me-5">READ MORE</button><i class="fas fa-play"></i></div>
            </div>
        <div class="jumbo-img">
            <img src="../../assets/images/portrait-of-young-architect-woman-on-meeting-KFZCE3A.jpg" alt="">
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
        .jumbo-bg {
            width: 35%;
        }
        .jumbo-img {
            width: 70%;
            img {
                max-width: 100%;
            }
        }
    }
    .fas.fa-play{
        color: var(--tx-green);
        font-size: 0.5em;
        border: 1px solid var(--tx-white-1);
        padding: 1.5em;
        border-radius: 50%;
    }
    .description-container {
                width: 40%;
                position: absolute;
                top: 30%;
                right: 50%;
                h6::before{
                    content:'';
                    display: inline-block;
                    width: 5%;
                    height: 2px;
                    background-color: var(--bg-green-1);
                    border-radius: 1px;
                    border-radius: 1px;
                    margin-right: 1em;
                }
                h1 {
                    font-size: 5em;
                    font-weight: 900;
                }
                button {
                    background-color: var(--bg-green-1);
                    border: none;
                    font-size: 0.7em;
                    padding: 1.5em 5em;
                }
            }
</style>