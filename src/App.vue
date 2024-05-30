<script>
import HeaderComponent from './components/HeaderComponent.vue';
import ProductListComponent from './components/ProductListComponent.vue';
import FooterComponent from './components/FooterComponent.vue'

export default {
    name: 'App',
    components: {
        HeaderComponent,
        ProductListComponent,
        FooterComponent
    }
}
</script>
<template>
<div id="app">
    <HeaderComponent />
    <ProductListComponent />
    <FooterComponent />
</div>
</template>
<style></style>