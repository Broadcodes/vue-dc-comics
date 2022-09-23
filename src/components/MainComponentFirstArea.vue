<template>
  <div class="containerArea">
    <span>CURRENT SERIES</span>
    <div class="card" v-for="(card, index) in cards" :key="card[index]">
      <img class="imageCard" :src="card.thumb" :alt="card.series" />
      <h3>{{ card.series }}</h3>
    </div>
    <button>LOAD MORE</button>
  </div>
</template>

<script>
export default {
  name: "MainComponentFirstArea",
  props: ["cards"],
};
</script>

<style lang="scss" scoped>
@mixin blueArea {
  color: #fff;
  background-color: #0282f9;
}

.containerArea {
  position: relative;
  background-color: #1c1c1c;
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  padding: 60px 9.5%;

  span {
    position: absolute;
    top: -20px;
    left: 8%;
    padding: 10px 20px;
    @include blueArea();
  }

  button{
    @include blueArea();
    position: relative;
    top: 40px;
    padding: 10px 60px;
    cursor: pointer;

    &:hover{
      background-color: #3ba0ff;
    }
  }

  .card {
    width: calc(100% / 6);

    .imageCard {
      width: 180px;
      height: 180px;
      object-fit: cover;
      object-position: top;
      transition: transform 0.5s;

      &:hover {
        transform: scale(1.1);
      }
    }

    h3 {
      color: #fff;
      font-size: 0.8rem;
      text-transform: uppercase;
      padding: 15px 0;
    }
  }
}
</style>