<template>
    <div class="flex items-center justify-between">
        <div class="my-2 mb-10">
            <h2 class="text-base md:text-2xl lg:text-3xl font-bold">
                {{ headerName }}
            </h2>
        </div>
        <div class="absolute right-4 my-2 mb-10 justify-items-end">
            <!-- Dropdown toggle button -->
            <button
                @click="show = !show"
                class="invisible md:visible lg:visible bg-gray-200 font-medium rounded-lg text-sm px-4 py-2.5 text-center inline-flex items-start"
            >
                <span class="mr-4">Best Selling</span>
                <svg
                    class="w-5 h-5 text-indigo-100 dark:text-white"
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
            </button>

            <button
                @click="show = !show"
                v-on:click="away()"
                class="md:hidden lg:hidden bg-gray-200 font-medium rounded-lg text-sm px-4 py-2.5 text-center inline-flex items-start"
            >
                <svg
                    width="20"
                    height="20"
                    viewBox="0 0 16 16"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                >
                    <path
                        d="M1.02498 2.2488C2.84298 4.5798 6.19998 8.8998 6.19998 8.8998V14.2998C6.19998 14.7948 6.60498 15.1998 7.09998 15.1998H8.89998C9.39498 15.1998 9.79998 14.7948 9.79998 14.2998V8.8998C9.79998 8.8998 13.148 4.5798 14.966 2.2488C15.425 1.6548 15.002 0.799805 14.255 0.799805H1.73598C0.988977 0.799805 0.565977 1.6548 1.02498 2.2488Z"
                        fill="white"
                    />
                </svg>
            </button>

            <!-- Dropdown menu -->
            <div v-show="show" class="absolute z-40 right-0 py-2 mt-2 bg-white rounded divide-y divide-gray-100 shadow w-40" >
                <ul class="py-1 text-sm" aria-labelledby="dropdownDefault">
                    <li>
                        <a href="#" class="block py-2 px-4 hover:bg-gray-100"
                            >Relevance</a
                        >
                    </li>
                    <li>
                        <a href="#" class="block py-2 px-4 hover:bg-gray-100"
                            >Price: Low To High</a
                        >
                    </li>
                    <li>
                        <a href="#" class="block py-2 px-4 hover:bg-gray-100"
                            >Price: High To Low</a
                        >
                    </li>
                    <li>
                        <a href="#" class="block py-2 px-4 hover:bg-gray-100"
                            >Best Sellers</a
                        >
                    </li>
                    <li>
                        <a href="#" class="block py-2 px-4 hover:bg-gray-100"
                            >New Arrivals</a
                        >
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    props: {
        headerName: String,
    },
    data: function () {
        return {
            show: false,
        };
    },
};
</script>
