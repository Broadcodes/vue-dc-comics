<template>
  <div class="containerArea">
    <ul>
      <li v-for="card in cardShop" :key="card.textTitle">
        <img :src="card.srcImg" :alt="card.textTitle" />
        <a :href="card.link">
          <h3>{{card.textTitle}}</h3>
        </a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "MainComponentSecondArea",
  data(){
    return {
      cardShop: [
        {
          srcImg: 'img/buy-comics-digital-comics.png',
          link: 'digital-comics',
          textTitle: 'DIGITAL COMICS'
        },
        {
          srcImg: 'img/buy-comics-merchandise.png',
          link: 'dc-merchandise',
          textTitle: 'DC MERCHANDISE'
        },
        {
          srcImg: 'img/buy-comics-subscriptions.png',
          link: 'subscription',
          textTitle: 'SUBSCRIPTION'
        },
        {
          srcImg: 'img/buy-comics-shop-locator.png',
          link: 'comic-shop-locator',
          textTitle: 'COMIC SHOP LOCATOR'
        },
        {
          srcImg: 'img/buy-dc-power-visa.svg',
          link: 'dc-power-visa',
          textTitle: 'DC POWER VISA'
        }
      ]
    }
  }
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