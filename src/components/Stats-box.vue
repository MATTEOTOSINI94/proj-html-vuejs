<template>
  <div class="container pb-5">
      <div class="d-flex box-stats">
          <div class="text-center box-statistiche" v-for="stats in statsBar" :key="stats.i">
              <h3>{{stats.totalNum}}</h3>
              <p>{{stats.type}}</p>
          </div>
          

      </div>
  </div>
</template>

<script>
export default {
    name:"Statsbox",

    data(){
        return{
            statsBar:[
                {
                 type:"Enrollment",
                 totalNum:"129+"
                },

                {
                 type:"Finished Session",
                 totalNum:"80"
                },
                {
                 type:"Statisfaction Rate",
                 totalNum:"4%"
                }
            ]
        }
    }

}
</script>


<style lang="scss" scoped>
.box-stats{
    padding-top: 30px;
    justify-content: center;
    

    .box-statistiche{
        padding: 0 20px;

        h3{
            font-weight: bold;
            color: #1fad95;
        }
    }
}

.middle-box{
    padding: 0 70px;
}

</style>