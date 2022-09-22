<template>
  <div id="app">

      <header>
        <HeaderArea />
      </header>

      <main>
        <MainComponentFirstArea />
        <MainComponentSecondArea />
      </main>

      <footer>

      </footer>
    </div>

</template>

<script>
import HeaderArea from "./components/HeaderArea.vue";
import MainComponentFirstArea from "./components/MainComponentFirstArea.vue";
import MainComponentSecondArea from "./components/MainComponentSecondArea.vue";

export default {
  name: "App",
  components: {
    HeaderArea,
    MainComponentFirstArea,
    MainComponentSecondArea
  },
};
</script>

<style lang="scss">
* {
  box-sizing: border-box;
  margin: 0px;
  padding: 0px;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
