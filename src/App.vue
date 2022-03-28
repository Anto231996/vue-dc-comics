<template>
  <div id="app">

    <!-- HEADER -->
    <IndexHeader />
    <!-- MAIN -->
    <IndexMain />
    <!-- INFO -->
    <IndexMainInfo />
    <!-- FOOTER -->
    <IndexFooter />
    
  </div>
</template>

<script>
import IndexHeader from './components/IndexHeader.vue';
import IndexMain from './components/IndexMain.vue';
import IndexMainInfo from './components/IndexMainInfo.vue';
import IndexFooter from './components/IndexFooter.vue';

export default {
  name: 'App',
  components: {
    IndexHeader, 
    IndexMain, 
    IndexFooter,
    IndexMainInfo
  }
}
</script>

<style lang="scss">

@import "./assets/scss/style.scss";
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@100;200;300;400;500;600;700;800;900&display=swap');

</style>