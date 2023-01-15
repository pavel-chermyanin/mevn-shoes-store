<template >
    <CartListItem v-for="product in cartItems" v-bind:key="product.id" :product="product"/>
</template>

<script>
import CartListItem from './CartListItem.vue';

export default {
    name: 'CartList',
    components: { CartListItem },
    props: ['cartItems'],

}
</script>

