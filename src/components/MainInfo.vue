<template>
  <div class="main-info">
    <div class="wrapper">
      <a href="#">
        <img src="../assets/img/buy-comics-digital-comics.png" alt="" />
        <h4>digital comics</h4>
      </a>

      <a href="#">
        <img src="../assets/img/buy-comics-merchandise.png" alt="" />
        <h4>dc merchandise</h4>
      </a>

      <a href="#">
        <img src="../assets/img/buy-comics-subscriptions.png" alt="" />
        <h4>subscription</h4>
      </a>

      <a href="#">
        <img src="../assets/img/buy-comics-shop-locator.png" alt="" style="width: 35px;" />
        <h4>comic shop locator</h4>
      </a>

      <a href="#">
        <img src="../assets/img/buy-dc-power-visa.svg" alt="" />
        <h4>dc power visa</h4>
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: "MainInfo",
};
</script>

<style scoped lang="scss">
div.main-info {
  height: 160px;
  background-color: #0880f8;

  div.wrapper {
    gap: 20px;
  }

  div.wrapper > a {
    display: flex;
    align-items: center;
  }

  div.wrapper > a img {
    height: 100%;
    width: 50px;
    margin-right: 1rem;
  }

  div.wrapper > a h4 {
    text-transform: uppercase;
    color: white;
    font-weight: normal;
  }
}
</style>
