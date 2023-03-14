<script>
import NavBar from './NavBar.vue'
import CartItem from './CartItem.vue'
export default {
    components: { NavBar, CartItem },
    data(){
        return{
            cart: {},
            total: 0
        }
    }
}
</script>

<template>
    <body>
        <NavBar></NavBar>
        <p>Cart: {{ cart }}</p>
        <p> Total Price: ${{ total }}</p>
        <CartItem name='Pickledog' desc="A disgusting hotdog with a pickle on the top. Smells terrible" price="5.50" url="https://i.ibb.co/swr7JHK/Pickledog.png"></CartItem>
        <CartItem name='Cookiedog' desc="A tasty hotdog with chocolate sprinkled on top. Smells amazing" price="5.50" url="https://i.ibb.co/WDwff6q/Cookiedog.png"></CartItem>
        <CartItem name='Cheddardog' desc="A very cheesy dog." price="5.50" url="https://i.ibb.co/3TLr0YR/Cheddardog.jpg"></CartItem>
        <CartItem name='Eggdog' desc="An eggdog... I don't know why" price="5.50" url="https://i.ibb.co/1rCqC2S/Eggdog.jpg"></CartItem>
    </body>
</template>

<style scoped></style>
