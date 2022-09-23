<template>
  <header>
    <img src="img/dc-logo.png" alt="Logo DC" />
    <div class="navigation">
      <ul>
        <li
          v-for="item in menu"
          :key="item.name"
          :class="{ active: item.active }"
        >
          <a :href="item.link">{{ item.name }}</a>
        </li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: "HeaderArea",
  data() {
    return {
      menu: [
        {
          name: "CHARACTERS",
          link: "characters",
          active: false,
        },
        {
          name: "COMICS",
          link: "comics",
          active: true,
        },
        {
          name: "MOVIES",
          link: "movies",
          active: false,
        },
        {
          name: "TV",
          link: "tv",
          active: false,
        },
        {
          name: "GAMES",
          link: "games",
          active: false,
        },
        {
          name: "COLLECTIBLES",
          link: "collectibles",
          active: false,
        },
        {
          name: "VIDEOS",
          link: "videos",
          active: false,
        },
        {
          name: "FANS",
          link: "fans",
          active: false,
        },
        {
          name: "NEWS",
          link: "news",
          active: false,
        },
        {
          name: "SHOP",
          link: "shop",
          active: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
header {
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-content: center;
  padding: 0px 8%;
  margin-top: 7px;

  img {
    width: 130px;
    height: 130px;
    padding: 20px;
  }
  .navigation {
    flex-grow: 1;
    display: flex;
    justify-content: flex-end;

    ul {
      display: flex;
      list-style-type: none;

      li {
        display: flex;
        align-items: center;
        height: 100%;
        margin: 0 17px;
        font-size: 0.9rem;

        &.active,
        &:hover {
          height: calc(100% + 7px);
          border-bottom: 7px solid #0282f9;
        }

        a {
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