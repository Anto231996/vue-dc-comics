<template>
  <div class="current-series-content">
    <span>current series</span>
    <div id="current-series-items" class="wrapper">
      <MainCurrentSeriesProducts
        v-for="(element, index) in productSeries"
        :key="index"
        :productObject="element"
      />
    </div>
  </div>
</template>

<script>
import MainCurrentSeriesProducts from "./MainCurrentSeriesProducts.vue";

export default {
  name: "MainCurrentSeries",
  data: function () {
    return {
      productSeries: [
        {
          thumb:
            "https://static.dc.com/2023-09/BMSDM_v2_Cv12_01211_DIGITAL.jpg?w=160",
          price: "$19.99",
          series: "Action Comics",
          type: "comic book",
        },
        {
          thumb:
            "https://static.dc.com/2023-09/BMSDM_v2_Cv12_01211_DIGITAL.jpg?w=160",
          price: "$3.99",
          series: "American Vampire 1976",
          type: "comic book",
        },
        {
          thumb:
            "https://static.dc.com/2023-09/BMSDM_v2_Cv12_01211_DIGITAL.jpg?w=160",
          price: "$16.99",
          series: "Aquaman",
          type: "graphic novel",
        },
        {
          thumb:
            "https://static.dc.com/2023-09/BMSDM_v2_Cv12_01211_DIGITAL.jpg?w=160",
          price: "$2.99",
          series: "Batgirl",
          type: "comic book",
        },
        {
          thumb:
            "https://static.dc.com/2023-09/BMSDM_v2_Cv12_01211_DIGITAL.jpg?w=160",
          price: "$3.99",
          series: "Batman",
          type: "comic book",
        },
        {
          thumb:
            "https://static.dc.com/2023-09/BMSDM_v2_Cv12_01211_DIGITAL.jpg?w=160",
          price: "$2.99",
          series: "Batman Beyond",
          type: "comic book",
        },
        {
          thumb:
            "https://static.dc.com/2023-09/BMSDM_v2_Cv12_01211_DIGITAL.jpg?w=160",
          price: "$3.99",
          series: "Batman/Superman",
          type: "comic book",
        },
        {
          thumb:
            "https://static.dc.com/2023-09/BMSDM_v2_Cv12_01211_DIGITAL.jpg?w=160",
          price: "$4.99",
          series: "Batman/Superman Annual",
          type: "comic book",
        },
        {
          thumb:
            "https://static.dc.com/2023-09/BMSDM_v2_Cv12_01211_DIGITAL.jpg?w=160",
          price: "$5.99",
          series: "Batman: The Joker War Zone",
          type: "comic book",
        },
        {
          thumb:
            "https://static.dc.com/2023-09/BMSDM_v2_Cv12_01211_DIGITAL.jpg?w=160",
          price: "$6.99",
          series: "Batman: Three Jokers",
          type: "comic book",
        },
      ],
    };
  },

  components: {
    MainCurrentSeriesProducts,
  },
};
</script>

<style scoped lang="scss">
div.current-series-content {
  position: relative;
  padding: 80px 0;
  background-color: #212121;

  span {
    position: absolute;
    top: -20px;
    left: 200px;
    padding: 10px 20px;
    background-color: #137beb;
    color: white;
    text-transform: uppercase;
    font-weight: 600;
  }

  .wrapper {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 40px;
  }
}
</style>
