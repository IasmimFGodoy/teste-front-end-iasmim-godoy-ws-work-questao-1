<template>
<div class="delimitador">
    <div class="bottom-products-container">
        <div class="separator-1">
            <div class="healthy-power-pills">
                <img class="img-apple" src="/img-apple.jpg" alt="apple image">
                <div class="healthy-power-pills-description">
                    <h3>Only $0.22</h3>
                    <p>Healthy power pills</p>
                    <p>Most Healhy for u</p>
                    <p id="marked-1">cheap and powerful remedy for long term healing</p>
                </div>
            </div>
            <button class="buy-now-btn">Buy now</button>
        </div>
        <hr>
        <div class="separator-2">
            <div class="best-drink">
                <img class="img-water" src="/img-water.jpg" alt="water image">
                <div class="best-drink-description">
                    <h2>best drink</h2>
                    <button class="for-free-btn">for free</button>
                    <p id="marked-2">Long term health</p>
                </div>
            </div>
            <p id="marked-3">Click here and join us with these magical benefits</p>
        </div>
    </div>
    <div class="separador">
        <FooterComponent/>
    </div>
</div>
</template>
<script>
import FooterComponent from './FooterComponent.vue';

export default {
    name: 'IndexPage',
    components: { FooterComponent }
}
</script>
<style>
.bottom-products-container, .healthy-power-pills, .best-drink{
    margin-top: 0.5rem;
    display: flex
}

.img-apple{
    width: 120px;
    height: 120px;
}
.img-water {
    width: 90px;
    height: 90px;
}
.healthy-power-pills-description {
    width:60%;
}
.healthy-power-pills-description h3 {
    font-size: 18px;
    margin-bottom: 0.5rem;
}
.healthy-power-pills-description p {
    margin-bottom: 0.2rem;
}
.bottom-products-container hr {
    margin-right: 2.5rem;
}
#marked-1 {
    font-weight: bold;
}
#marked-2{
    font-size: 18px;
}
#marked-3 {
    width: 60%;
}
.buy-now-btn, .for-free-btn {
    background-color: #8CD790;
    border: 1px solid black;
    text-transform: uppercase;
    font-size: 20px;
}
.buy-now-btn {
    padding: 5px 90px;
    font-weight: bold;
    margin-left: 1rem;
}
.for-free-btn {
    color: red;
    font-weight: bold;
    padding: 3px 15px;
}
.for-free-btn:hover,.buy-now-btn:hover {
    cursor:pointer;
    background-color: #AAFCB8 ;
}
.best-drink-description h2 {
    margin-top: 0.5rem;
    margin-bottom: 0.5rem;
}
.best-drink-description p {
    margin-top: 0.2rem;
    margin-bottom: 0.2rem;
}
.separador {
    margin-top: 0.5rem;
}
</style>