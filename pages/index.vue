<template>
<div class="construction-wrapper">
    <div class="container">
        <div class="row">
            <div class="col">
                <div class="constructions d-flex justify-content-center align-items-center flex-column">
                    <h1 class="constructions__title title title--style">
                        Page Is Under <strong>construction</strong> 
                    </h1>
                    <p class="constructions__text">We are working on something big. <br>We will be back soon. </p>
                    <Countdown class="mt-4" deadline="November 19, 2018"></Countdown>
                </div>
            </div>
        </div>
    </div>
</div>
</template>

<script>
import Countdown from 'vuejs-countdown'
export default {
    components: { 
        Countdown 
    }
}
</script>


<style lang="scss" scoped>

.construction-wrapper {
    background: linear-gradient(290deg, rgba(255,204,33,1) 0%, rgba(255,204,33,1) 30%, rgba(74,196,246,1) 80%, rgba(74,196,246,1) 100%);
    background-size: cover;
    background-attachment: scroll;
}

.constructions {
    min-height: 70vh;
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
    color: rgba(0, 0, 0, 0.78);
}
</style>
