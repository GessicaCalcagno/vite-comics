<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import IconsList from './components/IconsList.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  components: {
    AppHeader,
    AppMain,
    IconsList,
    AppFooter,
  }

}
</script>

<template>

  <AppHeader />
  <AppMain />
  <IconsList />
  <AppFooter />

</template>

<style land="scss"></style>
