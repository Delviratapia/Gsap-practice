<template>
    <div class="header relative text-center bg-gradient-to-r from-primary">

        <!--Content before waves-->
        <div class="in-header flex justify-center items-center text-center w-full m-0 p-0">

            <!--Logo-->

            <img src="public/images/acs-logo.png" alt="">
            <h1 class="app-text text-3xl text-gray-900">Appetite Creative <strong
                    class="text-primary">Soul</strong>utions</h1>

        </div>

        <!-- Container-->
        <div>
            <svg class="waves relative w-full -mb-2" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 24 150 28"
                preserveAspectRatio="none" shape-rendering="auto">
                <defs>
                    <path id="gentle-wave"
                        d="M-160 44c30 0 58-18 88-18s 58 18 88 18 58-18 88-18 58 18 88 18 v44h-352z" />
                </defs>
                <g class="parallax">
                    <use xlink:href="#gentle-wave" x="48" y="0" fill="rgba(255,255,255,0.7" />
                    <use xlink:href="#gentle-wave" x="48" y="3" fill="rgba(255,255,255,0.5)" />
                    <use xlink:href="#gentle-wave" x="48" y="5" fill="rgba(255,255,255,0.3)" />
                    <use xlink:href="#gentle-wave" x="48" y="7" fill="#fff" />
                </g>
            </svg>
        </div>
        <!--end-->

    </div>




    <!-- Content -->
    <div class="content flex justify-center items-center text-center text-lg mb-24">
        <p>Phaser animation</p>
        <a href="https://github.com/Delviratapia/phaserDogTest" target="_blank" class="phaserBtn">Repository</a>


    </div>



</template>






<script>
import { onMounted } from "vue";

onMounted(() => {

    let text = document.querySelector('.app-text');

    window.addEventListener('scroll', () => {
        let value = window.scrollY;

        text.style.top = value * 1 + 'px';

    })



});



</script>





<style scoped>
@import url(//fonts.googleapis.com/css?family=Lato:300:400);

body {
    margin: 0;
}

.app-text {
    font-family: 'Lato', sans-serif;
    font-weight: 300;
    letter-spacing: 2px;
    z-index: 1;
}

p {
    font-family: 'Lato', sans-serif;
    letter-spacing: 1px;
    color: #333333;
}


.phaserBtn {
    box-shadow: inset 0px 39px 0px -24px #e67a73;
    background-color: #e4685d;
    border-radius: 28px;
    border: 6px solid #ffffff;
    display: inline-block;
    cursor: pointer;
    color: #ffffff;
    font-family: Arial;
    font-size: 23px;
    padding: 15px 25px;
    text-decoration: none;
    text-shadow: 0px 1px 0px #b23e35;
}

.phaserBtn:hover {
    background-color: #eb675e;
}

.phaserBtn:active {
    position: relative;
    top: 1px;
}





.in-header {
    height: 65vh;
}

.waves {
    height: 15vh;
}

/* .content {
    position: relative;
    height: 20vh;
    text-align: center;
    background-color: white;
} */

/* Animation */

.parallax>use {
    animation: move-forever 25s cubic-bezier(.55, .5, .45, .5) infinite;
}

.parallax>use:nth-child(1) {
    animation-delay: -2s;
    animation-duration: 7s;
}

.parallax>use:nth-child(2) {
    animation-delay: -3s;
    animation-duration: 10s;
}

.parallax>use:nth-child(3) {
    animation-delay: -4s;
    animation-duration: 13s;
}

.parallax>use:nth-child(4) {
    animation-delay: -5s;
    animation-duration: 20s;
}

@keyframes move-forever {
    0% {
        transform: translate3d(-90px, 0, 0);
    }

    100% {
        transform: translate3d(85px, 0, 0);
    }
}

@media (max-width: 768px) {
    .waves {
        height: 40px;
        min-height: 40px;
    }

    .content {
        height: 30vh;
    }

    h1 {
        font-size: 24px;
    }
}
</style>