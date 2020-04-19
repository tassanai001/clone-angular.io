<template>
  <v-app>
    <div id="app">
      <div class="header__responsive--mobile">
        <appbarcmp>
          <headercmp></headercmp>
          <router-view />
          <footercmp></footercmp>
        </appbarcmp>
      </div>
      <div class="header__responsive--desktop">
        <appbarcmp></appbarcmp>
        <headercmp></headercmp>
        <router-view />
        <footercmp></footercmp>
      </div>
    </div>
  </v-app>
</template>

<script>
import Header from "@/components/Header";
import Footer from "@/components/Footer";
import Appbar from "@/components/Appbar";
export default {
  name: "App",
  components: {
    headercmp: Header,
    footercmp: Footer,
    appbarcmp: Appbar
  }
};
</script>

<style>
#app {
  font-family: "Roboto", "Helvetica Neue Light", "Helvetica Neue", "Helvetica",
    "Arial", "Lucida Grande", "sans-serif";
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
p {
  margin-bottom: unset !important;
}
/* .header__responsive--mobile {
  display: block;
}

.header__responsive--desktop {
  display: none;
} */

@media (max-width: 480px) {
  .header__responsive--mobile {
    display: block;
  }

  .header__responsive--desktop {
    display: none;
  }
}

@media (min-width: 481px) {
  .header__responsive--mobile {
    display: none;
  }

  .header__responsive--desktop {
    display: block;
  }
}
</style>
