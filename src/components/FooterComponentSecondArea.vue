<template>
  <footer>
    <input type="button" value="SIGN-UP NOW!" />
    <div class="containerSocial">
      <h2>FOLLOW US</h2>
      <img v-for="image in imageSocial" :key="image.alt" :src="image.link" :alt="image.alt" />
    </div>
  </footer>
</template>

<script>
export default {
  name: "FooterComponentSecondArea",
  data() {
    return {
      imageSocial: [
        {
          link: "img/footer-facebook.png",
          alt: "facebook",
        },
        {
          link: "img/footer-twitter.png",
          alt: "twitter",
        },
        {
          link: "img/footer-youtube.png",
          alt: "youtube",
        },
        {
          link: "img/footer-pinterest.png",
          alt: "pinterest",
        },
        {
          link: "img/footer-periscope.png",
          alt: "periscope",
        },
      ],
    };
  },
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

    &:hover {
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