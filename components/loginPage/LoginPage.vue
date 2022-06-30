<template>
  <div class="container-LoginPage h-screen flex justify-evenly pt-20">
    <div class="flex items-center">
        <img class="h-12" src="../../assets/icons/Logo.png" alt="logo">
    </div>
    <div class="form bg-white rounded-3xl p-10">
      <div class="flex justify-center pt-3">
        <img class="h-8 ml-4" src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/53/Google_%22G%22_Logo.svg/768px-Google_%22G%22_Logo.svg.png" alt="logo google">
        <img class="h-8 ml-4" src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/53/Google_%22G%22_Logo.svg/768px-Google_%22G%22_Logo.svg.png" alt="logo google">
        <img class="h-8 ml-4" src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/53/Google_%22G%22_Logo.svg/768px-Google_%22G%22_Logo.svg.png" alt="logo google">
      </div>
      <div>
        <p>or with Email</p> 
        <form class="flex">
          <input class="" type="text">
          <input type="password">
          <button></button>
        </form>
        <p>Forgotten password?</p>
        <hr>
        <p>Don't have an account? Register</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
    data(){
        return{

        }
    }
}
</script>

<style>
.container-LoginPage{
    background: rgb(10,10,10);
    background: linear-gradient(90deg, rgba(10,10,10,0.9459459459459459) 0%, rgba(0,0,0,0.38264580369843526) 100%);
}

.form {
  width: 540px;
  height: 634.9px;
}
</style>