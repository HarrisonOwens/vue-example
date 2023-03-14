<script>
export default{
    props: ['url', 'name', 'desc', 'price'],
    methods:{
        AddtoCart(){
            if (this.name in this.$parent.cart){
                this.$parent.cart[this.name] += 1
            }
            else{
                this.$parent.cart[this.name] =1
            }
            this.$parent.total += Number(this.price)
        }
    }
}
</script>

<template>
    <div class="item">
        <body>
            <img :src= "url" width="300" height="300">
            <h1>{{name}}</h1>
            <p>{{desc}}</p>
            <p>This is ${{price}}</p>
            <button @click="AddtoCart">Add to Cart</button>>
        </body>
    </div>
    
</template>
  
<style>
.item {
    display: flex;
    align-items: center;
    margin-top: 2rem;
}
</style>
  
