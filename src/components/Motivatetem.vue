<template>
   <div class="box-cont">
    <div class="container">
   
      <div class="row">
         <div class="col"></div>
         <div class="col-5 box-view">
              <div>
              <img class="img-style" src="../assets/home-3-team-image.png" alt="">
              </div>
              
              <div class="lines-box">
                  
                  <img class="style-line" src="../assets/maxcoach-shape-01.png" alt="">
                   <img class="shape-line" src="../assets/maxcoach-shape-05.png" alt="">
                  <img class="shape-lines" src="../assets/maxcoach-shape-07.png" alt="">
              </div>
          </div>
          <div class="col-4 box-info " >
              <h6>EVRITHING IN MAXCOACH</h6>
              <h1>We’re Here To <span class="style-work">Transform</span>You!</h1>
              <p>As learners, people can enjoy great companionship from MaxCoach mentors and educators. We can help you develop and grow at your best.</p>
                 <p><a href="#" class="style-free">View All </a></p>

                 <div class="btn-box">  
                <button class="btn-style">Download</button>
              </div>
          </div>
        
          <div class="col"></div>
      </div>
    </div>
  </div>
  
  

 
</template>

<script>
export default {

    name:"TrasformYou"

}
</script>

<style lang="scss" scoped>
    .box-cont{
  padding: 50px;
}

.box-view{
  position: relative;
  height: 100%;
}
.lines-box{

  .style-line{
    position: absolute;
    left: -100px;
    width: 20%;
  }

  .shape-line{
   position: absolute;
    width: 20%;
    top: 60px;
    left: -20px;
  }

  .shape-lines{
  
    position: absolute;
    width: 20%;
    right: 115px;
    bottom: -40px;
    z-index: -1;

  }
}


.img-style{
  width: 100%;
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
        font-size: 10px;
    }

     .btn-box{
      padding-top: 10px;
      .btn-style{
        border: 0;
      padding: 7px 30px;
      border-radius: 8px;
      color: white;
      background: linear-gradient(to left, #1fad95 50%, rgb(228, 228, 228) 50%) right;
      background-size: 200%;
      transition: .5s ease-out;
      }

      .btn-style:hover{
        background-position: left;
        color: black;
      }
    }
}
</style>