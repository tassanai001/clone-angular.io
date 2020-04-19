<template>
  <div>
    <div class="header__intro">
      <img :src="logo" class="header__intro--img" />
      <div class="header__intro--container">
        <div class="header__intro--text">
          One framework.
          <br />Mobile &amp; desktop.
        </div>
        <div class="header__intro--btncontainer">
          <v-btn depressed large rounded color="white" elevation="3" class="header__intro--btn">
            <span class="header__introbtn--text">Get Started</span>
          </v-btn>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
  components: {},
  data() {
    return {
      msg: "Welcome to Your Vue.js App",
      logo: require("@/assets/images/angular.svg")
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@media (max-width: 480px) {
  .header__intro {
    display: none;
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
    height: 100%;
    margin: 0 auto -32px;
    padding: 48px 0 0;
    color: #fff;
    flex-direction: column;
    background-color: #1976d2;
    background: linear-gradient(145deg, #0d47a1, #42a5f5);
    color: #fff;
  }

  .header__intro--text {
    font-size: 32px;
    font-size: 2rem;
    line-height: 50px;
    line-height: 3rem;
    margin: 20px 0px 50px 0px;
  }

  .header__introbtn--text {
    font-size: 1rem;
    color: #1976d2;
  }

  .header__intro--container {
    text-align: center;
  }

  .header__intro--img {
    height: 250px;
    widows: 250px;
  }

  .header__intro--btncontainer {
    position: relative;
    display: flex;
    justify-content: center;
  }

  .header__intro--btn {
    position: absolute;
    bottom: -20px;
  }
}

@media (min-width: 481px) and (max-width: 768px) {
  .header__intro--btncontainer {
    text-align: center;
  }

  .header__intro {
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
    height: 480px;
    margin: 0 auto -32px;
    color: #fff;
    flex-direction: column;
  }

  .header__intro--text {
    font-size: 32px;
    margin: 32px 0px;
  }

  .header__introbtn--text {
    font-size: 1rem;
    color: #1976d2;
  }

  .header__intro--container {
    text-align: start;
  }
  .header__intro--img {
    height: 400px;
    widows: 400px;
  }
}

@media (min-width: 769px) and (max-width: 1024px) {
  .header__intro {
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
    /* width: 900px; */
    height: 480px;
    margin: 0 auto -32px;
    padding: 48px 0 0;
    color: #fff;
  }

  .header__intro--text {
    font-size: 2.5rem;
    margin: 32px 0px;
  }

  .header__introbtn--text {
    font-size: 1rem;
    color: #1976d2;
  }

  .header__intro--container {
    text-align: start;
  }

  .header__intro--img {
    height: 400px;
    widows: 400px;
  }
}

@media (min-width: 1025px) {
  .header__intro {
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
    /* width: 900px; */
    height: 480px;
    margin: 0 auto -32px;
    padding: 48px 0 0;
    color: #fff;
  }

  .header__intro--text {
    font-size: 2.5rem;
    margin: 32px 0px;
  }

  .header__introbtn--text {
    font-size: 1rem;
    color: #1976d2;
  }

  .header__intro--container {
    text-align: start;
  }

  .header__intro--img {
    height: 400px;
    widows: 400px;
  }
}
</style>
