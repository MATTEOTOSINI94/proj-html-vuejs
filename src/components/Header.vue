<template>
<header>
  <div class="container ">
    
    <div class="d-flex box-nav">
     <NavList :dati="navBarList"></NavList>

      <div class="logo-container ">
        <img src='../assets/dark-logo.png' alt="">
      </div>

      <div class="inptu-container ms-auto">
        <input type="text">
      </div>
      </div>

    
  </div>
</header>
</template>

<script>
import NavList from "./Listnavbar.vue"
export default {
  name: 'Head',

  components:{
    NavList
  },
  data(){

    return{

      navBarList:[
        "Home","Pages","Courses","Features","Blog","Shop"
      ]
    }
  }

 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style  lang="scss">
  .container{
    padding: 10px 0;

    .lista-nav{
      list-style: none;
      padding: 0;

      li{
        padding: 0 10px;
        font-size: 13px;
      }
    }

    .logo-container{
      text-align: center;
      padding-left: 200px;
 
    img{
      width: 100px;
    }

    }

    .input-container{
     text-align: end;
    }
    

  }
</style>
