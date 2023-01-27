<template>
  <header class="header">
    <div class="container">
      <div class="row header__wrapper">
        <router-link class="header__logo" to="/"
          ><img src="../assets/logo.png" alt=""
        /></router-link>
        <ul class="header__nav">
          <li class="header__nav__item" v-for="item in nav" :key="item.id">
            <router-link :to="item.link" class="header__nav__link">
              {{ item.title }}
            </router-link>
          </li>
        </ul>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  data() {
    return {
      nav: [
        {
          id: 1,
          title: "Главная",
          link: "/",
        },
        {
          id: 2,
          title: "Автопарк",
          link: "/autopark",
        },
        {
          id: 3,
          title: "О нас",
          link: "about",
        },
        {
          id: 4,
          title: "Контакты",
          link: "contacts",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "../styles/_variables.scss";

.header {
  &__wrapper {
    align-items: center;
    height: 100px;
    justify-content: space-between;
  }
  &__logo {
    img {
      height: 70px;
    }
  }
  &__nav {
    display: flex;
    align-items: center;
    &__item {
    }
    &__link {
      font-size: 18px;
      text-transform: uppercase;
      font-weight: bold;
      margin-left: 30px;
      transition: 0.5s;
      color: $green;
      &:hover {
        color: $yellow;
      }
    }
  }
}
</style>
