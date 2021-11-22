<template>
         <div class="col-3">
          <div class="box-img"><img :src="dati.img" alt="">
        <div><p><strong>{{dati.price}}</strong></p>
        <h5>{{dati.type}}</h5>
        <div class="d-flex"><p>{{dati.include}}</p> <p>{{dati.maxStudend}}</p></div>
        </div>
        </div></div>
</template>

<script>
export default {
    name:"Card",

    props:{
        dati:Object
    }

}
</script>

<style lang="scss" scoped>
.box-img{

    img{
        width: 100%;
    }
}

</style>

