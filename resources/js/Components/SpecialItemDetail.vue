<template>
    <div class="flex flex-wrap -mx-1 overflow-hidden sm:-mx-1 md:-mx-1 lg:-mx-1 xl:-mx-1">
        <div class="my-1 px-1 w-full overflow-hidden sm:my-1 sm:px-1 sm:w-1/2 md:my-1 md:px-1 md:w-1/2 lg:my-1 lg:px-1 lg:w-1/2 xl:my-1 xl:px-1 xl:w-1/2">
            <img alt="Dog Tags" class="w-full h-5/6 object-fit object-center rounded border border-gray-200" src="https://m.media-amazon.com/images/I/71cPvIqZ+wL._AC_SX425_.jpg">
        </div>

        <div class="my-1 px-1 w-full overflow-hidden sm:my-1 sm:px-1 sm:w-1/2 md:my-1 md:px-1 md:w-1/2 lg:my-1 lg:px-1 lg:w-1/2 xl:my-1 xl:px-1 xl:pl-4 xl:w-1/2">
            <div class="flex justify-between px-2">
                <span class="text-xl">Price</span>
                <span class="font-semibold text-4xl">€ 20</span>
            </div>
            <div class="flex flex-col px-2 py-1">
                <span class="text-lg font-medium">Item description</span>
                <p class="pt-2 text-base">
                    Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aeneanommodo ligula eget dolor. Aenean massa. Cum sociis natoque
                    Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo, fringilla vel, aliquet nec,
                    vulputate eget, arcu. In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo. Nullam dictum felis eu pede mollis pretium. Integer tincidunt. Cras dapibus. Vivamus elementum semper nisi. Aenean vulputate eleifend tellus.
                </p>
            </div>
            <div class="relative px-2 py-1 mt-4 mr-8 lg:mr-12 ">
                <select class="block appearance-none w-full border border-gray-500 text-gray-700 py-2 px-4 mr-40 rounded leading-tight " >
                    <option>Select dog</option>
                    <option>Select dog</option>
                    <option>Select dog</option>
                </select>
                <div class="pointer-events-none absolute inset-y-0 right-0 flex items-center px-2 text-gray-700">
                    <svg class="fill-current h-4 w-4" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M9.293 12.95l.707.707L15.657 8l-1.414-1.414L10 10.828 5.757 6.586 4.343 8z"/></svg>
                </div>
            </div>
            <div class="flex items-center justify-between mt-4">
                <button class="flex text-white font-semibold bg-orange-600 rounded border-0 py-2 px-6 focus:outline-none">
                    <svg class="flex-1 w-6 md:w-4 lg:w-6 pr-1 pt-1 " viewBox="0 0 15 15" xmlns="http://www.w3.org/2000/svg">
                        <path d="M4.5 12C3.675 12 3.0075 12.675 3.0075 13.5C3.0075 14.325 3.675 15 4.5 15C5.325 15 6 14.325 6 13.5C6 12.675 5.325 12 4.5 12ZM0 0V1.5H1.5L4.2 7.1925L3.1875 9.03C3.0675 9.24 3 9.4875 3 9.75C3 10.575 3.675 11.25 4.5 11.25H13.5V9.75H4.815C4.71 9.75 4.6275 9.6675 4.6275 9.5625L4.65 9.4725L5.325 8.25H10.9125C11.475 8.25 11.97 7.9425 12.225 7.4775L14.91 2.61C14.97 2.505 15 2.3775 15 2.25C15 1.8375 14.6625 1.5 14.25 1.5H3.1575L2.4525 0H0ZM12 12C11.175 12 10.5075 12.675 10.5075 13.5C10.5075 14.325 11.175 15 12 15C12.825 15 13.5 14.325 13.5 13.5C13.5 12.675 12.825 12 12 12Z" fill="white"/>
                    </svg>
                    Add to cart
                </button>
                <button class="flex text-orange-500 font-semibold rounded border-2 border-orange-500 py-2 px-6 focus:outline-none">
                    <svg class="flex-1 w-8 md:w-6 lg:w-8 pr-1 pt-1 "  viewBox="0 0 18 13"  xmlns="http://www.w3.org/2000/svg">
                        <path d="M17.3327 2.83336H9.83268V4.50002H17.3327V2.83336ZM17.3327 9.50002H9.83268V11.1667H17.3327V9.50002ZM3.61602 6.16669L0.666016 3.21669L1.84102 2.04169L3.60768 3.80836L7.14102 0.275024L8.31602 1.45002L3.61602 6.16669ZM3.61602 12.8334L0.666016 9.88336L1.84102 8.70836L3.60768 10.475L7.14102 6.94169L8.31602 8.11669L3.61602 12.8334Z" fill="#FF6C00"/>
                    </svg>
                    Add to wishlist
                </button>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
