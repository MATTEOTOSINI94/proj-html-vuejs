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
        <Card v-for="el in course" :key="el.i" :dati="el"></Card>
        <div class="col"></div>
      </div>
    </div>
    <div class="slider" v-if="corsi === true">
      <div class="row slider-style ">
        <div class="col"></div>
        <Card v-for="el in course" :key="el.i" :dati="el"></Card>
        <div class="col"></div>
      </div>
    </div>
    <div class="btn-slider"></div>
  
    <div class="text-center pt-5"><p>Control your Personal preference to notify about <br> appropriate courses <span @click="corsi= true">View All Course</span></p></div>
  

    </div>
    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100" preserveAspectRatio="none" height="100">
	<path class="elementor-shape-fill" d="M 0 0 L0 100 L100 100 L100 0 Q 50 200 0 0"></path>
</svg>
  </div>
</template>

<script>
import Card from './Card.vue'


export default {
  
    name:"CardContainer",
    components:{
        Card
    },

    data(){

        return{
            course:[
                {   img:require("../assets/course-02-480x298.jpg"),
                    type: "Learing to write as a professional Author",
                    price:"40",
                    include: "20 Lesson",
                    maxStudend:"50 student",
                    coin:"00"
                },
                {
                    img:require("../assets/stock-full-hd-03-480x298.jpg"),
                    type: "Costumer-centric-info-tech Strategies",
                    price:"0",
                    include: "24 Lesson",
                    maxStudend:"769 student",
                    coin:"00"
                },
                {
                    img:require("../assets/stock-full-hd-04-480x298.jpg"),
                    type: "Open Programming Courses for Pyton",
                    price:"19",
                    include: "17 Lesson",
                    maxStudend:"62 student",
                    coin:"00"
                }

            ],

            corsi:false

        }
    }


}
</script>

<style lang="scss" scoped>
   .box-slider{
  margin-top: 100px;
  background: rgb(204,204,204);
  background: linear-gradient(0deg, rgba(204,204,204,1) 3%, rgba(255,255,255,1) 38%);
   border-radius: 100px / 50px;


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
 