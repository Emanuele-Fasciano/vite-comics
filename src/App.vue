<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppIcons from './components/AppIcons.vue';
import AppFooter from './components/AppFooter.vue';
import AppFollowUs from './components/AppFollowUs.vue';

export default {
  components: {
    AppHeader,
    AppMain,
    AppIcons,
    AppFooter,
    AppFollowUs
  }
}
</script>

<template>
    <AppHeader/>
    <AppMain/>
    <AppIcons/>
    <AppFooter/>
    <AppFollowUs/>
</template>

<style lang="scss">
@use "./scss/general.scss";

</style>
