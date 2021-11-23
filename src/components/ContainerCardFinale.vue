<template>
  <div class=" box-slider">
    <div class="container ">
      <div class="text-center">
    <h6>JOIN MAXCOACH AT BEST</h6>
    <h1>Latest Online <span class="style-work">Courses</span></h1>
    </div>

    <div class="slider">
      <div class="row slider-style ">
        <div class="col"></div>
        <Card :dati="el" v-for="el in cardComponent" :key="el.i"></Card>
        <div class="col"></div>
      </div>
    </div>
  </div>
  </div>
</template>

<script>

import Card from "./Card.vue"
export default {
    name:"ContainerCardFinal",

    components:{
        Card
    },

    props:{
        cardComponent:Array
    }

}
</script>

<style lang="scss" scoped>

   .box-slider{
    margin-top: 100px;
    background: rgb(204,204,204);
    background: linear-gradient(0deg, rgba(204,204,204,1) 3%, rgba(255,255,255,1) 38%);
    padding-bottom: 100px;
   


      .style-work{
        color: #1fad95;
        font-weight: 100;
    }
   

   h1{
     font-weight: bold;
     padding-bottom: 35px;
   }

   h6{
     font-size: 13px;
   }

   svg{
     width: 100%;
   }


   path{
     filter: invert(1);
   }

}
.slider-style{
 justify-content: center;
}

</style>

