<template>
  <div id="app">
    <Header />
    <router-view />
  </div>
</template>

<script>
import Header from "./components/headerPage.vue";
export default {
  components: {
    Header,
  },
};
</script>

<style lang="scss">
@import "./styles/global.scss";

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  text-decoration: none;
  color: inherit;
  list-style: none;
  font-family: "Roboto"
}

nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
