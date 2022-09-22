<template>
  <div id="app">

      <header>
        <HeaderArea />
      </header>

      <main>
        <MainComponentFirstArea />
      </main>

      <footer>

      </footer>
    </div>

</template>

<script>
import HeaderArea from "./components/HeaderArea.vue";
import MainComponentFirstArea from "./components/MainComponentFirstArea.vue";

export default {
  name: "App",
  components: {
    HeaderArea,
    MainComponentFirstArea
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
