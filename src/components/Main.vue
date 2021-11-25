<template>
<main>
  <HeroMain></HeroMain>
  <Maxcoachbox></Maxcoachbox>
  <Statsbox></Statsbox>
  <SkillBox></SkillBox>
  <CardContainer></CardContainer>
  <InfoQuality></InfoQuality>
  <TrasformYou></TrasformYou>
  <ContainerCardFinal :cardComponent="cardBlog"></ContainerCardFinal>
  <NewsLetter></NewsLetter>
  


  

  

 


</main>

</template>

<script>

import HeroMain from "./Heromain.vue"
import Maxcoachbox from "./Maxcoachbox.vue"
import Statsbox from "./Stats-box.vue"
import SkillBox from "./Upgradeskills.vue"
import CardContainer from "./Cardcontainer.vue"
import InfoQuality from "./HeartsUs.vue"
import TrasformYou from "./Motivatetem.vue"
import ContainerCardFinal from "./ContainerCardFinale.vue"
import NewsLetter from "./NewsLetter.vue"


export default {
    name:"Main",

    components:{
        HeroMain,
        Maxcoachbox,
        Statsbox,
        SkillBox,
        CardContainer,
        InfoQuality,
        TrasformYou,
        ContainerCardFinal,
        NewsLetter
        
        
    },

    data(){
      return{
        cardBlog:[
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
          
        ]
      }
    }

}
</script>

<style lang="scss" scoped>




</style>

