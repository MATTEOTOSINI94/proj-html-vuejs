<template>
  <div class="container box-slider">
    <div class="text-center">
    <h6>JOIN MAXCOACH AT BEST</h6>
    <h1>Latest Online <span>Courses</span></h1>
    </div>

    <div class="slider">
      <div class="row slider-style ">
        <div class="col"></div>
        <Card v-for="el in course" :key="el.i" :dati="el"></Card>
        <div class="col"></div>
      </div>
    </div>
    <div class="btn-slider"></div>
    <div class="text-center pt-5"><p>Control your Personal preference to notify about <br> appropriate courses <span>View All Course</span></p></div>

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
                {   img:require("../assets/stock-full-hd-03-480x298.jpg"),
                    type: "Learing to write as a professional Author",
                    price:"40$",
                    include: "20 Lesson",
                    maxStudend:"50 student",
                },
                {
                    img:require("../assets/stock-full-hd-03-480x298.jpg"),
                    type: "Costumer-centric-info-tech Strategies",
                    price:"0.00$",
                    include: "24 Lesson",
                    maxStudend:"769 student",
                },
                {
                    img:require("../assets/stock-full-hd-04-480x298.jpg"),
                    type: "Open Programming Courses for Pyton",
                    price:"19.00$",
                    include: "17 Lesson",
                    maxStudend:"62 student",
                }

            ]

        }
    }


}
</script>

<style>
    .box-slider{
  padding-top: 70px;
}
.slider-style{
 justify-content: center;
}
</style>