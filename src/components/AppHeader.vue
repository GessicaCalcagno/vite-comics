<script>
export default {
    data() {
        return {
            menu: [
                {
                    title: "CHARACTERS",
                    isActive: true,
                },
                {
                    title: "COMICS",
                    isActive: false,
                },
                {
                    title: "MOVIES",
                    isActive: false,
                },
                {
                    title: "TV",
                    isActive: false,
                },
                {
                    title: "GAMES",
                    isActive: false,
                },
                {
                    title: "COLLECTIBLES",
                    isActive: false,
                },
                {
                    title: "VIDEOS",
                    isActive: false,
                },
                {
                    title: "FANS",
                    isActive: false,
                },
                {
                    title: "NEWS",
                    isActive: false,
                },
                {
                    title: "SHOP",
                    isActive: false,
                },
            ]



        }
    }
}
</script>

<template>


    <header>
        
            <div class="header-nav">
                <div class="header-logo">
                    <img class="img-logo" src="../assets/img/dc-logo.png" alt="Logo DC">
                </div>
                <div>
                    <ul class="navigation">
                        <li v-for="item in menu">
                            <a href="" :class="{ 'active': item.isActive }">{{ item.title }}</a>
                        </li>
                    </ul>
                </div>
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
    padding: 10px 20px;
    width: 80%;
    margin: 0 auto;

    ul {
        @include flex(row, center, center);
        list-style-type: none;
        gap: 1rem;

        a {
            font-weight: 540;
            text-decoration: none;
            color: black;
            display: inline-block;
            padding-bottom: 20px;

            &:hover {
                color: $primary-color;
                border-bottom: 4px solid;
                // text-decoration: underline;
            }

            // &.active {
            //     background-color: $primary-color;
            // }
        }
    }
}


</style>