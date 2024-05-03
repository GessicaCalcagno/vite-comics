<script>

export default {



}
</script>

<template>
    <section class="hero">

        <div>
            <span class="j-button"><a href="">CURRENT SERIES</a></span>
        </div>
    </section>



</template>

<style scoped land="scss">
/* @use "../style/partials/variables" as *; NON LO PRENDE*/

.hero {
    background-image: url("../assets/img/jumbotron.jpg");
    min-height: 300px;
    background-size: cover;
    width: 100%;
    position: relative;
}

.j-button {
    background-color: #0282F9;
    padding: 15px;
    position: absolute;
    bottom: -1.5rem;
    left: 150px;
    box-shadow: 5px 5px 10px rgba(2, 2, 2, 0.922);
    /* Aggiunge un'ombra allo span */

    a {
        text-decoration: none;
        color: white;
        font-weight: bold;
    }

}
</style>