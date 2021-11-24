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
        <Card v-for="el in  filterSlide()" :key="el.i" :dati="el" class="card-slide"></Card>
        <div class="col"></div>
      </div>
    </div>
  

    <div class="slider" v-if="corsi === true">
      <div class="row slider-style ">
        <div class="col"></div>
        <Card v-for="el,i in course.slice(3,6)" :key="i" :dati="el" class="box-all-card"></Card>
        <div class="col"></div>
      </div>
    </div>
    
  

    </div>
    <div class="text-center icon-btn-conteiner" v-if="corsi === false">
      <i class="fa" @click="activeSlider=0" :class="activeSlider===0 ? 'fa-circle' : 'fa-circle-thin'" aria-hidden="true"></i>
      <i class="fa" @click="activeSlider=1" :class="activeSlider===1 ? 'fa-circle' : 'fa-circle-thin'" aria-hidden="true"></i>
      <i class="fa" @click="activeSlider=2" :class="activeSlider===2 ? 'fa-circle' : 'fa-circle-thin'" aria-hidden="true"></i>
      <i class="fa" @click="activeSlider=3" :class="activeSlider===3 ? 'fa-circle' : 'fa-circle-thin'" aria-hidden="true"></i>
    </div>
    <div class="text-center view-all"><p>Control your Personal preference to notify about <br> appropriate courses <span class="style-view" v-if="corsi===false" @click="clickViewCourse()">View All Course</span> <span class="style-view" v-if="corsi===true" @click="corsi=false">Chiudi</span></p></div>
    
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
                },
            {   img:require("../assets/artist-blog-03-480x325.jpeg"),
                    price: "Artist",
                    type:"Brush Strokes Energize Trees in Paintings",
                    include: "May,15,2020",
                    maxStudend:"688 ",
                },
                {
                    img:require("../assets/artist-blog-01-480x325.jpg"),
                    price: "Artist",
                    type:"Pocket-Sized Notebooks Hold Miniature Painting",
                    include: "May,15,2020",
                    maxStudend:"769 ",
                },
                {
                    img:require("../assets/artist-blog-02-480x325.jpg"),
                    price: "Artist",
                    type:"Connection Between Self-Protraits and Identity",
                    include: "May,15,2020",
                    maxStudend:"397 ",
                }

            ],



            corsi:false,
            activeSlider:0

        }

      
    },

      methods:{
        filterSlide(){
          if (this.activeSlider===0) {
            return this.course.slice(0,3)
          }

          else if (this.activeSlider ===1) {
             return this.course.slice(1,4)
            
          }

          else if(this.activeSlider ===2){
            return this.course.slice(2,5)

          }

          else if(this.activeSlider ===3){
            return this.course.slice(3,6)
          }
          
        },

        clickViewCourse(){
          return this.corsi=true ,
               this.activeSlider= 0

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

.style-view{
  font-weight: bold;
 border-bottom: #1fad95 ;
 color: #1fad95;
 cursor: pointer;
}

.bg-circle{
  background-color: rgba(0, 0, 0, 0.562);
  border-radius: 100%;
}

.view-all{
margin-top: 20px;
}

.box-all-card{
  padding-top: 100px;
  padding-bottom: 50px;
}
.icon-btn-conteiner{

  i{
    padding: 10px 10px;
  }
}



</style>
 