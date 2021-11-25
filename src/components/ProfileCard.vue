<template>
  <div class="container-box-profile" v-bind="activeSliders"  @click="persone.i = activeSliders" :class="filterSlider(persone.i)">
                    <div class="box-profile">
                      <div class="box-profile-style">
                          <div class="descrition"><h5>{{persone.descrizione}} </h5></div>
                           
                            <div><p>{{persone.need}}</p></div>
                            <div class="box-profile-icon-jobs" >
                                <img :src="persone.img" alt="">

                                <div class="jobs-name">
                                    <h6>{{persone.name}}</h6>
                                    <p>{{persone.jobs}}</p>
                                </div>
                            </div>

                        </div>
                    </div>    
                </div>
</template>

<script>
export default {
    name:"ProfileCard",

    props:{
        persone:Object,
    },

    data(){
        return{
            activeSliders:0,
            }
    },

        methods:{

        filterSlider(i){
            if(i === 0){
                return "box-mandlay"
  
            }

            else if(i===1){
                return "box-mina"
            }

            else if(i===2){
                return "box-ludic"
            }
        }

    }

   

}
</script>

<style lang="scss" scoped>

.box-profile{
    width: 100%;
    height: 100%;
    background: rgb(255, 255, 255);
    box-shadow:5px 5px 15px 5px #000000;

    .box-profile-style{
        padding: 30px;
        display: flex;
    flex-direction: column;
    gap: 10px;

          p{    
               
                font-size: 14px;
            }

    .box-profile-icon-jobs{
            display: flex;

            .descrition{
                h5{
                    font-weight: bold;
                }
            }
            
            img{
                border-radius: 50%;
                width: 50px;
                height: 50px;
            }

          

            .jobs-name{

                h5{
                    font-size: 14px;
                }
                padding-left: 10px;
                p{
                    font-size: 10px;
                }
            }
        }
    }
    
}

.box-mina{
position: absolute;
    overflow: hidden;
    opacity: 0.5;
    bottom: 50px;
    width: 100%;
    border: 1px solid rgb(151, 151, 151);
}

.box-mandlay{
    z-index: 10;
    position: absolute;
    top: 40px;
    width: 100%;

}
.box-ludic{
position: absolute;
    overflow: hidden;
    opacity: 0.5;
    top: 100px;
    width: 100%;
    border: 1px solid rgb(151, 151, 151);}

</style>
