<template>
    <div class="containerCard flex flex-wrap justify-start">
        <CardProduct v-for="card in cards" v-bind:item="card" :key="card.id" />
    </div>
</template>


<script>
export default {
    data() {
        return {
            cards: [
                {
                    id: 1,
                    pathImgCard: "https://cdn-www.bluestacks.com/bs-images/Featured_com.gtarcade.ioe_.global.jpg",
                    nameProduct: "Infinity Kingdom",
                    categories1: "Strategy",
                    categories2: "Platform",
                    valutation: 4.5,
                    price: "Free",
                    imgUser: "https://www.w3schools.com/w3css/img_avatar3.png"
                },
                {
                    id: 2,
                    pathImgCard: "https://cdn.akamai.steamstatic.com/steam/apps/975270/header.jpg?t=1626291858",
                    nameProduct: "Legion War",
                    categories1: "Strategy",
                    categories2: "Adventure",
                    valutation: 4.1,
                    price: "$9.99",
                    imgUser: "https://www.w3schools.com/w3css/img_avatar3.png"
                },
                {
                    id: 3,
                    pathImgCard: "https://steamcdn-a.akamaihd.net/steam/apps/1291010/header.jpg",
                    nameProduct: "Warpips",
                    categories1: "Strategy",
                    categories2: "Tower Defence",
                    valutation: 4.5,
                    price: "$11.99",
                    imgUser: "https://www.w3schools.com/w3css/img_avatar3.png"
                },
                {
                    id: 4,
                    pathImgCard: "https://steamcdn-a.akamaihd.net/steam/apps/1291010/header.jpg",
                    nameProduct: "Warpips",
                    categories1: "Strategy",
                    categories2: "Tower Defence",
                    valutation: 4.5,
                    price: "$11.99",
                    imgUser: "https://www.w3schools.com/w3css/img_avatar3.png"
                },
                {
                    id: 5,
                    pathImgCard: "https://steamcdn-a.akamaihd.net/steam/apps/1291010/header.jpg",
                    nameProduct: "Warpips",
                    categories1: "Strategy",
                    categories2: "Tower Defence",
                    valutation: 4.5,
                    price: "$11.99",
                    imgUser: "https://www.w3schools.com/w3css/img_avatar3.png"
                },
                {
                    id: 6,
                    pathImgCard: "https://steamcdn-a.akamaihd.net/steam/apps/1291010/header.jpg",
                    nameProduct: "Warpips",
                    categories1: "Strategy",
                    categories2: "Tower Defence",
                    valutation: 4.5,
                    price: "$11.99",
                    imgUser: "https://www.w3schools.com/w3css/img_avatar3.png"
                },
                {
                    id: 7,
                    pathImgCard: "https://steamcdn-a.akamaihd.net/steam/apps/1291010/header.jpg",
                    nameProduct: "Warpips",
                    categories1: "Strategy",
                    categories2: "Tower Defence",
                    valutation: 4.5,
                    price: "$11.99",
                    imgUser: "https://www.w3schools.com/w3css/img_avatar3.png"
                },
                {
                    id: 8,
                    pathImgCard: "https://steamcdn-a.akamaihd.net/steam/apps/1291010/header.jpg",
                    nameProduct: "Warpips",
                    categories1: "Strategy",
                    categories2: "Tower Defence",
                    valutation: 4.5,
                    price: "$11.99",
                    imgUser: "https://www.w3schools.com/w3css/img_avatar3.png"
                },
                {
                    id: 9,
                    pathImgCard: "https://steamcdn-a.akamaihd.net/steam/apps/1291010/header.jpg",
                    nameProduct: "Warpips",
                    categories1: "Strategy",
                    categories2: "Tower Defence",
                    valutation: 4.5,
                    price: "$11.99",
                    imgUser: "https://www.w3schools.com/w3css/img_avatar3.png"
                }
            ]
        }
    }
}
</script>