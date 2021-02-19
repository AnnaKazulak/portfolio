<template>
  <div>
    <section id="lebenslauf">
      <div class="heading" ref="contHeading">
        <span>Resume</span>
      </div>
      <div v-for="(item, index) in items" :key="index" class="row">
        <div class="subHeadingLeft">
          <p>{{ item.title }}</p>
        </div>
        <div class="column">
          <div
            class="station"
            v-for="(subitem, index) in item.subitems"
            :key="index"
          >
            <div class="resumeInhaltTime">{{ subitem.time }}</div>
            <div class="resumeInhaltFirm">{{ subitem.firm }}</div>
            <div class="resumeInhaltJob">{{ subitem.job }}</div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>
<script>
export default {
  data() {
    return {
      items: [
        {
          title: "Further Training",
          subitems: [
            {
              time: "2019-2021",
              firm: "CBM Projektmanagement",
              job: "Degree: Computer Science Expert. Software Development",
            },
          ],
        },
        {
          title: "Work Experience",
          subitems: [
            {
              time: "2020-2021",
              firm: "xpertnova GmbH",
              job: "Trainee: Junior Software Developer",
            },
            {
              time: "2013-2019",
              firm: "Amazon Logistik, Convergys, Webhelp, Agentur für Arbeit",
              job: "High Volume Hiring Recruiterin",
            },
          ],
        },
        {
          title: "Studies",
          subitems: [
            {
              time: "2014-2015",
              firm: "University in Hagen",
              job: " Business Administration. International Management",
            },
            {
              time: "2001-2006",
              firm: "Cardinal Stefan Wyszynski University",
              job:
                "Degree: Master in Political Science with a Focus on Social and Economic Policy",
            },
          ],
        },
      ],
    };
  },
  methods: {
    changeColor() {
      this.$refs.contHeading.classList.toggle("change");
    },
  },
};
</script>
<style lang="css">
#lebenslauf {
  padding-top: 5vh;
  /* height: 140vh; */
  width: 100%;
  justify-content: center;
  font-family: "Roboto Mono", monospace;
  background-color: #f8f8f8;
  padding-bottom: 10vh;
}

.heading {
  position: relative;
  width: 25vw;
  height: 4vw;
  border: 2px solid transparent;
  margin: 0 auto;
  padding-top: 10px;
  border-radius: 4px;
  border-image: linear-gradient(60deg, #bc3a80, #1762a7);
  border-image-slice: 1;
}

@media screen and (max-width: 600px) {
  .heading {
    width: 36vw;
    height: 6vw;
  }
  .heading span {
  }
}

.heading:hover {
  border: 2px solid #bc3a80;
}

.heading span {
  display: inline-block;
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
  color: black;
  font-size: 1.7rem;
  letter-spacing: 0.4rem;
}

.row {
  display: flex;
  width: 60vw;
  margin: 0 auto;
  margin-top: 7vh;
}

.subHeadingLeft {
  flex: 1;
  display: block;
  width: 30vw;
  text-align: center;
  font-size: 1.2vw;
  letter-spacing: 0.2rem;
  /* border: 2px solid tomato; */
}
.column {
  flex: 2;
  padding: 20px;
  border-left: 3px solid;
  border-left-color: cyan;
  border-left: 2px solid transparent;
  border-image: linear-gradient(180deg, #bc3a80, #1762a7) 1 100%;
  /* border: 2px solid tomato; */
}

.station {
  margin-bottom: 50px;
}

div .resumeInhaltTime {
  background-color: #1762a7;
  padding: 7px;
  margin-left: 10px;
  width: max-content;
  color: #fff;
}
div .resumeInhaltTime:hover {
  background-color: #bc3a80;
  transition: 300ms;
}

div .resumeInhaltFirm {
  padding: 10px;
  align-content: flex-start;
}

div .resumeInhaltJob {
  padding: 10px;
  justify-content: flex-start;
}

@media screen and (max-width: 1000px) {
  .row {
    width: 90vw;
    font-size: 2.5vw;
  }
  .subHeadingLeft {
    font-size: 2.5vw;
  }
}
</style>
