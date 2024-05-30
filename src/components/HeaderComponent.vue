<template>
    <header>
        <div class="container align-items">
            <div class="row">
                <div class="col-33">
                    <ul class="unlisted-list text-center py-10">
                        <li>
                            <a href="">Donna</a>
                        </li>
                        <li>
                            <a href="">Uomo</a>
                        </li>
                        <li>
                            <a href="">Bambini</a>
                        </li>
                    </ul>
                </div>
                <div class="col-33 py-10">
                    <img src="../assets/img/boolean-logo.png" alt="boolean" class="width logo">
                </div>
                <div class="col-33">
                    <ul class="unlisted-list text-center py-10">
                        <li>
                            <span class="material-symbols-outlined">
                                person
                                </span>
                        </li>
                        <li><span class="material-symbols-outlined">
                            favorite
                            </span></li>
                        <li><span class="material-symbols-outlined">
                            shopping_bag
                        </span></li>
                    </ul>
                </div>
            </div>
        </div>
    </header>
</template>

<!-- Script -->

<script>
export default {
    name: 'HeaderComponent'
}
</script>

<!-- /Script -->

<!-- Style -->
<style scoped lang="scss">
header {
    background-color: orange;
    padding: 10px 0;

    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    .unlisted-list {
        list-style: none;
    padding: 0;
    margin: 0;
    display: flex;
    gap: 10px;

    li {
        margin-right: 20px;
        
        a {
            text-decoration: none;
            color: black;
        }
    }
    }
    .logo {
        max-width: 150px;
    }
    .material-symbols-outlined {
    font-size: 24px;
}
}
</style>
<!-- /Style -->