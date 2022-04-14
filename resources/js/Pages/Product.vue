<template>
    <Nav />
    <div class="container px-4 pt-8 sm:px-8 md:px-2 lg:px-8 mx-auto">
        <Header :headerName="pageName"/>
        <div class="flex flex-wrap -mx-px overflow-hidden sm:-mx-px md:-mx-1 lg:-mx-px xl:-mx-1">
            <ProductItem/>
        </div>
    </div>
</template>
<script>
import Header from '../Components/Header.vue';
import ProductItem from '../Components/ProductItem.vue';
import Nav from "../Shared/Nav";


export default {
    components: {
        Nav,ProductItem,Header
    },
    data() {
        return {
            pageName: "Food / Canned Food",
        };
    },
};
</script>
