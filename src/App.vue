<template>
  <div id="app">
    <Header />
    <Home />
    <About />
    <Skills />
    <Portfolio />
    <Contact />
    <Svgs />
    <Svgs-r />
  </div>
</template>

<script>
import Home from "./components/Home.vue";
import Header from "./components/Header.vue";
import About from "./components/About.vue";
import Skills from "./components/Skills.vue";
import Portfolio from "./components/Portfolio.vue";
import Contact from "./components/Contact.vue";
import Svgs from "./components/Svgs.vue";
import SvgsR from "./components/SvgsR.vue";

export default {
  name: "App",
  components: {
    Home,
    Header,
    About,
    Skills,
    Portfolio,
    Contact,
    Svgs,
    SvgsR,
  },
};
</script>

<style>
#app {
  z-index: 10;
  background-color: #daf0fc;
  margin: 0px 150px;
  margin-bottom: 50px;
}
body {
  background-color: #152837;
}
* {
  margin: 0px;
  padding: 0px;
}
</style>
