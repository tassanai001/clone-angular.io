<template>
  <div>
    <div class="header__responsive--desktop">
      <div class="background-sky hero" />
      <v-app-bar color="transparent accent-4" elevation="0" dense dark height="64">
        <v-app-bar-nav-icon class="appbar__toolber--ham" style="color:white; margin: 0 8px 0 0;"></v-app-bar-nav-icon>

        <v-toolbar-title style="padding-left: unset;" class="appbar__toolber--logo">
          <img :src="shieldLargeLogo" width="37" height="40" style="display:flex;" />
        </v-toolbar-title>

        <v-toolbar-title class="appbar__toolber">
          <img :src="navlogo" width="150" height="40" />
        </v-toolbar-title>
        <v-toolbar-title style="padding-left: 20px;" class="appbar__toolber">
          <v-btn text>
            <span class="toolbar__btn--margin">Features</span>
          </v-btn>
        </v-toolbar-title>
        <v-toolbar-title class="appbar__toolber">
          <v-btn text>
            <span class="toolbar__btn--margin">Docs</span>
          </v-btn>
        </v-toolbar-title>
        <v-toolbar-title class="appbar__toolber">
          <v-btn text>
            <span class="toolbar__btn--margin">Resources</span>
          </v-btn>
        </v-toolbar-title>
        <v-toolbar-title class="appbar__toolber">
          <v-btn text>
            <span class="toolbar__btn--margin">Events</span>
          </v-btn>
        </v-toolbar-title>
        <v-toolbar-title class="appbar__toolber">
          <v-btn text>
            <span class="toolbar__btn--margin">Blog</span>
          </v-btn>
        </v-toolbar-title>

        <v-spacer></v-spacer>

        <input class="toolbar__search" type="text" name="search" placeholder="Search.." />

        <v-btn icon>
          <v-icon>mdi-twitter</v-icon>
        </v-btn>
        <v-btn icon>
          <v-icon>mdi-gitlab</v-icon>
        </v-btn>
      </v-app-bar>
    </div>

    <div class="header__responsive--mobile">
      <v-card class="overflow-hidden appbar__card--container">
        <div class="background-sky hero" />
        <v-app-bar
          absolute
          elevate-on-scroll
          scroll-target="#scrolling-techniques-7"
          class="appba__appbar--container"
        >
          <v-app-bar-nav-icon
            class="header__responsive--iconbtn"
            style="color:white; margin: 0 8px 0 0;"
          ></v-app-bar-nav-icon>

          <v-toolbar-title style="padding-left: unset;">
            <img :src="shieldLargeLogo" width="37" height="40" style="display:flex;" />
          </v-toolbar-title>

          <v-spacer></v-spacer>

          <input class="toolbar__search" type="text" name="search" placeholder="Search.." />

          <v-btn icon class="header__responsive--iconbtn">
            <v-icon style="color:white;">mdi-twitter</v-icon>
          </v-btn>
          <v-btn icon class="header__responsive--iconbtn">
            <v-icon style="color:white;">mdi-gitlab</v-icon>
          </v-btn>
        </v-app-bar>
        <v-sheet id="scrolling-techniques-7" class="overflow-y-auto">
          <v-container style="padding: unset; height: 100vh;">
            <slot></slot>
          </v-container>
        </v-sheet>
      </v-card>
    </div>
  </div>
</template>

<script>
export default {
  name: "Appbar",
  components: {},
  data() {
    return {
      msg: "Welcome to Your Vue.js App",
      navlogo: require("@/assets/images/logo-nav@2x.png"),
      logo: require("@/assets/images/angular.svg"),
      shieldLargeLogo: require("@/assets/images/shield-large.svg")
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.toolbar__btn--margin {
  margin: 0 4px;
}

.appbar__card--container {
  border-radius: unset;
}

@media (max-width: 480px) {
  .header__responsive--iconbtn {
    width: 40px !important;
  }

  .header__responsive--mobile {
    display: block;
  }

  .header__responsive--desktop {
    display: none;
  }

  .toolbar__search {
    background: white;
    border-radius: 20px;
    padding: 5px;
    font-size: 11px;
    font-size: 0.9rem;
  }
  .appba__appbar--container {
    background-color: #1976d2 !important;
    border-radius: unset;
  }

  .hero {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    position: absolute;
    width: 100%;
    min-height: 480px;
    height: 80vh;
    max-height: 490px;
    box-sizing: border-box;
    padding: 48px 48px 32px;
    overflow: hidden;
    transform: skewY(0deg);
    transform-origin: 100%;
  }

  .appbar__toolber--logo {
    display: none;
  }
  .appbar__toolber--hum {
    display: none;
  }
}

@media (min-width: 481px) and (max-width: 768px) {
  .appbar__toolber--logo {
    display: block;
  }

  .appbar__toolber--hum {
    display: block;
  }
  .background-sky {
    background: linear-gradient(145deg, #0d47a1, #42a5f5);
    color: #fff;
  }
  .appbar__toolber {
    display: none;
  }
  .hero {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    position: absolute;
    width: 100%;
    min-height: 480px;
    height: 80vh;
    max-height: 560px;
    box-sizing: border-box;
    padding: 48px 48px 32px;
    overflow: hidden;
    transform: skewY(8deg);
    transform-origin: 100%;
  }

  .header__responsive--mobile {
    display: none;
  }

  .header__responsive--desktop {
    display: block;
  }

  .toolbar__search {
    background: white;
    border-radius: 20px;
    padding: 5px;
    font-size: 11px;
    font-size: 0.9rem;
  }
  .appba__appbar--container {
    background-color: transparent !important;
    border-radius: unset;
  }
}

@media (min-width: 769px) and (max-width: 1024px) {
  .appbar__toolber--ham {
    display: block;
  }
  .appbar__toolber {
    display: none;
  }
  .background-sky {
    background: linear-gradient(145deg, #0d47a1, #42a5f5);
    color: #fff;
  }
  .appbar__toolber--logo {
    display: block;
  }
  .appbar__toolber--hum {
    display: none;
  }
  .hero {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    position: absolute;
    width: 100%;
    min-height: 480px;
    height: 80vh;
    max-height: 560px;
    box-sizing: border-box;
    padding: 48px 48px 32px;
    overflow: hidden;
    transform: skewY(8deg);
    transform-origin: 100%;
  }
  .header__responsive--mobile {
    display: none;
  }

  .header__responsive--desktop {
    display: block;
  }

  .toolbar__search {
    background: white;
    color: #444;
    border-radius: 20px;
    padding: 5px 16px;
    font-size: 11px;
    width: 180px;
    height: 32px;
    font-size: 0.9rem;
  }
}

@media (min-width: 1025px) {
  .appbar__toolber--ham {
    display: none;
  }
  .background-sky {
    background: linear-gradient(145deg, #0d47a1, #42a5f5);
    color: #fff;
  }
  .appbar__toolber--logo {
    display: none;
  }
  .appbar__toolber--hum {
    display: none;
  }
  .hero {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    position: absolute;
    width: 100%;
    min-height: 480px;
    height: 80vh;
    max-height: 560px;
    box-sizing: border-box;
    padding: 48px 48px 32px;
    overflow: hidden;
    transform: skewY(8deg);
    transform-origin: 100%;
  }
  .header__responsive--mobile {
    display: none;
  }

  .header__responsive--desktop {
    display: block;
  }

  .toolbar__search {
    background: white;
    color: #444;
    border-radius: 20px;
    font-size: 11px;
    width: 180px;
    height: 32px;
    padding: 5px 16px;
    font-size: 0.9rem;
  }
}
</style>
