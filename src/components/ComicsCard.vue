<script>
export default {
  props: {
    cardImage: String,
    cardTitle: String,
  }

};
</script>

<template>
  <div class="card">
    <img :src="cardImage" :alt="cardTitle">
    <h5>{{ cardTitle }}</h5>
  </div>
</template>

<style scoped lang="scss">
.card {
  padding: 1rem 0.5rem 1rem 0;
  // background-color: white;

  img {
    // max-width: 100%;

    height: 200px;


  }
}
</style>