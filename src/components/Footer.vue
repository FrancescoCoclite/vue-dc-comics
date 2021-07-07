<template>
  <div>
      <footer>
        <div class="container">
            <div class="lista">
                <h2>Dc comics</h2>
            <ul>
                <li><a href="#"></a>Testo di prova</li>
                <li><a href="#"></a>Testo di prova</li>
                <li><a href="#"></a>Testo di prova</li>
            </ul>
            </div>
            <div class="lista">
                <h2>Dc</h2>
            <ul>
                <li><a href="#"></a>Testo di prova</li>
                <li><a href="#"></a>Testo di prova</li>
                <li><a href="#"></a>Testo di prova</li>
            </ul>
            </div>
            <div class="lista">
                <h2>Sites</h2>
            <ul>
                <li><a href="#"></a>Testo di prova</li>
                <li><a href="#"></a>Testo di prova</li>
                <li><a href="#"></a>Testo di prova</li>
            </ul>
            </div>
        </div>
      </footer>
      <div class="bottom">
        <div class="container">
            <div class="under-footer">
                <button>Sign-up now!</button>
                <div class="social">
                    <span><strong>Follow Us</strong></span>
                    <img src="@/img/footer-facebook.png" alt="">
                    <img src="@/img/footer-periscope.png" alt="">
                    <img src="@/img/footer-pinterest.png" alt="">
                    <img src="@/img/footer-twitter.png" alt="">
                    <img src="@/img/footer-youtube.png" alt="">
                </div>
            </div> 
        </div>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped lang="scss">
footer{
    background-image: url(../img/footer-bg.jpg);
    height: 200px;
}
.container{
  width: 1080px;
  margin: auto;
}
.lista{
    display: inline-block;
    margin-right: 20px;
    margin-top: 30px;
    color:white;
    li{
        color: lightgray;
    }
}
.bottom{
    background-color: #1C1C1C;
    .under-footer{
        padding: 40px; 
        display: flex;
        justify-content: space-between;
        img{
            margin-right: 20px;
        }
        span{
            color: #0282F9;
            vertical-align: super;
            margin-right: 10px;
            font-size: 20px;
            text-transform: uppercase;
        }
    }
}
button{
    border: 3px solid #0282F9;
    padding: 10px;
    background-color: #1C1C1C;
} 
h2{
    text-transform: uppercase;
    margin-bottom: 20px;
}

</style>