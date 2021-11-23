<template>
  <div class="box-bg">
      <div class="box-bg-content">
          <h4 class="m-0"><strong>Commence New Buisness</strong></h4>
          <h1>Distant Mentoring Program</h1>
          <button>Download Free GuidBook</button>
      </div>
  </div>
</template>

<script>
export default {
    name: "HeroMain"

}
</script>

<style lang="scss" scoped>
.box-bg{
    background: url(../assets/home-3-hero-bg.jpg);
    background-position: center center;
    background-size: cover;
    height: 100vh;
    position: relative;

    .box-bg-content{
        text-align: center;
        position: absolute;
        top: 50%;
        right: 50%;
        transform: translate(50%,-50%);


        h4,h1{
            color: white;
        }

        button{
            margin-top: 8px;
            padding: 10px 25px;
            border: 0;
            border-radius: 5px;
            background-color: white;
            font-size: 10px;
        }
    }
}

</style>

