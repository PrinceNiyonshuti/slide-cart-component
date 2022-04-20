<template>
    <div class="my-px px-px w-full overflow-hidden sm:my-px sm:px-px sm:w-full md:my-1 md:w-1/2 lg:my-px lg:px-px lg:w-1/2 xl:my-1 xl:px-1 xl:w-1/2" v-for="item in items" v-bind:key="item.id">
        <div class="flex flex-wrap overflow-hidden">
            <div class="w-full overflow-hidden">
                <div class="text-slate-700  sm:px-0 md:px-0 lg:pr-4 mb-6" >
                    <div class="flex-wrap sm:flex  sm:space-x-0 md:flex-nowrap md:items-center md:space-x-0 lg:flex-nowrap lg:space-x-5 items-center mr-0 md:mr-0 lg:mr-8">
                        <div class="">
                            <Link href="/ProductDetail">
                                <img class="rounded-md w-full h-60 object-fit md:w-80 md:h-32 lg:w-60 lg:h-40 border border-gray-200" src="https://m.media-amazon.com/images/I/81OoqT9zwXL._AC_SL1500_.jpg" alt="brad" />
                            </Link>
                        </div>
                        <div class="mt-2 md:mt-0 md:px-4 md:h-full">
                            <h1 class="text-xl font-bold md:text-base lg:text-xl">
                                <Link href="/ProductDetail">Cesar Classics</Link>
                            </h1>
                            <p class=" md:max-w-lg md:text-sm md:tracking-tighter lg:text-base lg:tracking-normal">The wide ranging nature of items and practices to which the term creative can be sensibly applied </p>
                            <p class="text-xl font-semibold md:text-base lg:text-xl">24 €</p>
                            <div class="flex items-center justify-between mt-2 ">
                                <button class="flex items-center font-semibold text-orange-500  md:text-sm lg:text-base">
                                    <svg class="flex-1 w-6 md:w-4 lg:w-6 pr-1 pt-1 " viewBox="0 0 15 15" xmlns="http://www.w3.org/2000/svg">
                                        <path d="M4.5 12C3.675 12 3.0075 12.675 3.0075 13.5C3.0075 14.325 3.675 15 4.5 15C5.325 15 6 14.325 6 13.5C6 12.675 5.325 12 4.5 12ZM0 0V1.5H1.5L4.2 7.1925L3.1875 9.03C3.0675 9.24 3 9.4875 3 9.75C3 10.575 3.675 11.25 4.5 11.25H13.5V9.75H4.815C4.71 9.75 4.6275 9.6675 4.6275 9.5625L4.65 9.4725L5.325 8.25H10.9125C11.475 8.25 11.97 7.9425 12.225 7.4775L14.91 2.61C14.97 2.505 15 2.3775 15 2.25C15 1.8375 14.6625 1.5 14.25 1.5H3.1575L2.4525 0H0ZM12 12C11.175 12 10.5075 12.675 10.5075 13.5C10.5075 14.325 11.175 15 12 15C12.825 15 13.5 14.325 13.5 13.5C13.5 12.675 12.825 12 12 12Z" fill="#FF6C00"/>
                                    </svg>
                                    Add to cart
                                </button>
                                <button class="flex items-center font-semibold  md:text-sm lg:text-base">
                                    <svg class="flex-1 w-8 md:w-6 lg:w-8 pr-1 pt-1 "  viewBox="0 0 18 13"  xmlns="http://www.w3.org/2000/svg">
                                        <path d="M17.3327 2.83336H9.83268V4.50002H17.3327V2.83336ZM17.3327 9.50002H9.83268V11.1667H17.3327V9.50002ZM3.61602 6.16669L0.666016 3.21669L1.84102 2.04169L3.60768 3.80836L7.14102 0.275024L8.31602 1.45002L3.61602 6.16669ZM3.61602 12.8334L0.666016 9.88336L1.84102 8.70836L3.60768 10.475L7.14102 6.94169L8.31602 8.11669L3.61602 12.8334Z" fill="#D0D0D0"/>
                                    </svg>
                                    Add to wishlist
                                </button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
import { Link } from '@inertiajs/inertia-vue3'

export default {
    components: {
        Link,
    },
    props: {
        items: Number,
    },
}
</script>
