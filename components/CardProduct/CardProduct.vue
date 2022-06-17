<template>
    <div class="card">
        <img :src="pathImgCard" class="imgCardProduct" :alt="nameProduct" />
        <div class="container-product">
            <h3 class="titleCard"><b>{{nameProduct}}</b></h3>
            <div class="container-categoriesCard">
                <p class="categoriesCard">{{categories1}}</p>
                <span class="dot"></span> 
                <p class="categoriesCard">{{categories2}}</p>
            </div>
            <span class="valutationCard">{{valutation}}</span> 
            <span class="starCard">{{star}}</span>
            <span class="priceCard"><b>{{price}}</b></span>
            <div class="container-logos-img-Carduser">
                <div class="system-operator-logos">
                   <img class="img-windows" src="../../assets/icons/windows.svg" alt="logo windows">
                   <img class="img-apple" src="../../assets/icons/apple.svg" alt="logo apple">
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

.container-categoriesCard {
    display: flex;
    align-items: center;
}

.valutationCard,
.categoriesCard,
.priceCard{
    color: #767676;
    font-size: 14px;
    line-height: 19px;
}

.dot{
    border-radius: 50%;
    display: block;
    background-color: #767676;
    width: 3px;
    height: 2.96px;
    margin: 0 10px 0 10px;
}

.priceCard {
    color: #616161;
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