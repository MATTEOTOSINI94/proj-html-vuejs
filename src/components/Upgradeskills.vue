<template>
   <div class="container">
    <div class="box-Max-Coach">
      <div class="row">
          <div class="col"></div>
           <div class="col-5 box-play">
              <div>
              <img src="../assets/stock-full-hd-11-670x450.jpg" alt="">
             
              </div>
              
              
              <div class="lines-box">
                 <img class="youtube-btn" src="../assets/icon-youtube-play.png" alt="">
                 <img class="shape-line" src="../assets/maxcoach-shape-05.png" alt="">
                  <img class="shape-lines" src="../assets/maxcoach-shape-07.png" alt="">
                  
              </div>
          </div>
          


          <div class="col-4 box-info">
              <h6>HOW WE WORK</h6>
              <h1>Upgrade Your Skills <span class="style-work">Upgrade Your Life</span> </h1>
              <p>Opening up more opportuities in front of you to get the ticket to more enjoyable door in life.
                Getting equipped with new skills for new sets of insights into your carrer.
                MaxCoach accompany learners in every stage of learning.
              </p>
              <a href="#">Download free guidebook</a>
              
          </div>
         
          <div class="col"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
    name:"SkillBox"

}
</script>

<style lang="scss" scoped>
.box-play{
 height: 100%;
 position: relative;

  img{
    width: 100%;
    z-index: 1;
  }
}



.lines-box{


  .youtube-btn{
    position: absolute;
    top: 50%;
    right: 50%;
    transform: translate(50%,-50%);
    width: 50px;
  }

  .shape-lines{
    position: absolute;
    right: 7px;
    bottom: -50px;
    width: 20%;
    z-index: -1;
  }

  .shape-line{
    position: absolute;
    width: 20%;
    left: -15px;
    top:-20px;
    z-index: -1;

  }


}

.box-info{
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

    a{
      font-weight: bold;
      font-size: 12px;
      color: black;
      text-decoration: none;
      border-bottom: 1px solid grey;
    }
}

</style>
