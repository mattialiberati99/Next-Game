<template>
  <div class="flex justify-between">
    <div>
      <Header />
    </div>
    <div>
      <ContainerCard />
    </div>
  </div>
</template>

<script>
import Header from '../horizontalHeader/Header.vue';
import ContainerCard from '../containerCard/ContainerCard.vue';

export default {
  name: "GameStore",
  components: { Header, ContainerCard }
}
</script>
