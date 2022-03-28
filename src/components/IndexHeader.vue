<template>
  <div class="header-nav">
    <div>
      <img src="../assets/img/dc-logo.png" alt="main dc-logo">
    </div>
    <div>
      <nav>
        <ul>
          <li v-for="(element, index) in navBarLink" :key="index">
            <a href="#" :class="{active: element.current}">{{element.name}}</a>
          </li>
        </ul>
      </nav>
    </div>
  </div>
</template>

<script>
export default {
 name: 'IndexHeader',
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
    height: 15vh;
    width: 70%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin: 0 auto;

    li{
      display: inline;
      margin-left: 1.7rem;
      text-transform: uppercase;
      font-weight: 600;
      font-size: .8rem;

      a{
        text-decoration: none;
        color: #212121;
      }

      a.active, 
      a:hover{
        color: #137beb;
      }
    }
  }
</style>