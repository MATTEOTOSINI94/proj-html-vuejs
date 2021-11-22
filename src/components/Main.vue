<template>
<main>
  <HeroMain></HeroMain>
  <Maxcoachbox></Maxcoachbox>
  <Statsbox></Statsbox>
  <SkillBox></SkillBox>
  <CardContainer></CardContainer>
  
 
  

 


</main>

</template>

<script>

import HeroMain from "./Heromain.vue"
import Maxcoachbox from "./Maxcoachbox.vue"
import Statsbox from "./Stats-box.vue"
import SkillBox from "./Upgradeskills.vue"
import CardContainer from "./Cardcontainer.vue"
export default {
    name:"Main",

    components:{
        HeroMain,
        Maxcoachbox,
        Statsbox,
        SkillBox,
        CardContainer
        
        
    }

    

}
</script>

<style lang="scss" scoped>









</style>

