<template>
  <section id="home">
    <div class="text-box in">
      <h2 class="heading-primary">
        <span class="heading-primar--main">Welcome</span>
        <span class="heading-primar--sub">to my frontend world</span>
      </h2>
    </div>
  </section>
</template>
<script>
export default {};
</script>
<style lang="css">
/* * {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
} */
#home {
  font-family: "Roboto Mono", monospace;
  display: flex;
  padding: 10vw;
  height: 50vh;
  /* background-color: rgb(15, 15, 15); */
  /* background-image: url(../../assets/Hamburg_Hafen_1.jpeg); */
  background-image: url("../../assets/Hamburg_Hafen_1.jpeg");
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-position: center;
  background-size: cover;
}

.heading-primary {
  color: whitesmoke;
  text-transform: uppercase;
}
.heading-primar--main {
  display: block;
  font-size: 5rem;
  font-weight: 400;
  letter-spacing: 1.5rem;
  padding-left: 20px;
  padding-top: 15px;
}

.heading-primar--sub {
  display: block;
  font-size: 1rem;
  font-weight: 300;
  letter-spacing: 0.9rem;
  padding-bottom: 15px;
  padding-left: 20px;
}

/* animation */
.text-box {
  position: absolute;
  border-radius: 4px;
  animation: intro 1s 1s ease-in-out forwards;
}
.text-box:after {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  border-radius: 4px;
  /* background: linear-gradient(120deg, #00f260, #0575e6, #00f260); */
  background: linear-gradient(120deg, #bc3a80, #1762a7, #bc3a80);
  background-size: 300% 300%;
  clip-path: polygon(
    0% 100%,
    3px 100%,
    3px 3px,
    calc(100% - 3px) 3px,
    calc(100% - 3px) calc(100% - 3px),
    3px calc(100% - 3px),
    3px 100%,
    100% 100%,
    100% 0%,
    0% 0%
  );
}

.text-box.in:after {
  animation: frame-enter 1s forwards ease-in-out reverse,
    gradient-animation 4s ease-in-out infinite;
}

/* motion */
@keyframes gradient-animation {
  0% {
    background-position: 15% 0%;
  }
  50% {
    background-position: 85% 100%;
  }
  100% {
    background-position: 15% 0%;
  }
}

@keyframes frame-enter {
  0% {
    clip-path: polygon(
      0% 100%,
      3px 100%,
      3px 3px,
      calc(100% - 3px) 3px,
      calc(100% - 3px) calc(100% - 3px),
      3px calc(100% - 3px),
      3px 100%,
      100% 100%,
      100% 0%,
      0% 0%
    );
  }
  25% {
    clip-path: polygon(
      0% 100%,
      3px 100%,
      3px 3px,
      calc(100% - 3px) 3px,
      calc(100% - 3px) calc(100% - 3px),
      calc(100% - 3px) calc(100% - 3px),
      calc(100% - 3px) 100%,
      100% 100%,
      100% 0%,
      0% 0%
    );
  }
  50% {
    clip-path: polygon(
      0% 100%,
      3px 100%,
      3px 3px,
      calc(100% - 3px) 3px,
      calc(100% - 3px) 3px,
      calc(100% - 3px) 3px,
      calc(100% - 3px) 3px,
      calc(100% - 3px) 3px,
      100% 0%,
      0% 0%
    );
  }
  75% {
    -webkit-clip-path: polygon(
      0% 100%,
      3px 100%,
      3px 3px,
      3px 3px,
      3px 3px,
      3px 3px,
      3px 3px,
      3px 3px,
      3px 0%,
      0% 0%
    );
  }
  100% {
    -webkit-clip-path: polygon(
      0% 100%,
      3px 100%,
      3px 100%,
      3px 100%,
      3px 100%,
      3px 100%,
      3px 100%,
      3px 100%,
      3px 100%,
      0% 100%
    );
  }
}
@keyframes intro {
  0% {
    background-color: transparent;
    backdrop-filter: blur(0px);
  }
  100% {
    background-color: rgba(0, 0, 0, 0.1);
    backdrop-filter: blur(10px);
  }
}

@media screen and (max-width: 1000px) {
  .heading-primar--main {
    font-size: 15vw;
    letter-spacing: 0.5rem;
    padding-right: 20px;
  }
  .heading-primar--sub {
    font-size: 6.25vw;
    letter-spacing: 0;
    padding-right: 20px;
  }
  .text-box {
    position: absolute;
    left: 50vw;
    top: 25vh;
    transform: translate(-50%, -50%);
  }
}
</style>
