<template>
    <div class="col-33">
    <div class="content">
    <img class="main-image" :src="product.mainImage" :alt="`prodotto ${product.id}`">
    <img class="hover-image" :src="product.hoverImage" :alt="`prodotto ${product.id}b`">
    <div v-if="product.discount" class="discount-label bg-red">{{ product.discount }}</div>
    <div v-if="product.sustainability" class="sustainability-label bg-green">Sostenibilità</div>
    <div class="red-heart">&hearts;</div>
    <div class="brand">{{ product.brand }}</div>
    <h2>{{ product.name }}</h2>
    <div class="price">{{ product.price }} &euro;</div>
    <div v-if="product.oldPrice" class="old-price">{{ product.oldPrice }} &euro;</div>
    </div>
</div>
</template>

<script>
export default {
name: 'ProductCardComponent',
props: {
    product: {
    type: Object,
    required: true
    }
}
}
</script>

<style scoped lang="scss">
.col-33 {
    flex: 1 1 33%;
    max-width: 33%;
}

.content {
    position: relative;
    padding: 20px;
    border: 1px solid #eee;
}

.main-image, .hover-image {
    width: 100%;
    transition: opacity 0.3s;
}

.hover-image {
    position:absolute;
    top: 0;
    left: 0;
    opacity: 0;
}

.content:hover .hover-image {
    opacity: 1;
}

.discount-label,
.sustainability-label,
.label-left {
    position: absolute;
top: 10px;
left: 10px;
padding: 5px 10px;
color: #fff;
font-weight: bold;
}

.bg-red {
background-color: red;
}

.bg-green {
background-color: green;
}

.red-heart {
position: absolute;
top: 10px;
right: 10px;
color: red;
}

.brand {
font-weight: bold;
margin-top: 10px;
}

.price {
color: red;
font-size: 18px;
font-weight: bold;
}

.old-price {
text-decoration: line-through;
color: #999;
}
</style>