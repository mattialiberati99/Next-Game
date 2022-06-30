<template>
    <div class="rounded-3xl h-75 w-64 p-3 mt-5 mr-2 bg-white">
        <img class="w-full rounded-3xl w-60 h-48 object-cover" :src="item.pathImgCard" alt="Sunset in the mountains" />
        <div class="px-6 py-4">
          <h2 class="font-bold text-l">{{item.nameProduct}}</h2>
          <div class="flex text-sm container-categories items-center">
            <p>{{item.categories1}}</p>
            <span class="dot rounded-full w-1 h-1 mr-2 ml-2"></span>
            <p>{{item.categories2}}</p>
          </div>
          <div class="flex text-sm container-price items-center mt-1 mb-1">
            <p>{{item.valutation}}</p>
            <svg class="star h-4 mr-2.5 ml-2.5" xmlns="http://www.w3.org/2000/svg" width="15" height="15" fill="none"><path d="M7.94838 0.778719C7.86415 0.60805 7.69034 0.5 7.50001 0.5C7.30969 0.5 7.13587 0.60805 7.05165 0.778719L5.00476 4.92621L0.42816 5.59081C0.239806 5.61816 0.0833166 5.75008 0.0244934 5.93109C-0.0343298 6.1121 0.0147161 6.31081 0.151008 6.44366L3.46277 9.67185L2.68076 14.2306C2.64858 14.4182 2.72569 14.6078 2.87966 14.7196C3.03364 14.8315 3.23778 14.8463 3.40624 14.7577L7.50001 12.6054L11.5938 14.7577C11.7623 14.8463 11.9664 14.8315 12.1204 14.7196C12.2743 14.6078 12.3515 14.4182 12.3193 14.2306L11.5373 9.67185L14.849 6.44366C14.9853 6.31081 15.0344 6.1121 14.9755 5.93109C14.9167 5.75008 14.7602 5.61816 14.5719 5.59081L9.99527 4.92621L7.94838 0.778719Z" fill="orange"/></svg>
            <h3 class="price font-bold">{{item.price}}</h3>
            <p class="symbol-dollar font-bold" v-if="item.price !== 'Free'"> USD</p>
          </div>
          <div class="flex justify-between">
            <div class="flex">
                   <img class="img-windows h-4" src="../../assets/icons/windows.svg" alt="logo windows">
                   <img class="img-apple h-4" src="../../assets/icons/apple.svg" alt="logo apple">
            </div>
            <div class="flex">
                <img class="rounded-full w-6 border-white border-2 -mr-1" :src="item.imgUser" alt="user image">
                <img class="rounded-full w-6 border-white border-2 -mr-1" :src="item.imgUser" alt="user image">
                <img class="rounded-full w-6 border-white border-2 -mr-1" :src="item.imgUser" alt="user image">
            </div>
          </div>
        </div>
    </div>
</template>

<script>
export default {
    props: ["item"],
    data(){
        return{}
    }
}
</script>

<style>

.container-categories,
.container-price {
    color: #767676;
}

.dot {
  background: #767676;
}

.price,
.symbol-dollar {
    color: #616161;
}


</style> 

