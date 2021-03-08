<template>
  <div>
    <footer>
      <!-- <span class="copyright">&copy;</span> -->
      <img class="copyright" src="../../assets/copyright.svg" />
      <span> 2021 created by Anna Kazulak</span>
    </footer>
  </div>
</template>
<script>
export default {};
</script>
<style lang="css" scoped>
div {
  background-color: rgb(36, 36, 36);
  display: flex;
  height: 10vh;
  /* align-content: center; */
  justify-content: center;
  /* height: 50vh; */
}

.copyright {
  width: 17px;
  height: 17px;
  padding-top: 10px;
  filter: invert(100%);
}
span {
  color: whitesmoke;
}
</style>
