<template>
    <div class="card">
        <img :src="pathImgCard" class="imgCardProduct" />
        <div class="container-product">
            <h3 class="titleCard"><b>{{nameProduct}}</b></h3>
            <p class="categoriesCard">{{categories1}} . {{categories2}}</p>
            <span class="valutationCard">{{valutation}}</span> 
            <span class="starCard">{{star}}</span>
            <span class="priceCard">${{price}} USD</span>
        </div>
        <div>

        </div>
    </div>
</template>

<script>
export default {
    data(){
        return{
           pathImgCard: "https://cdn.akamai.steamstatic.com/steam/apps/595790/capsule_616x353.jpg?t=1642707664",
           nameProduct: "Hell is other demons",
           categories1: "Shooter",
           categories2: "Platform",
           valutation: 4.8,
           star: "⭐",
           price: 4.49
        }
    }
}
</script>

<style>

.card {
    margin: 50px auto;
    background-color: whitesmoke;
    width: 258px;
    padding: 10px;
    border-radius: 25px;
}

.imgCardProduct {
    background-color: #CCCCCC;
    height: 195.25px;
    width: 238px;
    border-radius: 25px;
    margin-bottom: 20px;
}

.container-product {
    padding-left: 10px;
}

.titleCard {
    font-size: 16px;
}

.categoriesCard,
.categoriesCard,
.priceCard {
    font-size: 14px;
}

</style>