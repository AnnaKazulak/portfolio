<template>
  <div id="cont" ref="cont">
    <div class="menu-btn" @click="showSideBar">
      <Burger />
    </div>
    <div class="sidebar">
      <div class="photo-small">
        <img src="../../assets/Bewerbungsphoto_Kwadrat.jpg" alt="" />
      </div>

      <nav class="item-list">
        <a data-scroll href="#home">
          <!-- <i><BIconArrowUp /></i> -->
          <i><BIconHouseDoor /></i>

          <!-- <i><b-icon icon="house-door" style="color: #7952b3;"></b-icon> </i> -->
          <span class="sidebar-menu">Home</span>
        </a>
        <a data-scroll href="#about">
          <!-- <i><b-icon icon="person"></b-icon></i> -->
          <i> <BIconPerson /></i>
          <span class="sidebar-menu">About</span>
        </a>
        <a href="#lebenslauf">
          <!-- <i> <b-icon icon="file-earmark-text"></b-icon> </i> -->
          <i> <BIconFileEarmarkText /> </i>
          <span class="sidebar-menu">Resume</span>
        </a>
        <a href="#skills">
          <!-- <i><b-icon icon="code-slash"></b-icon> </i> -->
          <i><BIconCodeSlash /> </i>
          <span class="sidebar-menu">Skills</span>
        </a>
        <!-- <a href="#kontakt"> -->
        <!-- <i><b-icon icon="envelope-open"></b-icon> </i> -->
        <!-- <i><BIconEnvelopeOpen /> </i>
          <span class="sidebar-menu">Projects</span>
        </a> -->
      </nav>
      <SocialMedia />
    </div>
  </div>
</template>
<script>
import Burger from "./Burger";
import SocialMedia from "../../pages/about/SocialMedia";
export default {
  components: {
    Burger,
    SocialMedia,
  },
  methods: {
    showSideBar() {
      this.$refs.cont.classList.toggle("open");
    },
  },
};
</script>
<style lang="css">
#cont {
  position: fixed;
  top: 0;
  right: 0;
  width: calc(17vw + 65px);
  transform: translateX(17vw);
  transition: 1s;
  z-index: 5;
}

.sidebar {
  display: inline-block;
  width: 17vw;
  height: 100vh;
  background-color: #e5e5e5;
  opacity: 0.85;
  position: absolute;
  right: 0;
}

@media screen and (max-width: 1500px) {
  .sidebar {
    width: 25vw;
  }

  #cont {
    width: calc(25vw + 65px);
    transform: translateX(25vw);
  }
}
@media screen and (max-width: 650px) {
  .sidebar {
    width: 65vw;
  }

  #cont {
    width: calc(65vw + 65px);
    transform: translateX(65vw);
  }
  .menu.btn {
    margin-right: 5px;
  }

  .photo-small img {
    display: flex;
    width: 200px;
  }
}
@media (min-width: 650px) and (max-width: 1000px) {
  .sidebar {
    width: 55vw;
  }

  #cont {
    width: calc(55vw + 65px);
    transform: translateX(55vw);
  }
  .photo-small img {
    width: 30vw;
  }
}

.menu-btn {
  display: inline-block;
  position: absolute;
  left: 0;
  top: 0;
  width: 50px;
  margin-right: 15px;
  margin-top: 15px;
  color: red;
  height: 80px;
  cursor: pointer;
  transition: all 0.5s ease-in-out;
}
#cont.open {
  height: 100vh;
  display: inline-block;
  transform: translateX(0);
}
.photo-small {
  display: flex;
  width: 100%;
  justify-content: center;
  align-items: center;
  margin-top: 20px;
}

.photo-small img {
  display: flex;
  width: 13vw;
  border-radius: 50%;
  /* align-items: center; */
  justify-content: center;
}

nav a {
  display: flex;
  width: 100%;
  text-decoration: none;
  font-family: "Roboto Mono", monospace;
  font-size: 1.7rem;
  letter-spacing: 0.4rem;
  padding-top: 5vh;
  padding-left: 1vw;
  color: black;
}

.item-list i {
  padding-right: 1vw;
}

.item-list a:hover {
  color: #bc3a80;
}
</style>
