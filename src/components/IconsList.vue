<script>
export default {
    data() {
        return {
            images: [
                {
                    image: "buy-comics-digital-comics.png",
                    title: "DIGITAL COMISCS",
                },
                {
                    image: "buy-comics-merchandise.png",
                    title: "DC MERCHANDISE",
                },
                {
                    image: "buy-comics-subscriptions.png",
                    title: "SUBSCRIPTION",
                },
                {
                    image: "buy-comics-shop-locator.png",
                    title: "COMIC SHOP LOCATOR",
                },
                {
                    image: "buy-dc-power-visa.svg",
                    title: "DC POWER VISA",
                },
            ],
        };
    },

    methods: {
        getImageUrl(imageName) {
            return new URL(`../assets/img/${imageName}`, import.meta.url).href;
        }
    }
};

</script>

<template>
    <section>
        <div class="container">
            <ul>
                <li v-for="curImage in images">
                    <img :src="getImageUrl(curImage.image)" alt="">
                    <h5>{{ curImage.title }}</h5>
                </li>
            </ul>

        </div>

    </section>

</template>

<style scoped lang="scss">
@use "../style/partials/variables" as *;
// @use "../style/partials/mixins" as *; --> non lo prendeva

section {
    background-color: $primary-color;
    padding: 3rem 0;
    color: white;
    min-height: 100px;

    .container {
        width: 70%;
        margin: 0 auto;

        ul {
            list-style: none;
            display: flex;
            justify-content: space-evenly;

            li {
                display: flex;
                align-items: center;
                font-size: small;

                img {
                    height: 40px;
                    padding-right: 18px;
                    padding-left: 12px;
                }
            }


        }
    }


}
</style>