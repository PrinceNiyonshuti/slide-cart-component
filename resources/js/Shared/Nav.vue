<template>
    <div
        class="w-screen flex flex-row items-center p-1 justify-between bg-white shadow-lg"
    >
        <div class="ml-8 text-lg text-gray-700 hidden md:flex">CaniClub</div>
        <span
            class="w-screen md:w-1/3 h-10 bg-gray-200 cursor-pointer border border-gray-300 text-sm rounded-lg flex"
        >
            <input
                type="search"
                name="serch"
                placeholder="Search item"
                class="flex-grow px-4 rounded-lg text-sm focus:outline-none"
            />
        </span>
        <div class="flex flex-row-reverse mr-4 ml-4 md:hidden">
            <i class="fas fa-bars"></i>
        </div>
        <div class="flex flex-row mr-8 hidden md:flex">
            <div class="text-gray-900 font-bold text-center px-4 py-2 m-2">
                <Link href="/">Home</Link>
            </div>
            <div class="text-gray-900 font-bold text-center px-4 py-2 m-2">
                <Link href="/Product">Categories</Link>
            </div>
            <div class="text-gray-900 font-bold text-center px-4 py-2 m-2">
                <Link href="/SpecialProduct">Shops</Link>
            </div>
            <Link
                href="/Cart"
                class="relative inline-block text-gray-700 text-center bg-gray-700 px-2 py-2 m-2 rounded-full"
            >
                <svg
                    class="flex-1 w-8 h-8 pl-1 pt-1 fill-white"
                    viewbox="0 0 24 24"
                >
                    <path
                        d="M17,18C15.89,18 15,18.89 15,20A2,2 0 0,0 17,22A2,2 0 0,0 19,20C19,18.89 18.1,18 17,18M1,2V4H3L6.6,11.59L5.24,14.04C5.09,14.32 5,14.65 5,15A2,2 0 0,0 7,17H19V15H7.42A0.25,0.25 0 0,1 7.17,14.75C7.17,14.7 7.18,14.66 7.2,14.63L8.1,13H15.55C16.3,13 16.96,12.58 17.3,11.97L20.88,5.5C20.95,5.34 21,5.17 21,5A1,1 0 0,0 20,4H5.21L4.27,2M7,18C5.89,18 5,18.89 5,20A2,2 0 0,0 7,22A2,2 0 0,0 9,20C9,18.89 8.1,18 7,18Z"
                    />
                </svg>
            </Link>
            <Link
                href="/"
                class="relative inline-block text-gray-700 text-center bg-gray-500 px-2 py-2 m-2 rounded-full"
            >
                <img
                    class="object-cover w-8 h-8 rounded-full"
                    src="https://images.unsplash.com/photo-1520315342629-6ea920342047?ixid=MnwxMjA3fDB8MHxzZWFyY2h8MjR8fGNhdHxlbnwwfHwwfHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60"
                    alt="Avatar"
                />
            </Link>
        </div>
    </div>
</template>
<script>
import { Link } from "@inertiajs/inertia-vue3";
export default {
    components: {
        Link,
    },
};
</script>
