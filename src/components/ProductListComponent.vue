<template>
    <section>
        <div class="container">
            <div class="products">
                <ProductCardComponent v-for="product in products.products" :key="product.id" :product="product" />
            </div>
        </div>
    </section>
</template>

<script>
import ProductCardComponent from './ProductCardComponent.vue';
import products from '../assets/data/db.json';

export default {
    name: 'ProductListComponent',
    components: {
        ProductCardComponent
    },
    data() {
        return {
            products: products
        }
    }
};
</script>

<style scoped lang="scss">
// Stile del componente
</style>

<style scoped lang="scss">
// section {
//     padding: 60px 0;
// }

.products {
    display: flex;
    flex-wrap: wrap;
}
</style>
