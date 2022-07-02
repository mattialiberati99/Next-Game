<template>
  <div class="container-LoginPage flex justify-evenly">
    <div class="flex flex-col justify-center">
        <img class="h-16" src="../../assets/icons/Logo.png" alt="logo">
        <h3 class="text-white">Join ULT now and play mighty <br>games!</h3>
    </div>
    <div class="conteinerForm bg-white rounded-3xl p-10 mb-10 mt-20 h-2/4 max-w-2xl w-full">
      <div class="flex justify-center pt-2">
        <a href="#"><img class="h-14" src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/53/Google_%22G%22_Logo.svg/768px-Google_%22G%22_Logo.svg.png" alt="logo google"></a>
        <a href="#"><img class="h-14 ml-6" src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/53/Google_%22G%22_Logo.svg/768px-Google_%22G%22_Logo.svg.png" alt="logo google"></a>
        <a href="#"><img class="h-14 ml-6" src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/53/Google_%22G%22_Logo.svg/768px-Google_%22G%22_Logo.svg.png" alt="logo google"></a>
      </div>
      <div class="text-center mt-6">
        <div class="flex items-center">
          <hr class="h-0.5 flex-1 mx-4">
          <p class="enterWithEmail">or with Email</p>
          <hr class="h-0.5 flex-1 mx-4">
        </div>
        <form>
          <input class="block rounded-2xl h-16 w-full mt-6 p-4 mb-6 focus:outline-none" type="email" placeholder="Email">
          <input class="block rounded-2xl h-16 w-full mt-6 p-4 mb-6 focus:outline-none" type="text" placeholder="Username">
          <input class="block rounded-2xl h-16 w-full mb-6 p-6 focus:outline-none" type="password" placeholder="Password">
          <button class="buttonForm w-full rounded-2xl h-16">Register</button>
        </form>
        <hr>
        <div class="flex justify-center mt-10">
          <p class="newAccount mr-2">Already have an account?</p>
          <p class="register"><a href="#">Log In</a></p>
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

hr {
  background-color: #E9E9E9;
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

.newAccount,
.enterWithEmail {
  color: #6C6C6C;
}

</style>