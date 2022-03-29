<template>
  <div class="header">
    <div class="header-nav">
      <div class="wrapper">
        <img src="../assets/img/dc-logo.png" alt="main dc-logo">
        <nav>
          <ul>
            <li v-for="(element, index) in navBarLink" :key="index">
              <a href="#" :class="{active: element.current}">{{element.name}}</a>
            </li>
          </ul>
        </nav>
      </div>
    </div>
    <div id="jumbotron"></div>
  </div>
</template>

<script>
export default {
  name: 'HeaderIndex',
  data: function() {
    return {
      navBarLink:[
      {
        name:"characters",
        url: "#",
        current: false
      },

      {
        name:"comics",
        url: "#",
        current: true
      },

      {
        name:"movies",
        url: "#",
        current: false
      },

      {
        name:"tv",
        url: "#",
        current: false
      },

      {
        name:"games",
        url: "#",
        current: false
      },

      {
        name:"collectibles",
        url: "#",
        current: false
      },

      {
        name:"videos",
        url: "#",
        current: false
      },

      {
        name:"fans",
        url: "#",
        current: false
      },

      {
        name:"news",
        url: "#",
        current: false
      },

      {
        name:"shop",
        url: "#",
        current: false
      }

    ]
  }
},
}
</script>

<style scoped lang="scss">
  div.header-nav{
    height: 140px;

    li{
      display: inline;
      margin-left: 1.7rem;
      font-size: .8rem;
      font-weight: 600;
      text-transform: uppercase;

      a{
        color: #212121;
      }

      a.active, 
      a:hover{
        color: #137beb;
      }
    }
  }

  div#jumbotron{
    height: 400px;
    background-image: url(../assets/img/jumbotron.jpg);

    img{
      height: 100%;
      width: 100%;
    }
  }
</style>