<template>
<div class="construction-wrapper">
    <div class="container">
        <div class="row no-gutters">
            <div class="col">
                <div class="constructions d-flex justify-content-center align-items-center flex-column">
                    <img src="/hps-white.svg" alt="" style="max-width: 370px">
                    <p class="constructions__text">We are working on something big. <br>We will be back soon. </p>
                    <countdown class="mt-4" deadline="December 19, 2018"></countdown>
                </div>
            </div>
        </div>
    </div>
</div>
</template>

<script>
import countdown from 'vuejs-countdown'
export default {
    components: { 
        countdown 
    }
}
</script>


<style lang="scss">

.construction-wrapper {
    background: linear-gradient(290deg, rgb(117, 15, 109) 0%, rgb(153, 18, 142) 30%, rgba(74,196,246,1) 80%, rgba(74,196,246,1) 100%);

    background-size: cover;
    background-attachment: fixed;
}

.constructions {
    min-height: 100vh;
    overflow: hidden;
    &__title {
        text-align: center; 
        font-size: 3.6rem;
        @media (max-width: 350px) {
            font-size: 3.2rem;
        }
        @media (max-width: 320px) {
            font-size: 2.2rem;
        }
    }
    &__text {
        text-transform: uppercase;
        text-align: center;
        margin-top: 2.5rem;
        line-height: 1.5;
        font-size: 1.6rem;
        font-weight: 700;
        color: rgba(0, 0, 0, 0.85);
        @media (max-width: 320px) {
            font-size: 1.4rem;
        }
    }
}

.digit, .text {
    color: #fff;
}
</style>
