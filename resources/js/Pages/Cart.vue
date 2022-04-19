<template>
    <Nav />
    <div class="container p-8 mx-auto">
        <div class="w-full overflow-x-auto">
            <div class="my-2 mb-10">
                <h2 class="text-3xl font-bold tracking-wider">My Cart</h2>
            </div>
            <div class="flex flex-wrap overflow-visible">
                <CartItems :items="1" :shopName="shopOne" />
                <CartSummary />
            </div>
            <div class="flex flex-wrap overflow-visible mt-6">
                <CartItems :items="3" :shopName="shopTwo" />
                <CartSummary />
            </div>
            <div class="flex flex-wrap overflow-visible mt-6">
                <CartItems :items="1" :shopName="shopThree" />
                <CartSummary />
            </div>
        </div>
    </div>
</template>
<script>
import CartItems from "../Components/CartItems.vue";
import CartSummary from "../Components/CartSummary.vue";
import Nav from "../Shared/Nav";

export default {
    components: {
        Nav,
        CartItems,
        CartSummary,
    },
    data() {
        return {
            shopOne: "Bamboo shop",
            shopTwo: "Doghaus",
            shopThree: "Bylen",
        };
    },
};
</script>
