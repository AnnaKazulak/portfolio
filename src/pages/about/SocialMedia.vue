<template>
  <div id="social-media-container">
    <div class="icons">
      <a
        href="https://www.linkedin.com/in/anna-kazulak-13a61a67/"
        target="_blank"
        ><img class="linkedin" src="../../assets/logo-linkedin.svg"
      /></a>
      <a
        href="https://www.xing.com/profile/Anna_Kazulak2/portfolio"
        target="_blank"
        ><img class="xing" src="../../assets/logo-xing.svg"
      /></a>
      <a href="#"><img class="github" src="../../assets/logo-github.svg"/></a>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style lang="css">
#social-media-container {
  display: block;
  background-color: rgba(229, 229, 229, 0.75);
  height: 5vh;
  padding: 2vh 0;
  text-align: center;
}

.icons {
  width: 100%;
  height: 100%;
}
.icons a img {
  height: 100%;
  margin: 0 10px;
  opacity: 0.7;
  transform: scale(0.9);
  transition: 300ms;
}
.icons img:hover {
  filter: none;
  transform: scale(1.2);
}
</style>
