<template>
    <div class="w-full overflow-hidden sm:w-full md:w-2/3 md:mt-4 lg:w-1/4 xl:w-1/4 mb-4">
        <div class="pl-4">
            <h3 class="text-lg font-semibold">CART SUMMARY</h3>
            <div class="flex justify-between px-2 py-1 mt-2 border-b-[1px]">
                <span class="font-semibold">Subtotal</span>
                <span class="font-semibold">50 €</span>
            </div>
            <div class="flex justify-between px-2 py-1 border-b-[1px]">
                <span class="font-semibold">Taxes</span>
                <span class="font-semibold">0 €</span>
            </div>
            <div class="flex justify-between px-2 py-1">
                <span class="font-semibold">Packaging</span>
                <span class="font-semibold">0 €</span>
            </div>
            <div class="flex justify-between px-2 border-b-[1px]">
                <span class="font-regular text-sm text-gray-400"
                    >Free Basic Packaging</span
                >
            </div>
            <div class="flex items-center justify-between px-2 py-2">
                <span class="font-semibold">Total</span>
                <span class="font-semibold">50</span>
            </div>
        </div>
        <div class="flex items-center justify-end">
            <button
                class="py-2 px-4 text-center text-white bg-orange-600 rounded-md shadow hover:bg-orange-500"
            >
                Buy From This Shop
            </button>
        </div>
    </div>
</template>
<script>
export default {};
</script>
