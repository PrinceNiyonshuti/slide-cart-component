<template>
    <table
        class=" overflow-x-auto sm:w-1/2 md:w-1/2 lg:w-3/4 xl:w-3/4 h-full grow-0 border border-gray-200 hidden lg:block"
    >
        <thead>
            <tr class="bg-gray-200">
                <td colspan="8" class="px-8 py-2">
                    <span class="font-bold text-orange-600">Shop</span>
                    <span class="pl-4">{{ shopName }}</span>
                </td>
            </tr>
            <tr class="border-b-solid border-[1px] border-grey-400">
                <th class="px-6 py-3 whitespace-nowrap">Image</th>
                <th class="px-6 py-3 whitespace-nowrap">Item name</th>
                <th class="px-6 py-3 whitespace-nowrap">Size</th>
                <th class="px-6 py-3 whitespace-nowrap">Color</th>
                <th class="px-6 py-3 whitespace-nowrap">Price</th>
                <th class="px-6 py-3 whitespace-nowrap">Quantity</th>
                <th class="px-2 py-3 whitespace-nowrap">Total</th>
                <th class="py-3 whitespace-nowrap"></th>
            </tr>
        </thead>
        <tbody v-for="item in items" v-bind:key="item.id">
            <tr class="border-b border-gray-200">
                <td class="py-2">
                    <div
                        class="flex justify-center flex-shrink-0 overflow-hidden rounded-md"
                    >
                        <img
                            src="https://tailwindui.com/img/ecommerce-images/shopping-cart-page-04-product-01.jpg"
                            class="object-cover h-[80px] w-[80px] border border-gray-200"
                            alt="image"
                        />
                    </div>
                </td>
                <td class="p-4 px-6 text-center whitespace-nowrap">
                    <div class="flex flex-col items-center justify-center">
                        <h3>Tennis ball</h3>
                    </div>
                </td>
                <td class="p-4 px-6 text-center whitespace-nowrap">Large</td>
                <td class="p-4 px-6 text-center whitespace-nowrap">
                    <div
                        class="w-8 h-8 bg-orange-600 rounded-full mx-auto"
                    ></div>
                </td>
                <td class="p-4 px-6 text-center whitespace-nowrap">25 €</td>
                <td class="p-4 text-center whitespace-nowrap">
                    <div class="border border-gray-200">
                        <button>
                            <svg
                                xmlns="http://www.w3.org/2000/svg"
                                class="inline-flex w-6 h-6 text-red-600"
                                fill="none"
                                viewBox="0 0 24 24"
                                stroke="currentColor"
                            >
                                <path
                                    stroke-linecap="round"
                                    stroke-linejoin="round"
                                    stroke-width="2"
                                    d="M15 12H9m12 0a9 9 0 11-18 0 9 9 0 0118 0z"
                                />
                            </svg>
                        </button>
                        <input
                            type="text"
                            name="qty"
                            value="2"
                            class="w-12 text-center bg-gray-100 outline-none"
                        />
                        <button>
                            <svg
                                xmlns="http://www.w3.org/2000/svg"
                                class="inline-flex w-6 h-6 text-green-600"
                                fill="none"
                                viewBox="0 0 24 24"
                                stroke="currentColor"
                            >
                                <path
                                    stroke-linecap="round"
                                    stroke-linejoin="round"
                                    stroke-width="2"
                                    d="M12 9v3m0 0v3m0-3h3m-3 0H9m12 0a9 9 0 11-18 0 9 9 0 0118 0z"
                                />
                            </svg>
                        </button>
                    </div>
                </td>
                <td class="p-4 px-2 text-center whitespace-nowrap">50 €</td>
                <td class="p-4 text-center whitespace-nowrap">
                    <button>
                        <svg
                            xmlns="http://www.w3.org/2000/svg"
                            class="w-6 h-6 text-red-400"
                            fill="none"
                            viewBox="0 0 24 24"
                            stroke="currentColor"
                        >
                            <path
                                stroke-linecap="round"
                                stroke-linejoin="round"
                                stroke-width="2"
                                d="M19 7l-.867 12.142A2 2 0 0116.138 21H7.862a2 2 0 01-1.995-1.858L5 7m5 4v6m4-6v6m1-10V4a1 1 0 00-1-1h-4a1 1 0 00-1 1v3M4 7h16"
                            />
                        </svg>
                    </button>
                </td>
            </tr>
        </tbody>
    </table>
</template>
<script>
export default {
    props: {
        shopName: String,
        items: Number,
    },
};
</script>
