<template>
  <div class="containerArea">
    <div class="card" v-for="(card, index) in cards" :key="card[index]">
      <img class="imageCard" :src="card.thumb" :alt="card.series">
      <h3>{{card.series}}</h3>
    </div>
  </div>
</template>

<script>
export default {
  name: "MainComponentFirstArea",
  props: ["cards"]
};
</script>

<style lang="scss" scoped>
.containerArea {
  background-color: #1c1c1c;
  h2 {
    color: #fff;
    padding: 60px 9.5%;
  }
}
</style>