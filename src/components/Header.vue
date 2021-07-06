<template>
  <div id="box">
    <div class="container">

    <header>

      <div class="logo">
        <img src="@/img/dc-logo.png" alt="logo-dc">
      </div>
      <nav>
        <ul>
          <li><a href="#"></a>Characters</li>
          <li><a href="#"></a>Comics</li>
          <li><a href="#"></a>Movies</li>
          <li><a href="#"></a>Tv</li>
          <li><a href="#"></a>Games</li>
          <li><a href="#"></a>Collectibles</li>
          <li><a href="#"></a>Videos</li>
          <li><a href="#"></a>Fans</li>
          <li><a href="#"></a>News</li>
          <li><a href="#"></a>Shop</li>
        </ul>
      </nav>
  
    </header>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header',
  props: {
    msg: String
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
          padding-bottom: 70px;
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
