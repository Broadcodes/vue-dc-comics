<template>
  <footer>
    <input type="button" value="SIGN-UP NOW!" />
    <div class="containerSocial">
      <h2>FOLLOW US</h2>
      <img src="../assets/img/footer-facebook.png" alt="" />
      <img src="../assets/img/footer-twitter.png" alt="" />
      <img src="../assets/img/footer-youtube.png" alt="" />
      <img src="../assets/img/footer-pinterest.png" alt="" />
      <img src="../assets/img/footer-periscope.png" alt="" />
    </div>
  </footer>
</template>

<script>
export default {
  name: "FooterComponentSecondArea",
};
</script>

<style lang="scss" scoped>
footer {
  display: flex;
  justify-content: space-between;
  padding: 30px 8%;
  background-color: #303030;

  input {
    background: none;
    padding: 10px;
    color: #fff;
    border: 2px solid #047dee;

    &:hover{
        background-color: #047dee58;
    }
  }

  .containerSocial {
    display: flex;
    align-items: center;

    h2 {
      color: #047dee;
      padding: 0 20px;
      font-size: 1.1rem;
    }

    img {
      margin: 0 8px;
      cursor: pointer;
    }
  }
}
</style>