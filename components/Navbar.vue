<template>
  <nav>
    <v-toolbar flat dark :color="col">
      <a target="_blank" href="https://www.solidworks.com/">
        <!-- <v-img max-width="144px" :src="require('../assets/img/SWX.png')"></v-img>
        -->
        <v-img justify="center" height="33px" width="180px" :src="require('../assets/img/SWX.png')"></v-img>
      </a>
      <v-spacer></v-spacer>
    </v-toolbar>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      col: "#E31818",
      drawer: false,
      dialog: false,
      un: 3,
      updateText: [
        "Final product submission has been started. Submissions links has been emailed to all the participants.",
        "Final product submission ends on 31st August 2019.",
        "Announcing Zonal Rounds - Zonal qualifier rounds will happen in three zones Delhi, Ahmedabad and Chennai. For more details checkout Process section."
      ],
      Home: { icon: "fas fa-home", text: "Home", route: "/" },
      Process: { icon: "fas fa-cogs", text: "Process", route: "/Process" },
      Oldak: {
        icon: "fas fa-location-arrow",
        text: "Journey So Far",
        items: [
          { text: "AAKRUTI2018", route: "/Previous/18" },
          { text: "AAKRUTI2017", route: "/Previous/17" },
          { text: "AAKRUTI2016", route: "/Previous/16" }
        ]
      },
      Gallery: { icon: "fas fa-image", text: "Gallery", route: "/Gallery" }
    };
  }
};
</script>

<style scoped>
.thin {
  font-family: "3ds-light";
  font-size: 34px;
}
.para {
  font-size: calc(12px + 4 * ((100vw - 320px) / 880)) !important;
}
.fontz {
  font-size: calc(14px + 2.5 * ((100vw - 320px) / 880)) !important;
  font-family: "3ds";
  margin-bottom: 12px;
  line-height: 1.2;
  letter-spacing: -0.2px;
  color: #012d52;
  /* 757575 424242*/
}
.navtogglebg {
  background: #00345c;
  background: linear-gradient(
    180deg,
    #00345c 0%,
    rgba(2, 44, 67, 0.7) 100%
  ) !important;
  font-family: "3ds";
}
.hover {
  background-color: #1e6794;
}
.display-1 {
  font-family: "3ds" !important;
}
.fontbtn {
  font-family: "3ds" !important;
  font-size: 13px !important;
}
.fontz2 {
  font-size: calc(16px + 5 * ((100vw - 320px) / 880)) !important;
  font-family: "3ds-SemiBold";
  background-color: #014a7d;
}
.v-dialog__content--active {
  background-color: rgba(0, 0, 0, 0.5) !important;
}
</style>
