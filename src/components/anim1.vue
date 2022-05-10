<template>

    <!-- FOUR CORNER FLOWER -->


    <div class="flex justify-center mt-16">

        <div class="parent bg-white relative">

            <!-- TOP CORNER FLOWERS -->

            <div class="relative top-left-petals">

                <img id="pinkPT" class="toplPink1 object-cover h-3 w-auto absolute" src="public/images/path-pink-t.png"
                    alt="petal top">
                <img id="pinkPB" class="toplPink2 object-cover h-3 w-auto relative left-10 top-0"
                    src="public/images/path-pink-b.png" alt="petal bottom ">

                <img id="yellowPL" class="toplYellow1 object-cover h-3 w-auto absolute "
                    src="public/images/path-yellow-l.png" alt="petal left">
                <img id="yellowPR" class="toplYellow2 object-cover h-3 w-auto absolute "
                    src="public/images/path-yellow-r.png" alt="petal right">
            </div>

            <div class=" relative top-right-petals">

                <img id="pinkPT" class="toprPink1 object-cover h-3 w-auto absolute" src="public/images/path-pink-t.png"
                    alt="petal top">
                <img id="pinkPB" class="toprPink2 object-cover h-3 w-auto absolute" src="public/images/path-pink-b.png"
                    alt="petal bottom">

                <img id="yellowPL" class="toprYellow1 object-cover h-3  w-auto absolute"
                    src="public/images/path-yellow-l.png" alt="petal left">
                <img id="yellowPR" class="toprYellow2 object-cover h-3  w-auto absolute"
                    src="public/images/path-yellow-r.png" alt="petal right">
            </div>



            <!--  CENTER FLOWERS -->


            <div class="container  flex flex-col justify-between">

                <div class="flex justify-between">

                    <div class=" w-screen flex flex-col">

                        <!-- top div -->

                        <div class=" flex flex-row justify-center items-center">

                            <div id="greenPL" class="relative top-16 left-2 ">
                                <img class="object-cover h-20 w-auto" src="public/images/path-green-bl@2x.png"
                                    alt="petal top">
                            </div>

                            <div id="greenPR" class="relative right-4 ">
                                <img class="object-cover h-20 w-auto" src="public/images/path-green-tr@2x.png"
                                    alt="petal bottom">
                            </div>


                        </div>


                        <!-- bottom div -->

                        <div class="flex flex-row justify-center items-center">

                            <div class="relative  bottom-20">
                                <img id="bluePL" class="object-cover h-20  w-auto"
                                    src="public/images/path-blue-tl@2x.png" alt="petal bottom">
                            </div>
                            <div class="relative  bottom-4 right-3">
                                <img id="bluePR" class="object-cover h-20  w-auto"
                                    src="public/images/path-blue-br@2x.png" alt="petal bottom">

                            </div>
                        </div>


                        <!-- green small petals -->


                        <div class="absolute justify-center self-center ">

                            <div class="greenLeft flex">
                                <img id="greenSPL" class=" object-cover h-10  w-auto relative top-9 right-6"
                                    src="public/images/path-green-tl.png" alt="petal top">
                            </div>

                            <div class="greenRight  flex">
                                <img id="greenSPR" class=" object-cover h-10  w-auto left-3 top-7 relative"
                                    src="public/images/path-green-br.png" alt="petal bottom">
                            </div>

                        </div>

                        <!-- blue small petals -->

                        <div class="absolute justify-center self-center ">

                            <div class="blueRight flex">
                                <img id="blueSPL" class="object-cover h-10  w-auto top-9 left-3 relative"
                                    src="public/images/path-blue-tr.png" alt="petal top">
                            </div>

                            <div id="blueSPR" class="blueLeft flex">
                                <img class="object-cover h-10  w-auto relative top-7 right-5"
                                    src="public/images/path-blue-bl.png" alt="petal bottom">
                            </div>


                        </div>

                        <!-- BOTTOM CORNER FLOWERS -->


                        <div class="flex flex-row ">

                            <div class="relative bottom-left-petals">

                                <!-- <div class=" flex flex-col justify-center items-center"> -->
                                <img id="pinkPT" class="btlPink1 object-cover h-3  w-auto absolute"
                                    src="public/images/path-pink-t.png" alt="petal top">
                                <img id="pinkPB" class="btlPink2 object-cover h-3  w-auto absolute"
                                    src="public/images/path-pink-b.png" alt="petal bottom">
                                <!-- </div> -->

                                <!-- <div class="flex flex-row w-24 absolute  bottom-2 left-1 "> -->
                                <img id="yellowPL" class="btlYellow1 object-cover h-3  w-auto absolute"
                                    src="public/images/path-yellow-l.png" alt="petal left">
                                <img id="yellowPR" class="btlYellow2 object-cover h-3  w-auto absolute"
                                    src="public/images/path-yellow-r.png" alt="petal right">
                                <!-- </div> -->

                            </div>


                            <div class="relative bottom-right-petals">

                                <!-- <div class="flex flex-col justify-center items-center gap-1"> -->
                                <img id="pinkPT" class="btrPink1 object-cover h-3  w-auto absolute"
                                    src="public/images/path-pink-t.png" alt="petal top">
                                <img id="pinkPB" class="btrPink2 object-cover h-3  w-auto absolute"
                                    src="public/images/path-pink-b.png" alt="petal bottom">
                                <!-- </div> -->

                                <!-- <div class="flex flex-row w-24 absolute bottom-2  ml-auto mr-auto left-1"> -->
                                <img id="yellowPL" class="btrYellow1 object-cover h-3  w-auto absolute"
                                    src="public/images/path-yellow-l.png" alt="petal left">
                                <img id="yellowPR" class="btrYellow2 object-cover h-3  w-auto absolute"
                                    src="public/images/path-yellow-r.png" alt="petal right">
                                <!-- </div> -->
                            </div>
                        </div>



                    </div>


                </div>

            </div>
        </div>
    </div>




</template>


<script setup>

import gsap from "gsap";
import { onMounted } from "vue";

onMounted(() => {


    gsap.to("#yellowPL",
        {
            duration: 2,
            x: -5,
            yoyo: true,
            repeat: -1,
            ease: 'power1.out',


        });

    gsap.to("#yellowPR",
        {
            duration: 2,
            x: 5,
            yoyo: true,
            repeat: -1,
            ease: 'power1.out',


        });

    gsap.to("#pinkPT",
        {
            duration: 2,
            y: -5,
            yoyo: true,
            repeat: -1,
            ease: 'power1.out',


        });

    gsap.to("#pinkPB",
        {
            duration: 2,
            y: 5,
            yoyo: true,
            repeat: -1,
            ease: 'power1.out',



        });

    // Big exterior petals


    gsap.to("#bluePL",
        {
            duration: 2,
            transformOrigin: "85% 100%",
            y: -25,
            rotation: '43',
            scale: '1.1',
            yoyo: true,
            repeat: -1,
            ease: 'power1.out',
        });


    gsap.to("#bluePR",
        {
            duration: 2,
            transformOrigin: "0% 15%",
            y: 25,
            rotation: '43',
            scale: '1.1',
            yoyo: true,
            repeat: -1,
            ease: 'power1.out',
        });




    gsap.to("#greenPR",
        {
            duration: 2,
            transformOrigin: "5% 90%",
            x: 25,
            rotation: '45',
            scale: '1.1',
            yoyo: true,
            repeat: -1,
            ease: 'power1.out',
        });


    gsap.to("#greenPL",
        {
            duration: 2,
            transformOrigin: "90% 5%",
            x: -25,
            rotation: '45',
            scale: '1.1',
            yoyo: true,
            repeat: -1,
            ease: 'power1.out',
        });

    // small inside petals


    gsap.to("#greenSPL",
        {
            duration: 2,
            transformOrigin: "85% 95%",
            y: -20,
            rotation: '43',
            scale: '1.1',
            yoyo: true,
            repeat: -1,
            ease: 'power1.out',
        });


    gsap.to("#greenSPR",
        {
            duration: 2,
            transformOrigin: "0% 15%",
            y: 20,
            rotation: '43',
            scale: '1.1',
            yoyo: true,
            repeat: -1,
            ease: 'power1.out',
        });


    gsap.to("#blueSPL",
        {
            duration: 2,
            transformOrigin: "5% 90%",
            x: 10,
            rotation: '45',
            scale: '1.1',
            yoyo: true,
            repeat: -1,
            ease: 'power1.out',
        });


    gsap.to("#blueSPR",
        {
            duration: 2,
            transformOrigin: "30% 5%",
            x: 10,
            rotation: '45',
            scale: '1.1',
            yoyo: true,
            repeat: -1,
            ease: 'power1.out',
        });

});

</script>



<style scoped>
@media only screen and (min-width: 950px) {

    .top-left-petals {
        width: 100%;
        left: 38rem;
    }

    .top-right-petals {
        width: 100%;
        right: 44rem;
        top: 1.2rem;
    }

    .bottom-left-petals {
        width: 100%;
        left: 43rem;
        bottom: 1.2rem;
    }

    .bottom-right-petals {
        width: 100%;
        left: 4rem;
        bottom: 1.2rem;
    }
}

@media only screen and (max-width: 900px) {

    .top-left-petals {
        width: 100%;
        left: 15rem;
    }

    .top-right-petals {
        width: 100%;
        right: 21.5rem;
        top: 1.2rem;
    }

    .bottom-left-petals {
        width: 100%;
        left: 20rem;
        bottom: 1.2rem;
    }

    .bottom-right-petals {
        width: 100%;
        left: 2rem;
        bottom: 1.2rem;
    }
}






@media only screen and (max-width: 700px) {

    .top-left-petals {
        width: 100%;
        left: 15rem;
    }

    .top-right-petals {
        width: 100%;
        right: 21.5rem;
        top: 1.3rem;
    }

    .bottom-left-petals {
        width: 100%;
        left: 8.5rem;
        bottom: 1rem;
    }

    .bottom-right-petals {
        width: 100%;
        left: 3rem;
        bottom: 1rem;

    }
}



/* bottom  petals */

.btrYellow1 {
    left: 35px;
    top: 10px;
}

/* .btrYellow1 {
        right: 51px;
        top: 10px;
    } */

.btrYellow2 {
    left: 45px;
    top: 10px;

}

.btrPink1 {
    bottom: -17px;
    left: 40px;
}

.btrPink2 {
    left: 40px;
    top: 15px;
}

.btlYellow1 {
    left: -40px;
    top: 10px;
}

.btlYellow2 {
    left: -30px;
    top: 10px;
}

.btlPink1 {
    left: -35px;
    top: 5px;
}

.btlPink2 {
    left: -35px;
    top: 15px;
}






/* top  petals */

.toprYellow1 {
    bottom: 25px;
    right: -40px;
}

.toprYellow2 {
    bottom: 25px;
    right: -50px;

}


.toplYellow1 {
    left: 35px;
    bottom: 5px;

}

.toplYellow2 {
    left: 45px;
    bottom: 5px;

}

.toprPink1 {
    right: -45px;
    bottom: 30px;

}

.toprPink2 {
    right: -45px;
    bottom: 20px;
}

.toplPink1 {
    left: 40px;
    bottom: 10px;
}

.toplPink2 {
    left: 40px;
}


</style>