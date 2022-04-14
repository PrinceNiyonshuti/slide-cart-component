<template>
    <div class="flex items-center justify-between ">
        <div class="my-2 mb-10">
            <h2 class="text-base md:text-2xl lg:text-3xl font-bold ">{{ headerName }}</h2>
        </div>
        <div class="my-2 mb-10 justify-items-end">
            <button id="dropdownDefault" data-dropdown-toggle="dropdown" class="invisible md:visible lg:visible bg-gray-200 font-medium rounded-lg text-sm px-4 py-2.5 text-center inline-flex items-start " type="button">Best Selling<svg class="ml-2 w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7"></path></svg></button>
            <button id="dropdownDefault" data-dropdown-toggle="dropdown" class="md:hidden lg:hidden bg-gray-200 font-medium rounded-lg text-sm px-4 py-2.5 text-center inline-flex items-start " type="button">
                <svg width="20" height="20" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M1.02498 2.2488C2.84298 4.5798 6.19998 8.8998 6.19998 8.8998V14.2998C6.19998 14.7948 6.60498 15.1998 7.09998 15.1998H8.89998C9.39498 15.1998 9.79998 14.7948 9.79998 14.2998V8.8998C9.79998 8.8998 13.148 4.5798 14.966 2.2488C15.425 1.6548 15.002 0.799805 14.255 0.799805H1.73598C0.988977 0.799805 0.565977 1.6548 1.02498 2.2488Z" fill="white"/>
                </svg>
            </button>
            <!-- Dropdown menu -->
            <div id="dropdown" class="hidden z-4 w-40 bg-white rounded divide-y divide-gray-100 shadow ">
                <ul class="py-1 text-sm " aria-labelledby="dropdownDefault">
                    <li>
                        <a href="#" class="block py-2 px-4 hover:bg-gray-100 ">Relevance</a>
                    </li>
                    <li>
                        <a href="#" class="block py-2 px-4 hover:bg-gray-100 ">Price: Low To High</a>
                    </li>
                    <li>
                        <a href="#" class="block py-2 px-4 hover:bg-gray-100 ">Price: High To Low</a>
                    </li>
                    <li>
                        <a href="#" class="block py-2 px-4 hover:bg-gray-100 ">Best Sellers</a>
                    </li>
                    <li>
                        <a href="#" class="block py-2 px-4 hover:bg-gray-100 ">New Arrivals</a>
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
}
</script>
