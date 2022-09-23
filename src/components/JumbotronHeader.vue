<template>
  <div class="jumbo">
    <img src="../../public/img/jumbotron.jpg" alt="Jumbotron" />
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.jumbo {
  height: 61vh;

  img {
    width: 100%;
    height: 60vh;
    margin-top: 7px;
    object-fit: cover;
    object-position: top;
  }
}
</style>