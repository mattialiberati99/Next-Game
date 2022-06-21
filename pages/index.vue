<template>
  <div>
    <ContainerCard />
  </div>
</template>

<script>
import NuxtLogo from '../components/NuxtLogo.vue';
import Header from '../components/horizontalHeader/Header.vue';
import ContainerCard from '../components/ContainerCard/ContainerCard.vue';
import CardProduct from '../components/CardProduct/CardProduct.vue';
export default {
    name: "IndexPage",
    components: { NuxtLogo, Header, ContainerCard, CardProduct }
}
</script>

<style>


</style>