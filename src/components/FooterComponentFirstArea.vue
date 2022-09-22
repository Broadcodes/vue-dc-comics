<template>
  <footer>
    <img src="../assets/img/dc-logo-bg.png" alt="Logo Footer">
    <div class="navigationFooter">
        <div class="col-1">
            <h2>DC COMICS</h2>
            <ul>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Comics</a></li>
                <li><a href="#">Movies</a></li>
                <li><a href="#">TV</a></li>
                <li><a href="#">Games</a></li>
                <li><a href="#">Videos</a></li>
                <li><a href="#">News</a></li>
            </ul>
            <h2>SHOP</h2>
            <ul>
                <li><a href="#">Shop DC</a></li>
                <li><a href="#">Shop DC Collectibles</a></li>
            </ul>
        </div>
        <div class="col-2">
            <h2>DC</h2>
            <ul>
                <li><a href="#">Terms Of Use</a></li>
                <li><a href="#">Privacy policy (New)</a></li>
                <li><a href="#">Ad Choices</a></li>
                <li><a href="#">Advertising</a></li>
                <li><a href="#">Jobs</a></li>
                <li><a href="#">Subscriptions</a></li>
                <li><a href="#">Talent Workshops</a></li>
                <li><a href="#">CPSC Certificates</a></li>
                <li><a href="#">Ratings</a></li>
                <li><a href="#">Shop Help</a></li>
                <li><a href="#">Contact Us</a></li>
            </ul>
        </div>
        <div class="col-3">
            <h2>SITES</h2>
            <ul>
                <li><a href="#">DC</a></li>
                <li><a href="#">MAD Magazine</a></li>
                <li><a href="#">DC Kids</a></li>
                <li><a href="#">DC Universe</a></li>
                <li><a href="#">DC Pawer Visa</a></li>
            </ul>
        </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "FooterComponentFirstArea",
};
</script>

<style lang="scss" scoped>
footer {
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-content: center;
  background-image: url("../assets/img/footer-bg.jpg");
  background-size: 120%;
  padding: 40px 8% 70px;
  position: relative;
  overflow: hidden;

  img{
    position: absolute;
    top: -80px;
    right: -60px;
    transform: scale(1.1);
  }

  .navigationFooter{
    width: 40%;
    display: flex;

    .col-1,
    .col-2,
    .col-3{
        width: calc(100% / 3);
        height: 100%;

        h2{
            color: #fff;
            font-size: 1.3rem;
            padding: 15px 0;
        }

        ul{
            list-style-type: none;

            li a{
                text-decoration: none;
                color: #848485;
                font-size: 0.9rem;
                line-height: 1.3rem;
            }
        }
    }
  }
}
</style>