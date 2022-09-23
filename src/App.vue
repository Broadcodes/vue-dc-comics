<template>
  <div id="app">
      <header>
        <HeaderArea />
        <JumbotronHeader />
      </header>

      <main>
        <MainComponentFirstArea :cards="cardsComics"/>
        <MainComponentSecondArea />
      </main>

      <footer>
        <FooterComponentFirstArea />
        <FooterComponentSecondArea />
      </footer>
    </div>

</template>

<script>
import HeaderArea from "./components/HeaderArea.vue";
import MainComponentFirstArea from "./components/MainComponentFirstArea.vue";
import MainComponentSecondArea from "./components/MainComponentSecondArea.vue";
import FooterComponentFirstArea from "./components/FooterComponentFirstArea.vue";
import FooterComponentSecondArea from "./components/FooterComponentSecondArea.vue";
import JumbotronHeader from "./components/JumbotronHeader.vue";

import {cardsComics} from "./data/dc_comics";

export default {
  name: "App",
  components: {
    HeaderArea,
    MainComponentFirstArea,
    MainComponentSecondArea,
    FooterComponentFirstArea,
    FooterComponentSecondArea,
    JumbotronHeader
},
  data(){
    return {
      cardsComics
    }
  }
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
