<script>
import HeaderComponent from './components/HeaderComponent.vue';


export default {
    name: 'App',
    components: {
        HeaderComponent,
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