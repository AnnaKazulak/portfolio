<template>
  <div class="click-area" @click="click">
    <div id="burger" :class="{ open }"></div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      open: false,
    };
  },
  methods: {
    click() {
      this.open = !this.open;
    },
  },
};
</script>

<style scoped>
.click-area {
  width: 50px;
  height: 50px;
  display: inline-block;
}
#burger {
  display: inline-block;
  width: 40px;
  height: 5px;
  background: black;
  position: relative;
  transition: 300ms;
}
/* #burger:hover::before::after {
  background-color: aqua;
} */
#burger:hover::after {
  background: #bc3a80;
}
#burger:hover {
  background: #bc3a80;
}
#burger:hover::before {
  background: #bc3a80;
}

#burger::before {
  content: "";
  display: inline-block;
  position: absolute;
  top: 15px;
  left: 0;
  width: 40px;
  height: 5px;
  background: black;
  transition: 200ms;
}
#burger::after {
  content: "";
  display: inline-block;
  position: absolute;
  top: 30px;
  left: 0;
  width: 40px;
  height: 5px;
  background: black;
  transition: 200ms;
}
#burger.open {
  background: transparent;
}
#burger.open::before {
  display: inline-block;
  width: 40px;
  top: 15px;
  height: 5px;
  background: black;
  position: absolute;
  transform: rotate(45deg);
}
#burger.open::after {
  display: inline-block;
  width: 40px;
  top: 15px;
  height: 5px;
  background: black;
  position: absolute;
  transform: rotate(-45deg);
}
</style>
