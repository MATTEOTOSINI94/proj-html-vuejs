<template>
   <ul class=" d-flex lista-nav m-0 ">
        <li v-for="(el,i) in dati" :key="i" class="elemento-lista" ><a  href="#" >{{el}}<i class="fa fa-chevron-down " aria-hidden="true"></i></a> </li>
        
    </ul>
</template>

<script>
export default {
    name:"NavList",

    props:{
        dati:Array
    },

    data(){
        return{
            active:0
        }
    }

}
</script>

<style>
.icons-style{
    width: 10%;
}





    
</style>