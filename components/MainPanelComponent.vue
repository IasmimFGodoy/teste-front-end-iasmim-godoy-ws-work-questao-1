<template>
        <div class="principal">
            <div class="main-panel">
                <div class="panel-content">
                    <HeaderComponent/>
                    <div class="sidebar-product-wrapper">
                        <SidebarComponent/>
                        <ProductsComponent/>
                    </div>
                </div>
            </div>
        </div>
</template>

<script>
import HeaderComponent from './HeaderComponent.vue';
import SidebarComponent from './SidebarComponent.vue';
import ProductsComponent from './ProductsComponent.vue';

export default {
    name: "IndexPage",
    components: { HeaderComponent, SidebarComponent, ProductsComponent},
}
</script>
<style>
    * {
        margin: 0;
        padding: 0;
    }
    .main-panel {
        width: 800px;
        height: 600px;
        border: 3px solid black;
        display: block;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
    }
    .panel-content {
        display: flex;
        height: 100%;
        flex-direction: column;
    }
    .sidebar-product-wrapper {
        display: flex;
        flex: 1;
    }
    .product1-separator {
        width: 600px;
    }
</style>

