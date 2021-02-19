<template>
  <section id="skills">
    <div class="heading"><span>Skills</span></div>
    <div class="icons">
      <img src="../../assets/skills/js.svg" alt="" />
      <img src="../../assets/skills/sass.svg" alt="" />
      <img src="../../assets/skills/vue.svg" alt="" />
      <img src="../../assets/skills/bootstrap.svg" alt="" />
      <img src="../../assets/skills/figma.svg" alt="" />
      <img src="../../assets/skills/css3.svg" alt="" />
      <img src="../../assets/skills/xd.svg" alt="" />
      <img src="../../assets/skills/mysql.svg" alt="" />
    </div>
  </section>
</template>
<script>
export default {};
</script>
<style scoped>
#skills {
  font-family: "Roboto Mono", monospace;
  /* background-color: thistle; */
  padding-top: 8vh;
  padding-bottom: 10vh;
}
.icons {
  margin: 0 auto;
  margin-top: 15px;
  width: 60vw;
  opacity: 0.85;

  /* border: 2px solid tomato; */
}
.icons img {
  width: 100px;
  filter: saturate(0) contrast(3) brightness(0.5);
  transform: scale(0.9);
  transition: 300ms;
  margin-top: 20px;
}
.icons img:hover {
  filter: none;
  transform: scale(1);
}
</style>
