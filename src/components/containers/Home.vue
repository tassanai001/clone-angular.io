<template>
  <div>
    <articlecmp></articlecmp>
  </div>
</template>

<script>
import Article from "@/components/Article";
export default {
  name: "Home",
  components: {
    articlecmp: Article
  },
  data() {
    return {
      msg: "Welcome to Your Vue.js App"
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
