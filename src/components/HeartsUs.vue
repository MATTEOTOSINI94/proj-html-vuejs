<template>
   <div class="box-cont">
    <div class="container">
   
      <div class="row">
         <div class="col"></div>
          <div class="col-4 box-info " >
              <h6>EVRITHING IN MAXCOACH</h6>
              <h1>Why Do People?<span class="style-work">*Hearts*</span> Us</h1>
              <p>Seeking for verbals of our service quality? Find them here. Everything is transparent and straightforward for your sense of jusitifcation.</p>
                 <p><a href="#" class="style-free">View All </a></p>
          </div>
          <div class="col-5 box-view">
              <!-- prima carta profile -->
                <ProfileCard v-for="profilo,indice in profili " :key="indice" :persone="profilo" :inde="indice" @click="indiceActive=indice"></ProfileCard>
               
                
                
                <!-- fine prima carta profile -->
             
              
              <div class="lines-box">
                  
                  
              </div>
          </div>
          <div class="col"></div>
      </div>
    </div>
  </div>
 
</template>

<script>
import ProfileCard from "./ProfileCard.vue"

export default {
    name:"InfoQuality",

    components:{
        ProfileCard


    },


    data(){

        

        
        return{
            
            
            profili:[
                {
                    name:"Mandlay Pandor",
                    descrizione:"Professional team of specialists and passionate mentors at reach",
                    need:"I need to get a certification for English proficiency and MaxCoach is my best choice. Their tutors are smart and professional when dealing with students.",
                    jobs:"It specialists",
                    img: require("../assets/testimonial-avata-01.jpg"),
                    classe:"box-mandlay",
                    i:0
                },
                 {
                    name:"Mina Hollace",
                    descrizione:"High level of efficiency and scientific teaching methods",
                    need:"I am free to learn at my own pace, follow my own schedule and choose the subject I want to learn from the syllabus. Great study portal for people like me.",
                    jobs:"Freelancer",
                    img: require("../assets/testimonial-avata-02.jpg"),
                    classe:"box-mina",
                    i:1
                },
                 {
                    name:"Ludic Dubble",
                    descrizione:"The MaxCoach team works really hard to ensure high level of quality",
                    need:"I am happy with their arrangement of lessons and subjects. They reflect a scientific  investigation into effective methods to adopt.",
                    jobs:"/Private Tutor",
                    img: require("../assets/testimonial-avata-03.jpg"),
                    classe:"box-ludic",
                    i:2
                }
            ]
        }

        

    },

   



}
</script>

<style lang="scss" scoped>
    .box-cont{
  padding: 50px;
}

.img-style{
    width: 100%;
}

.box-view{
    position: relative;
}






.box-info{
    align-self: center;
    padding-left: 60px;
    padding-top: 35px;
    height: 100%;

    .style-work{
        color: #1fad95;
        font-weight: 100;
    }

    

    h6{
        font-size: 13px;
    }

    h1{
        font-style: bold;
    }
    p{
        font-size: 13px;
    }
}

.style-free{
    font-weight: bold;
    color: black;
}






</style>

