<template>
  <div id="app">
    <Header />
    <Main />
    <Footer />
    <!-- <Nav class="mb-6" />
    <HelloWorld msg="Welcome to Your Vue.js App" class="text-center"/> -->
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import Nav from './components/Nav.vue'
import Main from "./pages/main.vue";
import Header from "./pages/header.vue";
import Footer from "./pages/footer.vue";

export default {
  name: "App",
  components: {
    Main,
    Header,
    Footer,
    // HelloWorld,
    // Nav
  },
};
</script>