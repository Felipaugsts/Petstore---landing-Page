<template>
  <div>
    <Navbar />
    <router-view />
    <Footer />
  </div>
</template>
<script>
import Navbar from "../src/components/TheNavigationBar.vue";
import Footer from "../src/components/AppFooter.vue";
export default {
  components: {
    Navbar,
    Footer,
  },
};
</script>
<style>
@import url("https://fonts.googleapis.com/css2?family=Inter:wght@500&display=swap");
@import url("./assets/css/navibar.css");
@import url("./assets/css/responsive.css");
</style>
