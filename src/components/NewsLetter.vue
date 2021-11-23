<template>
  <div class="box-newsletter">
  <div class="text-center">
     <h1>Subscribe <span class="style-work">NewsLetter</span></h1>
     <p>Enter your email address to register to our newsletter subscription <br> delivered on a regular basis!</p>
     <form>
        
        <input class="text-email-style" placeholder="Enter your email" type="email" id="email" name="email">
        <input class="btn-sub" type="submit">
    </form>

  </div>
  </div>
</template>

<script>
export default {
    name:"NewsLetter"

}
</script>

<style lang="scss" scoped>
.box-newsletter{
  padding: 100px 0;

   .style-work{
        color: #1fad95;
        font-weight: 100;
    }
   

   h1{
     font-weight: bold;
     padding-bottom: 35px;
   }



   .btn-sub{

     border: 0;
     padding: 10px 30px;  
     border-radius: 0px 5px 5px 0px;
     background-color: #1fad95;
     color: whitesmoke;
   }
  .text-email-style{
    width: 40%;
    padding: 10px 30px;
    border: 0;
    background: rgba(228, 228, 228, 0.767);

    
  }
}

</style>

