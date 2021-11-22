<template>
   <div class="container">
    <div class="box-Max-Coach">
      <div class="row">
         <div class="col"></div>
          <div class="col-5 box-info " >
              <h6>EVRITHING IN MAXCOACH</h6>
              <h1>Learn About our <span class="style-work">Work Colture</span> at MaxCoach</h1>
              <p>Spend Time to Visit Our WebSite or Head Office and discover our current courses enrollement procedure and reagistration deadLine. 
                 We're opening new classes every beginnin of each Month</p>
                 <p>Have question? <a href="#" class="style-free">Free Guide</a></p>
          </div>
          <div class="col-4 box-view">
              <div>
              <img src="../assets/stock-full-hd-10-ohki1ayywq3cqutettrncduujpoaorifqu4relt2ts.jpg" alt="">
              </div>
              <div class="img-secondo-piano">
                  <img src="../assets/about-us-01-ohkia3qg98rq9vg3s0mn2hkflr1migdqdw370qnegc.jpg" alt="">
                 
              </div>
              <div class="lines-box">
                  <img class="shape-line" src="../assets/maxcoach-shape-02.png" alt="">
                   <img class="shape-lines" src="../assets/maxcoach-shape-07.png" alt="">
                  
              </div>
          </div>
          <div class="col"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
    name:"Maxcoachbox"

}
</script>

<style lang="scss" scoped>
.container{
    padding-top: 100px;
}

.box-info{
    padding-right: 60px;
    height: 100%;

    .style-work{
        color: #1fad95;
        font-weight: 100;
    }

    .style-free{
        color: #1fad95;
        border: 0;
        border-bottom: 0.3px dotted grey;
        
    }

    h6{
        font-size: 13px;
    }

    h1{
        font-style: bold;
    }
    p{
        font-size: 10px;
    }
}

.box-view{
    position: relative;
    height: 100%;
    img{ 
        width: 100%;
    }
   
   .img-secondo-piano{
     
       img{
        width: 27%;
        position: absolute;
        top: -55px;
        right: 0;
       }
   }


   .lines-box{
      
      

        .shape-line{
            position: absolute;
            bottom: -45px;
            right: 30px;
            width: 20%;
        }

       .shape-lines{
             width: 30%;
            position: absolute;
            top: -55px;
            right: 25px;
            z-index: -1;
       }
   }
}

</style>
