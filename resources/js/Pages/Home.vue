<template>
    <Nav />
        <div class="relative slide">
            <div
                class="carousel-indicators absolute bottom-0 flex h-24 w-full justify-center items-center"
            >
                <ol class="z-50 flex w-4/12 justify-center">
                    <li
                        v-for="(img, i) in images"
                        :key="i"
                        class="md:w-4 md:h-4 bg-gray-300 rounded-full cursor-pointer mx-2"
                    ></li>
                </ol>
            </div>
            <div class="carousel-inner relative overflow-hidden w-full">
                <div
                    v-for="(img, i) in images"
                    :id="`slide-${i}`"
                    :key="i"
                    :class="`${active === i ? 'active' : 'left-full'}`"
                    class="carousel-item inset-0 relative w-full h-[38rem] transform transition-all duration-500 ease-in-out"
                >
                    <button class="absolute bottom-[8rem] left-[12rem] flex rounded-[3.31px] bg-white px-6 py-2">Shop Now</button>
                    <img class="block w-full h-[38rem]" src="../../../public/images/1.png"  alt="First slide" />
                </div>
            </div>
        </div>
</template>
<script>
import Nav from "../Shared/Nav";

export default {
    components: {
        Nav,
    },
    data: () => ({
        images: [
            "https://picsum.photos/id/237/1024/800",
            "https://picsum.photos/id/238/1024/800",
            "https://picsum.photos/id/239/1024/800",
            "https://picsum.photos/id/240/1024/800",
        ],
        active: 0,
    }),
    mounted() {
        let i = 0;
        setInterval(() => {
            if (i > this.images.length - 1) {
                i = 0;
            }
            this.active = i;
            i++;
        }, 3000);
    },
};
</script>
<style scoped>
.left-full {
    left: -100%;
}

.carousel-item {
    float: left;
    position: relative;
    display: block;
    width: 100%;
    margin-right: -100%;
    backface-visibility: hidden;
}

.carousel-item.active {
    left: 0;
}
</style>
