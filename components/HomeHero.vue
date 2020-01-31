<template>
  <v-container fluid class="home-hero px-0" style="height: 100vh;">
    <!-- <HomeSlides/> -->
    <v-row no-gutters style="margin-top: 15vh;">
      <v-col justify="center" align="center" class="white--text animated fadeInDown pb-5">
        <h1 class="fontz">
          AAKRUTI
          <span class="lightfont">2020</span>
        </h1>
        <h2 class="fontz2">Shaping Imagination</h2>
      </v-col>

      <!-- <v-btn
        outline
        large
        class="mt-5 animated fadeInDown"
        target="_blank"
        href="https://www.surveymonkey.com/r/7T7D2VH"
        round
        color="#E31818"
        style="border: 2px solid !important;"
      >Register Here</v-btn> -->
     <v-col justify="center" align="center" cols="12">
        <v-btn
        fab
        dark
        small
        class="mt-5 animated infinite bounce"
        color="#3DA9EB"
        @click="$vuetify.goTo('#first', options)"
      >
        <v-icon dark>fas fa-angle-down</v-icon>
      </v-btn>
     </v-col>
    </v-row>
  </v-container>
</template>

<script>


export default {
  name: "HomeHero",
  components: {
    
  },
  computed: {
    options() {
      return {
        duration: 600,
        offset: 5,
        easing: "easeInOutCubic"
      };
    }
  }
};
</script>

<style scoped>
.home-hero {
  background: url("../assets/img/bg.png") center;
  background-size: cover;
  width: 100%;
  height: 100%;
}

.fontz {
  font-size: calc(50px + 32 * ((100vw - 320px) / 880)) !important;
  font-family: "3ds-SemiBold";
  font-weight: 300;
  line-height: 1.5;
  letter-spacing: -0.2px;
}
.fontz2 {
  font-size: calc(24px + 12 * ((100vw - 320px) / 880)) !important;
  font-family: "3ds-light";
  font-weight: 300;
  line-height: 0.5;
  letter-spacing: -0.2px;
  text-align: center !important;
}
.lightfont {
  font-family: "3ds-light";
  font-weight: 300;
}
</style>
