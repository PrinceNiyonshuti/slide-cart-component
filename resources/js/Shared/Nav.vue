<template>
    <div class="w-full px-4 md:px-2 lg:px-8 flex flex-row items-center p-1 justify-between bg-white shadow-lg">
        <div class="w-1/3 sm:w-0/3 md:w-1/3 lg:w-1/3  ml-8 text-lg text-gray-700 hidden md:flex">
            CaniClub
        </div>
        <div class="w-1/3 sm:w-0/3 md:w-1/3 lg:1/3 h-10 px-1 cursor-pointer border border-gray-300 text-sm rounded-lg flex justify-start hidden md:flex">
            <div class="container flex justify-center items-center">
                <svg class="w-fit h-6 " fill="currentColor" xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 24 24">
                    <path
                        d="M16.32 14.9l5.39 5.4a1 1 0 0 1-1.42 1.4l-5.38-5.38a8 8 0 1 1 1.41-1.41zM10 16a6 6 0 1 0 0-12 6 6 0 0 0 0 12z">
                    </path>
                </svg>
                <input
                    type="search"
                    name="search"
                    placeholder="Search item"
                    class="w-fit flex-grow px-2 rounded-lg text-sm focus:outline-none"
                />
            </div>
        </div>
        <div class="w-1/1 sm:w-3/3 md:w-1/3 lg:1/3 flex-row md:flex justify-between">
            <!-- Sidebar Modal toggle button -->
            <div @click="modal = !modal" class="md:block lg:hidden relative inline-block text-gray-700 text-center item-center ml-2 px-2 py-6">
                <svg class="" width="18" height="16" viewBox="0 0 18 16" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M0 0H18V2H0V0ZM0 7H12V9H0V7ZM0 14H18V16H0V14Z" fill="#3F3F44"/>
                </svg>
            </div>
            <!-- Sidebar Modal menu -->
            <div v-show="modal" class="absolute flex justify-between -mt-1 -ml-1 left-1 z-40 w-full min-h-screen" >
                <div class="sticky w-2/3 px-4 bg-white w-68">
                    <div class="text-lg text-gray-700">CaniClub</div>
                    <div class=" mt-4">
                        <ul class="py-1 text-sm" aria-labelledby="dropdownDefault">
                            <li>
                                <Link class="block py-1 px-4 hover:bg-gray-100 text-gray-900 font-bold " href="/">Home</Link>
                            </li>
                            <li>
                                <div class="relative justify-items-end">
                                    <!-- Dropdown toggle button -->
                                    <span
                                        @click="show = !show"
                                        class=" font-bold sm:visible md:visible lg:visible  text-center inline-flex items-start"
                                    >
                                        <span class="mr-2 px-4">Categories</span>
                                        <svg
                                            class="w-5 h-5 text-indigo-100 dark:text-white mt-1"
                                            xmlns="http://www.w3.org/2000/svg"
                                            viewBox="0 0 20 20"
                                            fill="black"
                                        >
                                            <path
                                                fill-rule="evenodd"
                                                d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                                                clip-rule="evenodd"
                                            />
                                        </svg>
                                    </span>
                                    <!-- Dropdown menu -->
                                    <div v-show="show" class="block left-2 py-2 px-4 w-64" >
                                        <div v-for="item in 4" v-bind:key="item.id">
                                            <span class="font-semibold">Food</span>
                                            <ul class="py-1 text-sm" aria-labelledby="dropdownDefault">
                                                <li>
                                                    <a href="#" class="block py-1 px-4 hover:bg-gray-100"
                                                        >Dry food</a
                                                    >
                                                </li>
                                                <li>
                                                    <a href="#" class="block py-1 px-4 hover:bg-gray-100"
                                                        >Canned food</a
                                                    >
                                                </li>
                                                <li>
                                                    <a href="#" class="block py-1 px-4 hover:bg-gray-100"
                                                        >Puppy food</a
                                                    >
                                                </li>
                                                <li>
                                                    <a href="#" class="block py-1 px-4 hover:bg-gray-100"
                                                        >Veternary autorised diets</a
                                                    >
                                                </li>
                                            </ul>
                                        </div>
                                    </div>
                                </div>
                            </li>
                            <li>
                                <Link class="block py-1 px-4 hover:bg-gray-100 text-gray-900 font-bold " href="/Shop">Shops</Link>
                            </li>
                        </ul>
                    </div>
                </div>
                <div @click="modal = !modal" class="w-full bg-gray-900 opacity-75">
                    asdasd
                </div>
            </div>
            <div class="hidden sm:hidden md:hidden lg:block text-gray-900 font-bold text-center px-1 py-2 m-2">
                <Link href="/">Home</Link>
            </div>
            <div class="hidden sm:hidden md:hidden lg:block text-gray-900 px-1 py-2 m-2">
                <div class="relative justify-items-end">
                    <!-- Dropdown toggle button -->
                    <span
                        @click="show = !show"
                        class="invisible font-bold md:visible lg:visible  text-center inline-flex items-start"
                    >
                        <span class="mr-2">Categories</span>
                        <svg
                            class="w-5 h-5 text-indigo-100 dark:text-white mt-1"
                            xmlns="http://www.w3.org/2000/svg"
                            viewBox="0 0 20 20"
                            fill="black"
                        >
                            <path
                                fill-rule="evenodd"
                                d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                                clip-rule="evenodd"
                            />
                        </svg>
                    </span>
                    <!-- Dropdown menu -->
                    <div v-show="show" class="absolute z-40 right-0 py-2 px-4 mt-2 bg-white rounded  shadow w-64" >
                        <div v-for="item in 4" v-bind:key="item.id">
                            <span class="font-semibold">Food</span>
                            <ul class="py-1 text-sm" aria-labelledby="dropdownDefault">
                                <li>
                                    <a href="#" class="block py-1 px-4 hover:bg-gray-100"
                                        >Dry food</a
                                    >
                                </li>
                                <li>
                                    <a href="#" class="block py-1 px-4 hover:bg-gray-100"
                                        >Canned food</a
                                    >
                                </li>
                                <li>
                                    <a href="#" class="block py-1 px-4 hover:bg-gray-100"
                                        >Puppy food</a
                                    >
                                </li>
                                <li>
                                    <a href="#" class="block py-1 px-4 hover:bg-gray-100"
                                        >Veternary autorised diets</a
                                    >
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
            <div class="hidden sm:hidden md:hidden lg:block text-gray-900 font-bold text-center px-2 py-2 m-2">
                <Link href="/Shop">Shops</Link>
            </div>
            <Link href="/search" class="block sm:block md:hidden lg:hidden ml-36 relative inline-block text-center bg-gray-200 px-2 py-2 m-2 rounded-full  ">
                <svg  class="flex-1 w-8 h-8 fill-white" viewBox="0 0 18 17" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M13.6246 11.6934L17.051 15.119L15.919 16.251L12.4934 12.8246C11.2188 13.8463 9.63341 14.4021 7.9998 14.3998C4.0254 14.3998 0.799805 11.1742 0.799805 7.19976C0.799805 3.22536 4.0254 -0.000244141 7.9998 -0.000244141C11.9742 -0.000244141 15.1998 3.22536 15.1998 7.19976C15.2021 8.83336 14.6464 10.4187 13.6246 11.6934ZM12.0198 11.0998C13.0351 10.0557 13.6021 8.6561 13.5998 7.19976C13.5998 4.10536 11.0934 1.59976 7.9998 1.59976C4.9054 1.59976 2.3998 4.10536 2.3998 7.19976C2.3998 10.2934 4.9054 12.7998 7.9998 12.7998C9.45615 12.802 10.8557 12.235 11.8998 11.2198L12.0198 11.0998Z" fill="#3F3F44" fill-opacity="0.3"/>
                </svg>
            </Link>
            <Link href="/Cart" class="relative inline-block text-gray-700 text-center bg-gray-400 px-2 py-2 m-2 rounded-full">
                <svg class="flex-1 w-8 h-8 pl-1 pt-1 fill-white" viewbox="0 0 24 24" >
                    <path d="M17,18C15.89,18 15,18.89 15,20A2,2 0 0,0 17,22A2,2 0 0,0 19,20C19,18.89 18.1,18 17,18M1,2V4H3L6.6,11.59L5.24,14.04C5.09,14.32 5,14.65 5,15A2,2 0 0,0 7,17H19V15H7.42A0.25,0.25 0 0,1 7.17,14.75C7.17,14.7 7.18,14.66 7.2,14.63L8.1,13H15.55C16.3,13 16.96,12.58 17.3,11.97L20.88,5.5C20.95,5.34 21,5.17 21,5A1,1 0 0,0 20,4H5.21L4.27,2M7,18C5.89,18 5,18.89 5,20A2,2 0 0,0 7,22A2,2 0 0,0 9,20C9,18.89 8.1,18 7,18Z"/>
                </svg>
            </Link>
            <Link href="/SpecialProduct" class="relative inline-block text-gray-700 text-center bg-gray-500 px-2 py-2 m-2 rounded-full">
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
    data: function () {
        return {
            show: false,
            modal: false,
        };
    },
};
</script>
