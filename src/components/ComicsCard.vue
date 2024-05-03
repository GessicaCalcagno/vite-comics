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
    <h4>{{ cardTitle }}</h4>
  </div>
</template>

<style scoped lang="scss">
.card {
  padding: 1rem;
  background-color: white;

  img {
    max-width: 100%;
  }
}
</style>