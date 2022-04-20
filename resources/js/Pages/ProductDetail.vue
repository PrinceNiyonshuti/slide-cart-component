<template>
    <Nav />
    <div class="container px-4 pt-8 sm:px-8 md:px-2 lg:px-8 mx-auto">
        <ProductDetailHeader :itemName="itemName"/>
        <ItemDetails/>
        <div class="flex flex-row items-center">
            <div class="my-2 mb-10">
                <h2 class="text-base md:text-2xl lg:text-2xl font-bold">
                    Similal Items
                </h2>
            </div>
        </div>

        <div class="flex flex-wrap -mx-px overflow-hidden sm:-mx-px md:-mx-1 lg:-mx-px xl:-mx-1">
            <ProductItem :items="4"/>
        </div>
        <Shops/>
    </div>
</template>
<script>
import Nav from "../Shared/Nav";
import ProductDetailHeader from "../Components/ProductDetailHeader.vue";
import ItemDetails from '../Components/ItemDetails.vue';
import ProductItem from '../Components/ProductItem.vue';
import Shops from '../Components/Shops.vue';

export default {
    components: {
        Nav,
        ProductDetailHeader,
        ProductItem,
        ItemDetails,
        Shops
    },
    data() {
        return {
            itemName: "Bamboo shop/ Dog Tags",
        };
    },
};
</script>
