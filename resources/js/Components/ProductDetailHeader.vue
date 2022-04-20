<template>
    <div class="flex flex-row items-center">
        <div class="my-2 mb-10 pr-4">
            <Link href="#" @click="back">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M19 12H5" stroke="black" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                    <path d="M12 19L5 12L12 5" stroke="black" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                </svg>
            </Link>
        </div>
        <div class="my-2 mb-10">
            <h2 class="text-base md:text-2xl lg:text-2xl font-bold">
                Bamboo shop/ Dog Tags
            </h2>
        </div>
    </div>
</template>
<script>
import { Link } from "@inertiajs/inertia-vue3";

export default {
    components: {
        Link,
    },
    methods: {
        back() {
        window.history.back();
        },
    }
};
</script>
