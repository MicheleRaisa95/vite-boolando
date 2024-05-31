<template>
    <div class="card">
        <img :src="getImageUrl(product.frontImage)" :alt="product.name" class="main-image" />
        <img :src="getImageUrl(product.backImage)" :alt="product.name" class="hover-image" />
        <div v-for="badge in product.badges" :key="badge.type"
            :class="badge.type === 'tag' ? 'sustainability-label bg-green' : 'discount-label bg-red'">
            {{ badge.value }}
        </div>
        <div :class="{ 'red-heart': product.isInFavorites }">
            &hearts;
        </div>
        <div class="brand">
            {{ product.brand }}
        </div>
        <h2>
            {{ product.name }}
        </h2>
        <div class="price">
            {{ product.price }} &euro;
        </div>
    </div>
</template>

<script>
export default {
    props: {
        product: {
            type: Object,
            required: true
        }
    },
    methods: {
        getImageUrl(imageName) {
            return require(`../assets/img/${imageName}`);
        }
    }
};
</script>

<style scoped lang="scss">
.card {
    position: relative;
    border: 10px solid white;
    width: calc(100% / 3);
    text-align: center;

    img {
        width: 100%;
    }

    .hover-image {
        display: none;
    }

    &:hover .main-image {
        display: none;
    }

    &:hover .hover-image {
        display: block;
    }

    .red-heart {
        position: absolute;
        top: 10px;
        right: 10px;
        width: 35px;
        text-align: center;
        background-color: white;
        display: block;
        color: red;
    }

    .brand {
        margin-top: 10px;
    }

    h2 {
        text-transform: uppercase;
    }

    .price {
        color: red;
    }

    .sustainability-label,
    .discount-label {
        position: absolute;
        bottom: 100px;
        color: #fff;
        padding: 5px;
    }

    .sustainability-label {
        left: 10px;
        background-color: green;
    }

    .discount-label {
        right: 10px;
        background-color: red;
    }
}
</style>
