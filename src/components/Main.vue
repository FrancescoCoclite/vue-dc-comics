<template>
  <main>
          <div class="jumbotron"></div>
      <section class="nero">
      <div class="container">
          <div class="contenuto">
              <!-- <button> current series</button> -->
              <div class="riga-top">
                <div class="immagini"></div>
                <div class="immagini"></div>
                <div class="immagini"></div>
                <div class="immagini"></div>
                <div class="immagini"></div>
                <div class="immagini"></div>
                <div class="immagini"></div>
                <div class="immagini"></div>
                <div class="immagini"></div>
                <div class="immagini"></div>
                <div class="immagini"></div>
                <div class="immagini"></div>
              </div>
             
              
              
          </div>
      </div>

      </section>

      <section class="blu">
      <div class="container">
          <div class="prodotti">
              <img src="@/img/prodotto1.png" alt="">
              <div class="descrizione-prod">digital comics</div>
              <img src="@/img/prodotto2.png" alt="">
              <div class="descrizione-prod">dc merchandise</div>
              <img src="@/img/prodotto4.png" alt="">
              <div class="descrizione-prod">subscription</div>
              <img src="@/img/prodotto3.png" alt="">
              <div class="descrizione-prod">comics shop locator</div>
              <img class="img_svg" src="@/img/buy-dc-power-visa.svg" alt="">
              <div class="descrizione-prod">dc power visa</div>
          </div>
      </div>
          
      </section>
  </main>
</template>

<script>
    import Array from '@/data/Array.vue';
export default {
    props :{
        titolo : String
    },
    data(){
        return{
            films: Array
        }
    }

}
</script>

<style scoped lang="scss">
main{
    margin-top: 60px;
    
}
.nero{
    background-color: #1C1C1C;
    width: 100%;
    padding: 40px;
}
.blu{
    background-color: #0282F9;
    width: 100%;
    padding: 60px;
}
.jumbotron{
    background-image: url(../img/jumbotron.jpg);
    height: 350px;
    background-size: cover;
}
.container{
  width: 1080px;
  margin: auto;
    .contenuto{
        display: flex;
        font-size: 25px;
        color: white;
        position: relative;
        .riga-top{
            width: 100%;
            display: flex;
            flex-wrap: wrap;
        }
        .immagini{
            height: 250px;
            width: calc(100% / 6 - 20px) ;
            background-color: red;
            margin-right: 20px;
            margin-top:30px;
        }   
        button{
            background-color:#0282F9;
            padding: 7px;
            position:absolute;
            bottom: 26px;
            font-size: 20px;
        }
        
    }
    .prodotti{
        display: flex;
        font-size: 20px;
        color: white;
        margin-right: 40px;
        justify-content: space-between;
    }
    img{
        height: 100px;
        width: 80px;
    }
    .descrizione-prod{
        display: flex;
       align-items: center;
       margin-right: 60px;
       text-transform: uppercase;
    }
}



</style>