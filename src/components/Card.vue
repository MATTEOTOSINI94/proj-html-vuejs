<template>
    <div class="col-3 card-box">
        <div class="box-img">
                <img :src="dati.img" alt="">
            <div class="box-text">
                <strong>{{dati.price}}<span class="coin-style">{{dati.coin}}</span></strong>
                <h6>{{dati.type}}</h6>
               <div class="d-flex">
                    <p>{{dati.include}}  </p>
                    <p class="ps-3">{{dati.maxStudend}}</p>
                </div>
            </div>
      </div>
    </div>
</template>

<script>
export default {
    name:"Card",

    props:{
        dati:Object,
        
    }

}
</script>

<style lang="scss" scoped>


.box-img{


    img{
        width: 100%;
    }

    .box-text{
        background-color: white;
        border-radius: 10px;
        min-height: 150px;
        padding: 20px;

        h6{
           
            padding-top: 10px ;
            padding-bottom: 10px;
            font-weight: bold;


        }

        p{
            font-size: 10px;
        }

        strong{
            
            color: #1fad95;
        }

        .coin-style{
            font-size: 11px;
        }
    }
}

</style>

