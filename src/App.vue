<script>
import AppHeader from './components/AppHeader.vue';
import AppHero from './components/AppHero.vue';
import AppMain from './components/AppMain.vue';
import IconsList from './components/IconsList.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  components: {
    AppHeader,
    AppHero,
    AppMain,
    IconsList,
    AppFooter,
  }

}
</script>

<template>

  <AppHeader />
  <AppHero />
  <AppMain />
  <IconsList />
  <AppFooter />

</template>

<style land="scss"></style>
