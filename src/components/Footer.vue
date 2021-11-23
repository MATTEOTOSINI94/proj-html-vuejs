<template>
  <footer>
      <div class="box-foot">
          <div class="container">
              <div class="row">
                  <div class="col"></div>
                  <div class="col-3">
                      <h4>
                          {{this.FooterDataAddress.intestazione}}
                      </h4>
                      <p>{{this.FooterDataAddress.street}}</p>
                      <p>{{this.FooterDataAddress.contactNumber}}</p>
                      <p>{{this.FooterDataAddress.email}}</p>
                      </div>
                       <div class="col-2"></div>
                  <div class="col">
                      <h4>Explore</h4>
                      <ul class="lista-explore p-0">
                          <li v-for="listEl,i in explore" :key="i"><a href="">{{listEl}}</a></li>
                      </ul>
                  </div>
                  <div class="col-2">
                      <h4>Information</h4>
                      <ul class="lista-info p-0">
                          <li v-for="el in info" :key="el.i"><a href="">{{el}}</a></li>
                      </ul>
                  </div>
                  <div class="col"></div>
                 
              </div>
          </div>
          <div class="text-center box-copyrirght"><h6>© 2020 Maxcoach. All Rights Reserved</h6></div>
      </div>

  </footer>
</template>

<script>
export default {
 name:"Footer",

 data(){
     return{
        FooterDataAddress:{
            intestazione:"Address",
            street:"382 NE 191st St # 87394 Miami, FL 33179-3899",
            contactNumber:"+1 (305) 547-9909",
            email:"support@maxcoach.com",
            icon:[]

        },

        explore:
        [
            "Start here","Success story","Blog","Courses","About us","Contact us"
        ],

        info:["Membership","Purchase guide","Privacy policy","Terms of service"]


     }
 }
}
</script>

<style lang="scss" scoped>
.box-foot{
    background: rgb(23, 22, 33);
    padding-top: 50px ;

    h4{
        color: white;
        font-size: 20px;
    }

    p{
        color: grey;
        font-size: 12px;
    }

    .lista-explore{
        list-style: none;
        display: flex;
        flex-direction: column;
        flex-wrap: wrap;
        height: 70px;
    

        li{
            padding-right: 25px;
            line-height: 23px;
            font-size: 12px;
            

            a{
                color: grey;
                text-decoration: none;
            }
        }
    }

    .lista-info{
        padding-left: 70px;
        list-style: none;

        li{
             line-height: 23px;
            font-size: 12px;
            
            a{  color: grey;
                text-decoration: none;
            }

        }


    }

    .box-copyrirght{
        padding-top: 40px;
        padding-bottom: 40px;

        h6{
            font-size: 13px;
            color: grey;
        }
    }

    
}
</style>


