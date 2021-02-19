<template>
  <section id="about">
    <div class="container">
      <div class="initials">
        <h2>Anna Kazulak</h2>
        <h3 class="underline">Junior Frontend Developer</h3>
      </div>

      <div>
        <article class="text">
          I am a bubbly, outgoing, energetic, extraverted, practical, decisive,
          analytical, sympathetic, adapt as you go, imaginative, inspirational,
          sensible person. I am also hard working, dependable, positive,
          self-motivated, team-orientated, organized, work-well on the pressure,
          effective communicator, flexible and confident multitasker, strategist
          and independent-thinker. I love to learn and love to learn how to
          develop beautiful and functional software.
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

h2,
h3 {
  display: inline-block;
  margin: 0;
}
h3 {
  margin-left: 15px;
}

div .text {
  background: rgba(229, 229, 229, 0.75);
  width: 40vw;
  border-radius: 10px;
  padding: 20px;
  font-family: Arial, Helvetica, sans-serif;
  margin-left: 8vw;
}

img.profile-image {
  border-radius: 50%;
  width: 8vw;
}
</style>
