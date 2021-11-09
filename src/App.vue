<template>
  <div id="app">
    <Header />
    <div>
      <section-1 />
      <section-2 />
      <section-3 />
      <section-4 />
      <section-5 />
    </div>
    <Footer />
  </div>
</template>

<script>

import Header from "./pages/header.vue";
import Footer from "./pages/footer.vue";
import Section1 from './pages/sections/section1.vue';
import Section2 from './pages/sections/section2.vue';
import Section3 from './pages/sections/section3.vue';
import Section4 from './pages/sections/section4.vue';
import Section5 from './pages/sections/section5.vue';

export default {
  name: "App",
  components: {
    Header,
    Footer,
    Section1,
    Section2,
    Section3,
    Section4,
    Section5,
  },
};
</script>