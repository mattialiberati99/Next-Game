<template>
  <div class="container-LoginPage h-1000 flex justify-evenly">
    <div class="flex items-center">
        <img class="h-12" src="../../assets/icons/Logo.png" alt="logo">
    </div>
    <div class="form bg-white rounded-3xl p-10 mb-10 mt-20">
      <div class="flex justify-center pt-3">
        <img class="h-8 ml-4" src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/53/Google_%22G%22_Logo.svg/768px-Google_%22G%22_Logo.svg.png" alt="logo google">
        <img class="h-8 ml-4" src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/53/Google_%22G%22_Logo.svg/768px-Google_%22G%22_Logo.svg.png" alt="logo google">
        <img class="h-8 ml-4" src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/53/Google_%22G%22_Logo.svg/768px-Google_%22G%22_Logo.svg.png" alt="logo google">
      </div>
      <div class="text-center mt-2">
        <p>Or with Email</p>
        <form>
          <input class="block rounded-2xl h-16 w-full mt-6 p-2 mb-6 focus:outline-none" type="text" placeholder="Username">
          <input class="block rounded-2xl h-16 w-full mb-6 p-2 focus:outline-none" type="password" placeholder="Password">
          <button class="buttonForm w-full rounded-2xl h-16">Log In</button>
        </form>
        <p class="passwordForgotten mt-6 mb-8">Forgotten password?</p>
        <hr>
        <div class="flex justify-center mt-16">
          <p class="newAccount mr-2">Don't have an account</p>
          <p class="register"><a href="#">Register?</a></p>
        </div>
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

form input {
  background-color : #f2f2f2;
  color: #6E6E6E;
}

.buttonForm {
  background-color:#F46119;
  color: white;
}

.passwordForgotten,
.register {
  color: #F46119;
}

.newAccount {
  color: #6C6C6C;
}

</style>