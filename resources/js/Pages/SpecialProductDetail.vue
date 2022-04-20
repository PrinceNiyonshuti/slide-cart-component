<template>
    <Nav />
    <div class="container px-4 pt-8 sm:px-8 md:px-2 lg:px-8 mx-auto">
        <ProductDetailHeader :itemName="itemName"/>
        <SpecialItemDetail/>
        <div class="flex flex-row items-center">
            <div class="my-2 mb-10">
                <h2 class="text-base md:text-2xl lg:text-2xl font-bold">
                    Similal Items
                </h2>
            </div>
        </div>

        <div class="flex flex-wrap -mx-px overflow-hidden sm:-mx-px md:-mx-1 lg:-mx-px xl:-mx-1">
            <SpecialProductItem :items="2"/>
        </div>

        <Shops/>
    </div>
</template>
<script>
import Nav from "../Shared/Nav";
import ProductDetailHeader from "../Components/ProductDetailHeader.vue";
import SpecialItemDetail from '../Components/SpecialItemDetail.vue';
import SpecialProductItem from '../Components/SpecialProductItem.vue';
import Shops from '../Components/Shops.vue';

export default {
    components: {
        Nav,
        ProductDetailHeader,
        SpecialItemDetail,
        SpecialProductItem,
        Shops
    },
    data() {
        return {
            itemName: "Canidae/ Lyme vaccine",
        };
    },
};
</script>
