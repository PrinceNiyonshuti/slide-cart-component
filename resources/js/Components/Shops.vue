<template>
    <div class="flex flex-row items-center">
        <div class="my-2 mb-10">
            <h2 class="text-base md:text-2xl lg:text-2xl font-bold">
                Item also available at
            </h2>
        </div>
    </div>

    <!-- Shops -->
    <div class="flex flex-wrap -mx-1 overflow-hidden sm:-mx-1 md:-mx-1 lg:-mx-1 xl:-mx-px" >

        <div class="my-1 px-1 w-1/2 overflow-hidden sm:my-1 sm:px-1 sm:w-1/2 md:my-1 md:px-1 md:w-1/4 lg:my-1 lg:px-1 lg:w-1/4 xl:my-px xl:px-px xl:w-1/4" v-for="item in 4" v-bind:key="item.id">
            <div class="mx-auto flex w-full flex-col justify-center lg:px-8 xl:px-8 ">
                <!-- img -->
                <img class="h-64 w-68 object-cover object-center rounded border border-gray-200" src="https://img.freepik.com/free-vector/cute-petshop-logo-with-cat-dog-vector_454510-133.jpg" />
                <!-- text information -->
                <div class="text-center">
                    <h1 class="text-lg font-medium text-slate-600 pb-2">Shop name</h1>
                </div>
            </div>
        </div>

    </div>
</template>
<script>
export default {

}
</script>
