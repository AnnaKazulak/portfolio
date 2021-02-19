<template>
  <div id="app">
    <Home />
    <SocialMedia />
    <SideBar />
    <About />
    <Lebenslauf />
    <Skills />
    <Kontakt />
    <SocialMedia />
    <Footer />
  </div>
</template>

<script>
import Home from "./pages/home/Home";
import SideBar from "./pages/sidebar/SideBar";
import About from "./pages/about/About";
import SocialMedia from "./pages/about/SocialMedia";
import Lebenslauf from "./pages/lebenslauf/Lebenslauf";
import Kontakt from "./pages/kontakt/Kontakt";
import Skills from "./pages/skills/Skills";
import Footer from "./pages/footer/Footer";
export default {
  name: "App",
  components: {
    Home,
    SideBar,
    About,
    SocialMedia,
    Lebenslauf,
    Skills,
    Kontakt,
    Footer,
  },
};
</script>

<style>
#app {
  /* font-family: Avenir, Helvetica, Arial, sans-serif; */
  font-family: "Roboto Mono", monospace;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  margin: 0px;
}
html {
  scroll-behavior: smooth;
}
body {
  margin: 0px;
}
</style>
