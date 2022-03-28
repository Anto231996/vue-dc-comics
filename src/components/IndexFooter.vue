<template>
  <div class="footer">
    <div class="footer-top">
          <div class="footer-wrapper">
      <div id="">
        <!-- <img src="../assets/img/dc-logo-bg.png" alt="dc logo"> -->
      </div>

      <div class="footer-links">
        <div>
          <nav>
            <h4>dc comics</h4>
            <ul>
              <li v-for="(element, index) in dccomicsFooterLink" :key="index">
                <a href="#">{{element.name}}</a>
              </li>
            </ul>
          </nav>
        </div>
        <div>
          <nav>
            <h4>dc</h4>
            <ul>
              <li v-for="(element, index) in dcFooterLink" :key="index">
                <a href="#">{{element.name}}</a>
              </li>
            </ul>
          </nav>
        </div>
        <div>
          <nav>
            <h4>sites</h4>
            <ul>
              <li v-for="(element, index) in sitesFooterLink" :key="index">
                <a href="#">{{element.name}}</a>
              </li>
            </ul>
          </nav>
        </div>
        <div>
          <nav>
            <h4>shop</h4>
            <ul>
              <li v-for="(element, index) in shopFooterLink" :key="index">
                <a href="#">{{element.name}}</a>
              </li>
            </ul>
          </nav>
        </div>
      </div>
    </div>
    </div>


    <div class="footer-bottom">

    </div>

  </div>
</template>

<script>
export default {
 name: 'IndexFooter',
 data: function() {
   return {
     dccomicsFooterLink:[
      {
        name:"Characters",
        url: "#",
      },

      {
        name:"Comics",
        url: "#",
      },

      {
        name:"Movies",
        url: "#",
      },

      {
        name:"Tv",
        url: "#",
      },

      {
        name:"Games",
        url: "#",
      },

      {
        name:"Video",
        url: "#",
      },

      {
        name:"News",
        url: "#",
      }
     ],

      dcFooterLink:[
      {
        name:"Terms Of Use",
        url: "#",
      },

      {
        name:"Privacy policy (New)",
        url: "#",
      },

      {
        name:"Ad Choices",
        url: "#",
      },

      {
        name:"Advertising",
        url: "#",
      },

      {
        name:"Jobs",
        url: "#",
      },

      {
        name:"Subscriptions",
        url: "#",
      },

      {
        name:"Talent Workshops",
        url: "#",
      },

      {
        name:"CPSC Certificates",
        url: "#",
      },

      {
        name:"Rating",
        url: "#",
      },

      {
        name:"Shop Help",
        url: "#",
      },

      {
        name:"Contact Us",
        url: "#",
      }
     ],

      sitesFooterLink:[
      {
        name:"DC",
        url: "#",
      },

      {
        name:"MAD Magazine",
        url: "#",
      },

      {
        name:"DC Kids",
        url: "#",
      },

      {
        name:"DC Universe",
        url: "#",
      },

      {
        name:"DC Power Visa",
        url: "#",
      }
     ],

      shopFooterLink:[
      {
        name:"Shop DC",
        url: "#",
      },

      {
        name:"Shop DC Collectibles",
        url: "#",
      }
     ]
   }
 },
}
</script>

<style scoped lang="scss">

  h4{
    color: white;
    text-transform: uppercase;
    margin-bottom: 1rem;
  }

  div.footer-top{
    height: 45vh;
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;
  }

  div.footer-wrapper{
    width: 70%;
    height: 100%;
    margin: 0 auto;
    display: flex;
    align-items: center;

    div.footer-links{
      display: flex;

      li{
        list-style: none;
        font-size: .8rem;
        margin-bottom: .3rem;

        a{
          text-decoration: none;
          color: gray;
        }

      }

    }

    div.footer-links > div{
      margin-right: 50px;
    }
  }

  div.footer-bottom{
    height: 10vh;
    background-color: #333333;
  }

</style>