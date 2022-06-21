<template>
    <div class="card">
        <img :src="item.pathImgCard" class="imgCardProduct" :alt="item.nameProduct" />
        <div class="container-product">
            <h3 class="titleCard"><b>{{item.nameProduct}}</b></h3>
            <div class="container-categoriesCard">
                <p class="categoriesCard">{{item.categories1}}</p>
                <span class="dot"></span> 
                <p class="categoriesCard">{{item.categories2}}</p>
            </div>
            <span class="valutationCard">{{item.valutation}}</span> 
            <span class="starCard">⭐</span>
            <span class="priceCard"><b>{{item.price}}</b></span>
            <div class="container-logos-img-Carduser">
                <div class="system-operator-logos">
                   <img class="img-windows" src="../../assets/icons/windows.svg" alt="logo windows">
                   <img class="img-apple" src="../../assets/icons/apple.svg" alt="logo apple">
                </div>
                <div class="container-img-cardUser">
                    <img :src="item.imgUser" alt="">
                    <img :src="item.imgUser" alt="">
                    <img :src="item.imgUser" alt="">
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
.card {
    background-color: rgb(255, 255, 255);
    max-width: 258px;
    padding: 10px;
    border-radius: 25px;
    margin-top: 20px;
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
.categoriesCard{
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
    font-size: 14px;
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
    border: 2px solid white;
    border-radius: 50%;
    margin-right: -5px;
}

</style>