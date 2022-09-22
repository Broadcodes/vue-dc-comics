<template>
  <div class="containerArea">
    <ul>
      <li>
        <img
          src="../assets/img/buy-comics-digital-comics.png"
          alt="DIGITAL COMICS"
        />
        <a href="#">
          <h3>DIGITAL COMICS</h3>
        </a>
      </li>
      <li>
        <img
          src="../assets/img/buy-comics-merchandise.png"
          alt="DC MERCHANDISE"
        />
        <a href="#">
          <h3>DC MERCHANDISE</h3>
        </a>
      </li>
      <li>
        <img
          src="../assets/img/buy-comics-subscriptions.png"
          alt="SUBSCRIPTION"
        />
        <a href="#">
          <h3>SUBSCRIPTION</h3>
        </a>
      </li>
      <li>
        <img
          src="../assets/img/buy-comics-shop-locator.png"
          alt="COMIC SHOP LOCATOR"
        />
        <a href="#">
          <h3>COMIC SHOP LOCATOR</h3>
        </a>
      </li>
      <li>
        <img src="../assets/img/buy-dc-power-visa.svg" alt="DC POWER VISA" />
        <a href="#">
          <h3>DC POWER VISA</h3>
        </a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "MainComponentSecondArea",
};
</script>

<style lang="scss" scoped>
.containerArea {
  display: flex;
  justify-content: center;
  background-color: #0282f9;
  ul {
    width: 80%;
    display: flex;
    justify-content: space-around;
    align-items: center;
    list-style-type: none;

    li{
        width: calc(100% / 5);
        height: 100%;
        display: flex;
        align-items: center;
        img{
            height: 35%;
        }

        a {
            text-decoration: none;
            font-size: 0.7rem;
            color: #fff;
            margin: 10px;
            transition: transform .7s;

            &:hover{
                transform: translateX(10px);
            }
        }
    }
  }
}
</style>