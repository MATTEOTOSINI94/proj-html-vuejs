<template>
<header>
  <div class="head-conteiner">
  <div class="container ">
    
    <div class="d-flex box-nav">
     <NavList :dati="navBarList"></NavList>

      <div class="logo-container ">
        <img src='../assets/dark-logo.png' alt="">
      </div>

      <div class="inptu-container ms-auto">
        <i class="fa fa-cart-plus" aria-hidden="true"></i>
        <i class="fa fa-user-circle-o" aria-hidden="true"></i>
           <input class="input-text" type="text" placeholder="Search..">
        
      </div>
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

.head-conteiner{
  overflow: hidden;
    background-color: #333;
    position: fixed;
    top: 0;
    right: 0;
    left: 0;
    width: 100%;
    z-index: 100;
    background: white;}
  .container{
    padding: 10px 0;

    .box-nav{
      align-items:center;
      padding: 10px 0;
    }

    .lista-nav{
      width: 40%;
      list-style: none;
      padding: 0;
      gap: 20px;

      li{
        min-width: fit-content;
        font-size: 13px;

        a{
         text-decoration: none;
         color: black;
        }

        a:hover{
          color: #1fad95;
        }
      }
    }

    .logo-container{
      width: 20%;
      text-align: center;
      
 
    img{
      width: 100px;
    }

    }

    .input-container{
      
      width: 40%;
      text-align: end;
    }

    .input-text{
      
      padding-right: 20px;
    }

    .fa-user-circle-o{
      padding:0 10px;
    }
   
    

  }

  
</style>
