<template>
   <ul class=" d-flex lista-nav m-0">
        <li v-for="el in dati" :key="el.i"><a href="">{{el}}</a></li>
    </ul>
</template>

<script>
export default {
    name:"NavList",

    props:{
        dati:Array
    }

}
</script>

<style>

</style>