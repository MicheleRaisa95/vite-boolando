<template>
    <div class="container">
        <div class="row">
            <ProductCardComponent v-for="product in products" :key="product.id" :product="product" />
        </div>
    </div>
</template>

<script>
import ProductCardComponent from './ProductCardComponent.vue'

export default {
    name: 'ProductListComponent',
    components: {
        ProductCardComponent
    },
    data() {
        return {
            products: [
                {
                    id: 1,
                    mainImage: './assets/img/1.webp',
                    hoverImage: './assets/img/1b.webp',
                    discount: '-50%',
                    sustainability: true,
                    brand: "Levi's",
                    name: 'relaxed fit tee unisex',
                    price: 14.99,
                    oldPrice: 29.99
                },
                {
                    id: 2,
                    mainImage: './assets/img/2.webp',
                    hoverImage: './assets/img/2b.webp',
                    discount: '-30%',
                    brand: 'Guess',
                    name: 'roses tee',
                    price: 20.99,
                    oldPrice: 29.99
                },
                {
                    id: 3,
                    mainImage: './assets/img/3.webp',
                    hoverImage: './assets/img/3b.webp',
                    discount: '-30%',
                    brand: 'Guess',
                    name: 'roses tee',
                    price: 20.99,
                    oldPrice: 29.99
                },
                {
                    id: 4,
                    mainImage: './assets/img/4.webp',
                    hoverImage: './assets/img/4b.webp',
                    discount: '-30%',
                    brand: 'Guess',
                    name: 'roses tee',
                    price: 20.99,
                    oldPrice: 29.99
                },
                {
                    id: 5,
                    mainImage: './assets/img/5.webp',
                    hoverImage: './assets/img/5b.webp',
                    discount: '-30%',
                    brand: 'Guess',
                    name: 'roses tee',
                    price: 20.99,
                    oldPrice: 29.99
                },
                {
                    id: 4,
                    mainImage: './assets/img/6.webp',
                    hoverImage: './assets/img/6b.webp',
                    discount: '-30%',
                    brand: 'Guess',
                    name: 'roses tee',
                    price: 20.99,
                    oldPrice: 29.99
                },
            ]
        };
    }
}
</script>

<style scoped>
.container {
display: flex;
justify-content: space-between;
align-items: center;
}

.row {
display: flex;
flex-wrap: wrap;
}
</style>