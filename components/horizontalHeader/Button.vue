<template>
    <NuxtLink :to="to" style="width:calc(100% - 10px);">
        <div class="flex flex-row items-center buttonHeader" v-bind:class="isActive ? 'active' : ''">
            <div class="icon"></div>
            <h1 class="text">{{ name }}</h1>
            <div v-if="notification" class="notification flex justify-center items-center">
                <h4>{{ notification > 99 ? 99 : notification }}</h4>
            </div>
        </div>
    </NuxtLink>
</template>

<style>
.buttonHeader {
    height: auto;
    width: 100%;
    padding: 8px;
    border-top-right-radius: 30px;
    border-bottom-right-radius: 30px;
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
    width: 24px;
    height: 24px;
    border-radius: 100%;
    background-color: var(--light6);
    margin-left: 25px;
    margin-right: 20px;
}

.buttonHeader.active .icon {
    background-color: var(--light1);
}

.buttonHeader h1 {
    margin: 0 25px;
}

.buttonHeader .text {
    width: 23%;
    color: var(--light6);
    font-weight: 600;
    font-size: 14px;
    line-height: 19px;
}

.buttonHeader .notification {
    width: 18px;
    height: 18px;
    padding: 1px;
    border-radius: 100%;
    background-color: var(--light1);
}

.buttonHeader .notification h4 {
    font-weight: 600;
    font-size: 10px;
    line-height: 13px;
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
        isActive: Boolean
    }
}
</script>