<script>
export default {
    name: 'HeaderComponent'
};
</script>

<template>
    <header>
        <div class="container">
            <nav>
            <div>
                <ul>
                    <li>
                        <a href="#">Uomo</a>
                    </li>
                    <li>
                        <a href="#">Donna</a>
                    </li>
                    <li>
                        <a href="#">Bambino</a>
                    </li>
                </ul>
            </div>
            <div>
                <img src="/image/boolean-logo.png" alt="boolando-logo">
            </div>
            <div>
                <ul>
                    <li>
                        person
                    </li>
                    <li>
                        favorite
                    </li>
                    <li>
                        shopping_bag
                    </li>
                </ul>
            </div>
            </nav>
        </div>
    </header>
</template>

<style scoped lang="scss">
header {
    background-color: #ff6900;
}
.container {
    text-align: center;
}

nav {
    display: flex;
    flex-wrap: wrap;

    img {
        display: block;
        margin-left: auto;
        margin-right: auto;
        width: 30%;
        padding: 20px;
    }
}

ul {
    display: flex;
    justify-content: center;

    li {
        padding: 20px;
    }
}
</style>