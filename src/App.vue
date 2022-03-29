<template>
  <div id="app">

    <HeaderIndex />
    <MainCurrentSeries />
    <MainInfo />
    <FooterIndex />
    
  </div>
</template>

<script>
import HeaderIndex from './components/HeaderIndex.vue';
import MainCurrentSeries from './components/MainCurrentSeries.vue';
import MainInfo from './components/MainInfo.vue';
import FooterIndex from './components/FooterIndex.vue';

export default {
  name: 'App',
  components: {
    HeaderIndex, 
    MainCurrentSeries, 
    MainInfo,
    FooterIndex
  }
}
</script>

<style lang="scss">

@import "./assets/scss/style.scss";
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@100;200;300;400;500;600;700;800;900&display=swap');

div#app{
  min-width: 1800px;
}

</style>