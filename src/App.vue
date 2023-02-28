<script>
import AppHeader from './components/AppHeader.vue';
import AppJumbotron from './components/AppJumbotron.vue';
import AppMain from './components/AppMain.vue';
import AppIcons from './components/AppIcons.vue';
import AppFooter from './components/AppFooter.vue';
import AppFollowUs from './components/AppFollowUs.vue';

import cardsList from './data/cardListArray.js';
import iconsList from './data/iconsListArray.js';
import headerLinks from './data/headerLinks.js';


export default {
  data(){
    return{
      cardsList,

      iconsList,

      headerLinks 
    }
  },
  components: {
    AppHeader,
    AppJumbotron,
    AppMain,
    AppIcons,
    AppFooter,
    AppFollowUs
  }
}
</script>

<template>
    <AppHeader :links="headerLinks"/>
    <AppJumbotron/>
    <AppMain :cards="cardsList"/>
    <AppIcons :icons="iconsList"/>
    <AppFooter/>
    <AppFollowUs/>
</template>

<style lang="scss">
@use "./scss/general.scss";

</style>
