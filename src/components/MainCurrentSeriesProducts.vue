<template>
  <div class="item" @click="sendAlert(productObject.price)">
      <img :src="productObject.thumb" :alt="productObject.series">
      <h4>{{ productObject.series }}</h4>
  </div>

</template>

<script>
export default {
  name: 'MainCurrentSeriesProducts',
  props: ['productObject'],
  methods:{
    sendAlert(price){
      alert("IL COSTO E' DI" + " " + price)
    }
  }
}
</script>

<style scoped lang="scss">
  .item{
    width: 200px;
    height: 200px;

    img{
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: top;
    }

    h4{
      font-weight: normal;
      color: white;
    }
  }
</style>