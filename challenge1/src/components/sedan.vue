<template>
  <div class="hello">
   <div class="card" style="">
  <div class="card-body">
    <!-- <h5 class="card-title">Card title</h5> -->
    <!-- <h6 class="card-subtitle mb-2 text-muted">Card subtitle</h6> -->
    <!-- <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
    <a href="#" class="card-link">Card link</a>
    <a href="#" class="card-link">Another link</a> -->

      <div class="row " style="border-radius:20px; padding: 5% 0; width: 65%; color: whitesmoke; font-family: 'Lexend Deca', sans-serif;">
      <div class="col-md-4 col-lg-4 p-3" style="background-color: orange; height: 100%;">
        <img src="../assets/icon-sedans.svg" alt="">
        <p>SEDANS </p>
       
        <div class="card-text">
          
          Choose a sedan for its affordability and excellent fuel economy. Ideal for cruising in the city or on your next road trip. 
        </div>
         <button type="button" class="btn btn-light" style="color:orange;">Learn More</button>
      </div>

      <div class="col-md-4 col-lg-4 p-3" style="background-color: darkcyan;">
         <img src="../assets/icon-suvs.svg" alt="">
        <p>SUVs </p>
        <div class="card-text">
           Take an SUV for its spacious interior, power, and versatility. Perfect for your next family vacation and off-road adventures. 
        </div>
        <button type="button" class="btn btn-light" style="color:darkcyan;">Learn More</button>
      </div>

      <div class="col-md-4 col-lg-4 p-3 " style="background-color: #002E2E;">
         <img src="../assets/icon-luxury.svg" alt=""> 
        <p>Luxury </p>
        <div class="card-text">
           Cruise in the best car brands without the bloated prices. Enjoy the enhanced comfort of a luxury rental and arrive in style.
        </div>
 <button type="button" class="btn btn-light" style="color:#002E2E;">Learn More</button>
      </div>
    </div>

  </div>
</div>
  </div>
</template>

<script>

export default {
  name: 'sedan',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss" > 
.card{
  margin: 40px;height: 70vh; border: none;box-shadow: rgba(0, 0, 0, 0.1) 0px 4px 12px;
}
.row{
  margin: 20% 0;
  text-align: left;
   margin: 0 20% 0% ;
  .col-md-4.col-lg-4{
    padding-left: 60px;
    img{
      width: 40px;
      padding-bottom: 40px;
    }
     display: flex;
    flex-direction:column;
    button{
        border-radius: 50px;
        margin-top: 40px;
        width: 50%;
        font-size: 11px;
        font-weight: 700;
      }
    .card-text{
      font-size: 15px;
      
      padding-bottom: 40px;

  
    }
    p{
      padding-bottom: 20px;
    }
  }

}
@media screen and (max-width:722px){
  .row{
    padding: 0  ;
  }
  .card{
    height: auto;
  }
  .col-md-4.col-lg-4{
    width: 100%;
    padding: 0 36px;
  }
  .card-body{
    padding: 0;
  }
}
</style>
