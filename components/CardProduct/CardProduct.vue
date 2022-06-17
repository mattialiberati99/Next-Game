<template>
    <div class="card">
        <img :src="pathImgCard" class="imgCardProduct" :alt="nameProduct" />
        <div class="container-product">
            <h3 class="titleCard"><b>{{nameProduct}}</b></h3>
            <p class="categoriesCard">{{categories1}} . {{categories2}}</p>
            <span class="valutationCard">{{valutation}}</span> 
            <span class="starCard">{{star}}</span>
            <span class="priceCard"><b>{{price}}</b></span>
            <div class="container-logos-img-Carduser">
                <div class="system-operator-logos">
                    <svg class="img-windows" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><path d="M0 93.7l183.6-25.3v177.4H0V93.7zm0 324.6l183.6 25.3V268.4H0v149.9zm203.8 28L448 480V268.4H203.8v177.9zm0-380.6v180.1H448V32L203.8 65.7z"/></svg>
                    <svg class="img-apple" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 384 512"><path d="M318.7 268.7c-.2-36.7 16.4-64.4 50-84.8-18.8-26.9-47.2-41.7-84.7-44.6-35.5-2.8-74.3 20.7-88.5 20.7-15 0-49.4-19.7-76.4-19.7C63.3 141.2 4 184.8 4 273.5q0 39.3 14.4 81.2c12.8 36.7 59 126.7 107.2 125.2 25.2-.6 43-17.9 75.8-17.9 31.8 0 48.3 17.9 76.4 17.9 48.6-.7 90.4-82.5 102.6-119.3-65.2-30.7-61.7-90-61.7-91.9zm-56.6-164.2c27.3-32.4 24.8-61.9 24-72.5-24.1 1.4-52 16.4-67.9 34.9-17.5 19.8-27.8 44.3-25.6 71.9 26.1 2 49.9-11.4 69.5-34.3z"/></svg>
                </div>
                <div class="container-img-cardUser">
                    <img :src="imgUser" alt="">
                    <img :src="imgUser" alt="">
                    <img :src="imgUser" alt="">
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data(){
        return{
           pathImgCard: "https://cdn-www.bluestacks.com/bs-images/Featured_com.gtarcade.ioe_.global.jpg",
           nameProduct: "Infinity Kingdom",
           categories1: "Strategy",
           categories2: "Platform",
           valutation: 4.5,
           star: "⭐",
           price: "Free",
           imgUser: "https://www.w3schools.com/w3css/img_avatar3.png"
        }
    }
}
</script>

<style>

.card {
    margin: 50px auto;
    width: 258px;
    padding: 10px;
    border-radius: 25px;
}

.imgCardProduct {
    height: 195.25px;
    width: 238px;
    border-radius: 25px;
    margin-bottom: 20px;
    object-fit: cover;
}

.container-product {
    padding-left: 10px;
}

.titleCard {
    font-size: 16px;
}

.categoriesCard {
    margin: 2px 0;
}

.categoriesCard,
.priceCard {
    font-size: 14px;
}

.priceCard {
    color: var(--light6);
}

.system-operator-logos {
    display: flex;
}

.img-windows,
.img-apple {
    height: 20px;
    margin-right: 10px;
}

.container-logos-img-Carduser {
    margin: 10px 0;
    display: flex;
    justify-content: space-between;
}

.container-img-cardUser {
    display: flex;
    height: 24px;
}

.container-img-cardUser > img {
    border-radius: 50%;
    margin-right: 2px;
}

</style>