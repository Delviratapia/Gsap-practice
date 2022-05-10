<template>


    <!-- CROSS FLOWERS -->



    <div class="flex justify-center mt-36">

        <div class="parent bg-white sm:w-full  relative">


            <div class="flex flex-col items-center justify-evenly mt-36">

                <img id="greenMixT" class="h-24 w-24 sm:h-52 sm:w-52 mb-12" src="public/images/Grupo 3616-green@2x.png"
                    alt="cross petal top">

                <div class="flex flex-col gap-7">
                    <img id="blueTC" class="w-14  sm:w-24" src="public/images/Grupo 3613-u@2x.png"
                        alt="blue top center">
                    <img id="blueBC" class="w-14  sm:w-24" src="public/images/Grupo 3613-d@2x.png"
                        alt="blue bottom center">
                </div>

                <img id="greenMixB" class="h-24 w-24 sm:h-52 sm:w-52 mt-12" src="public/images/Grupo 3616-green@2x.png"
                    alt="cross petal bottom">

            </div>


            <div class="flex flex-row items-center justify-evenly  ">

                <img id="greenMixL" class="h-24 w-24 sm:h-52 sm:w-52 " src="public/images/Grupo 3616-green@2x.png"
                    alt="cross petal top">

                <div class="flex flex-row gap-7">
                    <img id="blueLC" class="h-14 sm:h-24" src="public/images/Grupo 3613-l@2x.png"
                        alt="blue left center">
                    <img id="blueRC" class="h-14  sm:h-24" src="public/images/Grupo 3613-r@2x.png"
                        alt="blue right center">
                </div>

                <img id="greenMixR" class="h-24 w-24 sm:h-52 sm:w-52" src="public/images/Grupo 3616-green@2x.png"
                    alt="cross petal bottom">

            </div>



        </div>

    </div>


</template>

<script setup>

import gsap from "gsap";
import { onMounted } from "vue";

onMounted(() => {


    // Cross flower animation

// const timeline = gsap.timeline({ defaults: { duration: 2, ease: "power1.out", yoyo: true, repeat: -1 } });


    gsap.to("#greenMixB",
        {
            duration: 2,
            transformOrigin: "30% 70%",
            rotation: '45',
            x: 10,
            scale: '0.5',
            yoyo: true,
            repeat: -1,
            ease: 'power1.out',
        });

    gsap.to("#greenMixT",
        {
            duration: 2,
            transformOrigin: "60% 10%",
            rotation: '45',
            x: 10,
            scale: '0.5',
            yoyo: true,
            repeat: -1,
            ease: 'power1.out',
        });


    gsap.to("#greenMixL",
        {
            duration: 2,
            transformOrigin: "60% 50%",
            rotation: '45',
            x: 10,
            scale: '0.5',
            yoyo: true,
            repeat: -1,
            ease: 'power1.out',
        });

    gsap.to("#greenMixR",
        {
            duration: 2,
            transformOrigin: "30% 35%",
            rotation: '45',
            x: 10,
            scale: '0.5',
            yoyo: true,
            repeat: -1,
            ease: 'power1.out',
        });


    gsap.to("#blueLC",
        {
            duration: 2,
            transformOrigin: "50% 60%",
            x: -50,
            scale: '2',
            yoyo: true,
            repeat: -1,
            ease: 'power1.out',
        });


    gsap.to("#blueRC",
        {
            duration: 2,
            transformOrigin: "50% 60%",
            x: 50,
            scale: '2',
            yoyo: true,
            repeat: -1,
            ease: 'power1.out',
        });

    gsap.to("#blueTC",
        {
            duration: 2,
            transformOrigin: "50% 60%",
            y: -50,
            scale: '2',
            yoyo: true,
            repeat: -1,
            ease: 'power1.out',
        });

    gsap.to("#blueBC",
        {
            duration: 2,
            transformOrigin: "50% 60%",
            y: 50,
            scale: '2',
            yoyo: true,
            repeat: -1,
            ease: 'power1.out',
        });

})

</script>





<style scoped>
@media only screen and (max-width: 800px) {


    #greenMixL {
        position: relative;
        bottom: 15rem;

    }

    #greenMixR {
        position: relative;
        bottom: 15rem;

    }

    #blueLC {
        position: relative;
        bottom: 14.8rem;
    }

    #blueRC {
        position: relative;
        bottom: 14.8rem;
    }

}

@media only screen and (min-width: 700px) {


    #greenMixL {
        position: relative;
        bottom: 26rem;

    }

    #greenMixR {
        position: relative;
        bottom: 26rem;

    }

    #blueLC {
        position: relative;
        bottom: 26.5rem;
    }

    #blueRC {
        position: relative;
        bottom: 26.5rem;
    }

}


.crossRow {
    bottom: 216px;
}
</style>