<template>
  <div class="main-info">
    <div class="wrapper">
      <div>
        <a href="#">
          <img src="../assets/img/buy-comics-digital-comics.png" alt="">
          <h4>digital comics</h4>
        </a>
      </div>
      <div>
        <a href="#">
          <img src="../assets/img/buy-comics-merchandise.png" alt="">
          <h4>dc merchandise</h4>
        </a>
      </div>
      <div>
        <a href="#">
          <img src="../assets/img/buy-comics-subscriptions.png" alt="">
          <h4>subscription</h4>
        </a>
      </div>
      <div>
        <a href="#">
          <img src="../assets/img/buy-comics-shop-locator.png" alt="">
          <h4>comic shop locator</h4>
        </a>
      </div>
      <div>
        <a href="#">
          <img src="../assets/img/buy-dc-power-visa.svg" alt="">
          <h4>dc power visa</h4>
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
 name: 'IndexMainInfo',
}
</script>

<style scoped lang="scss">
  div.main-info{
    height: 15vh;
    background-color: #0880f8;

    div.wrapper{
      width: 70%;
      height: 100%;
      margin: 0 auto;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    div.wrapper > div a{
      display: flex;
      align-items: center;
      justify-content: space-evenly;
    }

    div.wrapper > div a img{
      width: 50px;
      margin-right: 1rem;
    }

    div.wrapper > div a h4{
      text-transform: uppercase;
      color: white;
      font-weight: normal;
    }
  }
</style>