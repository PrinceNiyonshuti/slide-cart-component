<template>
    <Nav />

    <div id="default-carousel" class="relative" data-carousel="static">
        <div
            class="overflow-hidden relative h-96 sm:h-64 xl:h-[450px] 2xl:h-96"
        >
            <div
                class="duration-700 ease-in-out absolute inset-0 transition-all transform translate-x-0 z-20"
                data-carousel-item=""
                v-for="image in images"
                v-bind:key="image.id"
            >
                <img
                    src="../../../public/images/1.png"
                    class="block absolute top-1/2 left-1/2 w-full h-full -translate-x-1/2 -translate-y-1/2"
                    alt="..."
                />
                <button
                    class="object-fill absolute bottom-[4rem] left-[12rem] sm:left-[1rem] flex rounded-[3.31px] bg-white px-6 py-2"
                >
                    Shop Now
                </button>
            </div>
        </div>

        <div
            class="flex absolute bottom-5 left-1/2 z-30 space-x-3 -translate-x-1/2"
        >
            <button
                type="button"
                class="w-3 h-3 rounded-full bg-white dark:bg-gray-800"
                aria-current="true"
                aria-label="Slide 1"
                data-carousel-slide-to="0"
                v-for="image in images"
                v-bind:key="image.id"
            ></button>
        </div>

        <button
            type="button"
            class="flex absolute top-0 left-0 z-30 justify-center items-center px-4 h-full cursor-pointer group focus:outline-none"
            data-carousel-prev=""
        >
            <span
                class="inline-flex justify-center items-center w-8 h-8 rounded-full sm:w-10 sm:h-10 bg-white/30 dark:bg-gray-800/30 group-hover:bg-white/50 dark:group-hover:bg-gray-800/60 group-focus:ring-4 group-focus:ring-white dark:group-focus:ring-gray-800/70 group-focus:outline-none"
            >
                <svg
                    class="w-5 h-5 text-white sm:w-6 sm:h-6 dark:text-gray-800"
                    fill="none"
                    stroke="currentColor"
                    viewBox="0 0 24 24"
                    xmlns="http://www.w3.org/2000/svg"
                >
                    <path
                        stroke-linecap="round"
                        stroke-linejoin="round"
                        stroke-width="2"
                        d="M15 19l-7-7 7-7"
                    ></path>
                </svg>
                <span class="hidden">Previous</span>
            </span>
        </button>
        <button
            type="button"
            class="flex absolute top-0 right-0 z-30 justify-center items-center px-4 h-full cursor-pointer group focus:outline-none"
            data-carousel-next=""
        >
            <span
                class="inline-flex justify-center items-center w-8 h-8 rounded-full sm:w-10 sm:h-10 bg-white/30 dark:bg-gray-800/30 group-hover:bg-white/50 dark:group-hover:bg-gray-800/60 group-focus:ring-4 group-focus:ring-white dark:group-focus:ring-gray-800/70 group-focus:outline-none"
            >
                <svg
                    class="w-5 h-5 text-white sm:w-6 sm:h-6 dark:text-gray-800"
                    fill="none"
                    stroke="currentColor"
                    viewBox="0 0 24 24"
                    xmlns="http://www.w3.org/2000/svg"
                >
                    <path
                        stroke-linecap="round"
                        stroke-linejoin="round"
                        stroke-width="2"
                        d="M9 5l7 7-7 7"
                    ></path>
                </svg>
                <span class="hidden">Next</span>
            </span>
        </button>
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
        const prevButton = document.getElementById("data-carousel-prev");
        const nextButton = document.getElementById("data-carousel-next");

        prevButton.addEventListener("click", () => {
            carousel.prev();
        });

        nextButton.addEventListener("click", () => {
            carousel.next();
        });

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

