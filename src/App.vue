<script>
import HeaderComponent from './components/HeaderComponent.vue';
import ProductListComponent from './components/ProductListComponent.vue'


export default {
    name: 'App',
    components: {
        HeaderComponent,
        ProductListComponent,
    },
};
</script>
<template>
<div id="app">
    <HeaderComponent />
    <ProductListComponent />
    <FooterComponent />
</div>
</template>
<style></style>