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
/* width */
::-webkit-scrollbar {
  width: 10px;
}

/* Track */
::-webkit-scrollbar-track {
  background: #f1f1f1;
}

/* Handle */
::-webkit-scrollbar-thumb {
  background: #1762a7;
  /* background: linear-gradient(180deg, #bc3a80, #1762a7); */
  border-radius: 10px;
}

/* Handle on hover */
::-webkit-scrollbar-thumb:hover {
  background: #bc3a80;
  cursor: pointer;
}

html {
  scroll-behavior: smooth;
}
body {
  margin: 0px;
}
</style>
