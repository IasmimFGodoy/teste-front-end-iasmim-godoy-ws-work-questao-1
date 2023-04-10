<template>
        <div class="container-product1">
            <div class="product1">
                <img class="product1-img" src="/Product1.jpg" alt="capsulas de remédio">
                <div class="product1-description">
                    <h2>$ 9,99</h2>
                    <p>super supplement for your health and well being natural and 100% functional, take advantage of this offer</p>
                    <button class="product1-buy-btn">Buy</button>
                </div>
            </div>
            <div class="product1-separator">
                <hr>
            </div>
            <CarouselComponent/>
            <div class="bottom-products-separator">
                <BottomProductsComponent/>
            </div>
        </div>
    </template>
<script>
import CarouselComponent from './CarouselComponent.vue';
import BottomProductsComponent from './BottomProductsComponent.vue';

export default {
    name: "IndexPage",
    components: { CarouselComponent, BottomProductsComponent },
}
</script>
<style>
*{
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
}
.container-product1 {
    display: flex;
    flex-direction: column;    
    background-image: linear-gradient(to right, #D7FFF1, #AAFCB8);
}
.product1 {
    width: 600px;
    display: flex;
    margin-top: 1.5rem;
    margin-left: 1rem;
    float: right;
}
.product1-description {
    width: calc(59%);
    margin-left: 1rem;
}
.product1-description h2 {
    font-size: 26px;
}
.product1-img {
    width: 300px;
    height: 150px;
    object-fit: cover;
}
.product1 p, .product1 h2{
    margin-bottom: 2%;
}
.product1-description p {
    font-size: 14px;
}
.product1-buy-btn {
    background-color: #8CD790 ;
    color: black;
    padding: 4px 15px;
    border: 1px solid black;
    font-weight: bold;
    font-size: 22px;
    margin-top: 2%;
}
.product1-buy-btn:hover {
    cursor: pointer;
    background-color: #AAFCB8 ;
}
.product1-separator {
    width: 600px;
    height: 20px;
    margin-left: 1rem;
    margin-top: 1rem;
}
.product1-separator hr{
    margin-top: 2%;
    border: 1.5px solid black;
}
</style>
