<template>
  <div id="app">

      <header>
        <HeaderArea />
      </header>

      <main>

      </main>

      <footer>

      </footer>
    </div>

</template>

<script>
import HeaderArea from "./components/HeaderArea.vue";

export default {
  name: "App",
  components: {
    HeaderArea,
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
