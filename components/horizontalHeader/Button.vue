<template>
    <NuxtLink :to="to" style="width:calc(100% - 10px);">
        <div class="flex flex-row items-center w-full p-2 h-auto rounded-r-3xl buttonHeader" v-bind:class="isActive ? 'active' : ''">
            <img v-if="!isActive" v-bind:src="'/icons/'+to+'.svg'" class="icon w-6 h-6" >
            <img v-else v-bind:src="'/icons/'+to+'Solid.svg'" class="icon w-6 h-6">

            <h1 class="text w-1/4 font-semibold text-sm leading-5">{{ name }}</h1>
            <div v-if="notification" class="notification flex justify-center items-center w-5 h-5 rounded-full p-px">
                <h4 class="font-semibold text-xs leading-3">{{ notification > 99 ? 99 : notification }}</h4>
            </div>
        </div>
    </NuxtLink>
</template>

<style>
.buttonHeader {
    transition: background-color 0.4s;
}

.buttonHeader.active {
    background-color: rgba(244, 98, 25, 0.265);
    position: relative;
}

.buttonHeader.active::before {
    content: "";
    width: 4.5px;
    background-color: var(--light1);
    height: 100%;
    position: absolute;
    top: 0;
    left: 0;
    border-radius: 0px 5px 5px 0px;
}

.buttonHeader:hover {
    background-color: #64646434;
}

.buttonHeader.active:hover {
    background-color: rgba(244, 98, 25, 0.319);
}

.buttonHeader .icon {
   
    margin-left: 25px;/*+8*/ 
    margin-right: 20px;
    filter: invert(36%) sepia(0%) saturate(2829%) hue-rotate(137deg) brightness(103%) contrast(80%);
    -webkit-filter: invert(36%) sepia(0%) saturate(2829%) hue-rotate(137deg) brightness(103%) contrast(80%);
}

.buttonHeader.active .icon {
   filter:invert(64%) sepia(62%) saturate(5282%) hue-rotate(353deg) brightness(100%) contrast(92%);
}

.buttonHeader h1 {
    margin: 0 25px;
}

.buttonHeader .text {
    color: var(--light6);
}

.buttonHeader .notification {
    background-color: var(--light1);
}

.buttonHeader .notification h4 {
    color: var(--light4);
}
</style>
<script>
export default {
    props: {
        to: String,
        name: String,
        notification: Number | String,
        icon: String,
        isActive: String
    },
    data (){
        return {
            color:`../../icons/user.svg`
        }
    }
}
</script>