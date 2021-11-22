<template>
   <ul class=" d-flex lista-nav">
        <li v-for="el in dati" :key="el.i">{{el}}</li>
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