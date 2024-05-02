<script>
export default {
    data() {
        return {

        }
    }
}
</script>

<template>

    <header class="header-nav">
        <div class="header-logo">
            <img class="img-logo" src="../assets/img/dc-logo.png" alt="Logo DC">
        </div>
        <div class="text">
            <ul>
                <li><a href="">CHARACTERS</a></li>
                <li><a href="">COMICS</a></li>
                <li><a href="">MOVIES</a></li>
                <li><a href="">TV</a></li>
                <li><a href="">GAMES</a></li>
                <li><a href="">COLLECTIBLES</a></li>
                <li><a href="">VIDEOS</a></li>
                <li><a href="">FANS</a></li>
                <li><a href="">NEWS</a></li>
                <li><a href="">SHOP</a></li>
            </ul>
        </div>
    </header>


</template>

<style scoped lang="scss">
@use "../style/partials/mixins" as *;
@use "../style/partials/variables" as *;


.header-nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px 40px;

    ul {
        @include flex(row, center, center);
        list-style-type: none;
        gap: 0.5rem;
        margin-top: 20px;

        a {
            padding: 9px 16px;
            text-decoration: none;
            color: black;
            display: inline-block;

            &:hover {
                color: $primary-color;
                // text-decoration: underline;
            }
        }
    }
}
</style>