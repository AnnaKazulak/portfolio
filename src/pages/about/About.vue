<template>
  <section id="about">
    <div class="container">
      <!-- <div class="initials">
        <h2>Anna Kazulak</h2>
        <h3 class="underline">Junior Frontend Developer</h3>
      </div> -->

      <div>
        <article class="text">
          I am a bubbly, outgoing, energetic, extraverted, practical, decisive,
          analytical, sympathetic, adapt as you go, imaginative, inspirational,
          sensible person. I am also hard working, dependable, positive,
          self-motivated, team-orientated, organized, work-well on the pressure,
          effective communicator, flexible and confident multitasker, strategist
          and independent-thinker. I love to learn and love to learn how to
          develop beautiful and functional software.
          <img
            class="profile-image mobile"
            src="../../assets/Bewerbungsphoto_Kwadrat.jpg"
            alt="profile"
          />
          <div class="wrapper">
            <span class="name">Anna Kazulak</span>
            <span class="profession">Junior Frontend Developer</span>
          </div>
        </article>

        <img
          class="profile-image"
          src="../../assets/Bewerbungsphoto_Kwadrat.jpg"
          alt="profile"
        />
      </div>
    </div>
  </section>
</template>
<script>
export default {};
</script>
<style lang="css">
#about {
  padding: 10vw;
  justify-content: center;
  align-items: center;
}
.container {
  margin-left: 11vw;
}

.initials {
  margin-left: 8vw;
}
/*
h2,
h3 {
  display: inline-block;
  margin: 0;
} */
/* h3 {
  margin-left: 15px;
} */

.wrapper {
  order: 1;
  display: flex;
  /* justify-items: self-end; */
  justify-content: flex-end;
  font-size: 1.17rem;
  font-weight: bolder;
  letter-spacing: 0.2rem;
}
.name,
.profession {
  margin-left: 15px;
}
div .text {
  display: flex;
  flex-direction: column;
  background: rgba(229, 229, 229, 0.75);
  width: 40vw;
  border-radius: 10px;
  padding: 20px;
  /* font-family: Arial, Helvetica, sans-serif; */
  /* font-family: "Comic Neue", cursive; */
  font-family: "Baloo 2", cursive;
  /* letter-spacing: 0.2rem; */
  font-size: 1vw;
  margin-left: 8vw;
}

img.profile-image {
  border-radius: 50%;
  width: 8vw;
}
img.profile-image.mobile {
  display: none;
}

@media screen and (max-width: 1500px) {
  div .text {
    width: 70vw;
    margin: 0;
    font-size: 100%;
    order: 1;
  }
  img.profile-image.mobile {
    display: inline-block;
  }
  img.profile-image {
    display: none;
  }
  .container {
    width: 100%;
    margin-left: 1vw;
    font-size: 2vw;
  }
  /* h2,
  h3 {
    font-size: 1.1rem;
  } */
}
@media screen and (max-width: 750px) {
  .name,
  .profession {
    font-size: 1.8vw;
  }
}
@media screen and (max-width: 650px) {
  div .text {
    width: 70vw;
    margin: 0;
    font-size: 100%;
    order: 1;
  }
  .container {
    width: 100%;
    margin-left: 1vw;
    font-size: 2vw;
  }
  .wrapper {
    max-width: 100%;
    display: flex;
    flex-direction: column;
  }
  .name,
  .profession {
    margin-left: 0;
  }
}
</style>
