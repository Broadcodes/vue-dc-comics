<template>
  <header>
    <img src="../assets/img/dc-logo.png" alt="Logo DC" />
    <div class="navigation">
      <ul>
        <li><a href="#">CHARACTERS</a></li>
        <li><a href="#">COMICS</a></li>
        <li><a href="#">MOVIES</a></li>
        <li><a href="#">TV</a></li>
        <li><a href="#">GAMES</a></li>
        <li><a href="#">COLLECTIBLES</a></li>
        <li><a href="#">VIDEOS</a></li>
        <li><a href="#">FANS</a></li>
        <li><a href="#">NEWS</a></li>
        <li><a href="#">SHOP</a></li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: "HeaderArea",
};
</script>

<style lang="scss" scoped>
header {
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-content: center;
  padding: 0px 8%;

  img {
    width: 130px;
    height: 130px;
    padding: 20px;
  }
  .navigation{
    flex-grow: 1;
    display: flex;
    justify-content: end;
    
    ul{
        display: flex;
        list-style-type: none;
        
        li{
            display: flex;
            align-items: center;
            height: 100%;
            margin: 0 17px;
            font-size: 0.9rem;

        &:hover{
            height: calc(100% + 7px);
            border-bottom: 7px solid #0282f9;
        }

            a{
                text-decoration: none;
                color: #000;
                font-weight: bold;
                cursor: pointer;
            }
        }
    }
  }
}
</style>