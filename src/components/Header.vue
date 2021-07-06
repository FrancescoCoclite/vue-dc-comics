<template>
  <div id="box">
    <div class="container">

    <header>

      <div class="logo">
        <img src="@/img/dc-logo.png" alt="logo-dc">
      </div>
      <nav>
        <ul>
          <li v-for="(link,index) in links" :key="index"><a href="#"></a>{{link.text}}</li>

        </ul>
      </nav>
  
    </header>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header',
  // props: {
  //   msg: String
  // },
  data() {
    return {
      links: [
      {
        text : 'Characters',
        url : '#',
        status : false,
      }, 
      {
        text : 'Comics',
        url : '#',
        status : false,
      },
      {
        text : 'Movies',
        url : '#',
        status : false,
      }, 
      {
        text : 'Tv',
        url : '#',
        status : false,
      }, 
      {
        text : 'Games',
        url : '#',
        status : false,
      }, 
      {
        text : 'Collectibles',
        url : '#',
        status : false,
      },
      {
        text : 'Videos',
        url : '#',
        status : false,
      },
      {
        text : 'Fans',
        url : '#',
        status : false,
      },
      {
        text : 'News',
        url : '#',
        status : false,
      }, 
      {
        text : 'Shop',
        url : '#',
        status : false,
      }, 
      ]

    }

  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container{
  width: 1080px;
  margin: auto;
}

header{
  height: 70px;
  &::after{
    display: table;
    content: '';
    clear: both;
  }
  .logo{
   float: left; 
  }
  nav{
    float: right;
    ul {
      list-style-type: none;
      padding: 0;
      
      li {
        
        display: inline-block;
        margin: 0 10px;
        &:hover{
          color: #3682F9;
          padding-bottom: 95px;
          border-bottom: 3px solid #3682F9;
        }
      }
      a{
        color: black;
      }
    }
  }
}

</style>
