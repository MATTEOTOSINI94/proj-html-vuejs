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


.card-box{
    height: 100%;


    img{
        width: 100%;
    }

    .box-text{
        background-color: white;
        -webkit-border-bottom-right-radius: 10px;
        -webkit-border-bottom-left-radius: 10px;
        -moz-border-radius-bottomright: 10px;
        -moz-border-radius-bottomleft: 10px;
        border-bottom-right-radius: 10px;
        border-bottom-left-radius: 10px;
        min-height: 150px;
        padding: 20px;
        transition: 0.7s;

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

    .box-text:hover{
        background-color: #1fad95;;
        color: white;

        strong{color: white;}
    }
}


</style>

