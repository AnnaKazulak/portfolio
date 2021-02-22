<template>
  <section id="kontakt">
    <!-- <div class="heading"><span class="kontakt">Projects</span></div> -->

    <!-- <h2 class="heading-text">
      Wenn Sie noch fragen haben stehe ich ihnen gerne zur Verfügung.
    </h2> -->
    <!-- <div class="container">
      <form class="formular">
        <input type="text" class="input input-name " />
        <input type="text" class="input input-email " />
        <input type="text" class="input input-thema " />
        <input type="text" class="input input-nachricht " />
        <input type="submit" value="Submit" />
      </form>
    </div>  -->
  </section>
</template>
<script>
export default {};
</script>
<style lang="css">
/* #kontakt {
  display: flex;
  flex-direction: column;
  padding-top: 5vh;
  height: 95vh;
  background-color: rgb(15, 15, 15);
  justify-content: center;
  align-items: center;
  font-family: "Roboto Mono", monospace;
}
*/
#kontakt {
  display: flex;
  flex-direction: column;
  padding-top: 5vh;
  height: 40vh;
  background-color: #f8f8f8;
  background-image: url("../../assets/Hamburg_Hafen_1_klein.jpg");
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-position: top center;
  background-size: cover;
}

@media screen and (max-width: 1000px) {
  #kontakt {
    background-position: center;
  }
}

/* .container {
  display: flex;
  height: 30vh;
  background-color: teal;
}

.heading-text {
  display: flex;
  flex-direction: column;
  font-size: 1rem;
  font-weight: 300;

  padding-bottom: 15px;
  color: whitesmoke;
} */
</style>
