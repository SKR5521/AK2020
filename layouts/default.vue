<template>
  <div class="body-all" id="body">
    <!-- App.vue -->
    <v-app>
      <!-- <v-navigation-drawer app>
        
      </v-navigation-drawer>-->

      <v-app-bar>
        <v-container fluid>
          <v-row>
            <v-col>
              <a target="_blank" href="https://www.3ds.com/">
                <v-img max-width="120px" :src="require('../assets/img/DS1.png')"></v-img>
              </a>
            </v-col>
            <v-spacer></v-spacer>
            <v-col justify="end">
              <v-row>
                <v-spacer></v-spacer>
                <a target="_blank" href="/">
                  <v-img max-width="120px" :src="require('../assets/img/logo.png')"></v-img>
                </a>
              </v-row>
            </v-col>
          </v-row>
        </v-container>
      </v-app-bar>
      <Navbar />

      <!-- Sizes your content based upon application components -->
      <v-content>
        <!-- Provides the application the proper gutter -->

        <nuxt />
        <v-container class="hidden-sm-and-up">
          <v-row>
            <v-col justify="center" align="center">
              <v-btn color="#012D52" class="fontzd" rounded fab small dark v-on:click="Top">
                <v-icon>fas fa-angle-up</v-icon>
              </v-btn>
            </v-col>
          </v-row>
        </v-container>
      </v-content>

      <v-footer padless absolute app style="background-color: #E31818 !important;">
        <v-container fluid class="hidden-xs-only ma-0 pa-0">
          <v-row class="px-4">
            <v-col cols="12" sm="4" align="start">
              <v-img
                justify="center"
                height="33px"
                width="180px"
                :src="require('../assets/img/SWX.png')"
              ></v-img>
            </v-col>

            <v-col cols="12" sm="8" align="end">
              <div>
                <v-btn
                  v-for="item in items"
                  :key="item.icon"
                  class="mx-4 white--text"
                  dark
                  target="_blank"
                  icon
                  :href="item.ref"
                >
                  <v-icon>{{ item.icon }}</v-icon>
                </v-btn>
              </div>
            </v-col>
          </v-row>
          <!-- <Footer/> -->
          <v-row class="grey darken-4 white--text text-lighten-2">
            <v-col align="center" cols="12" sm="6" class="caption">
              {{ new Date().getFullYear() }} —
              <span>Dassault Systèmes SOLIDWORKS Corporation</span>
            </v-col>
            <v-col align="center" cols="12" sm="6">
              <ul class="list-inline">
                <li v-for="link in Links" :key="link.text">
                  <a class="caption" :href="link.ref" target="_blank">{{link.text}}</a>
                </li>
              </ul>
            </v-col>
          </v-row>
        </v-container>

        <v-container fluid class="hidden-sm-and-up ma-0 pa-0">
          <v-row>
            <v-col cols="12" sm="4" align="center">
              <v-img
                justify="center"
                height="33px"
                width="180px"
                :src="require('../assets/img/SWX.png')"
              ></v-img>
            </v-col>

            <v-col cols="12" sm="8" align="center">
              <v-spacer></v-spacer>
              <div>
                <v-btn
                  v-for="item in items"
                  :key="item.icon"
                  class="mx-4 white--text"
                  dark
                  target="_blank"
                  icon
                  :href="item.ref"
                >
                  <v-icon>{{ item.icon }}</v-icon>
                </v-btn>
              </div>
            </v-col>
          </v-row>
          <!-- <Footer/> -->
          <v-row class="grey darken-4 white--text text-lighten-2">
            <v-col align="center" cols="12" sm="6" class="caption pb-0">
              {{ new Date().getFullYear() }} —
              <span>Dassault Systèmes SOLIDWORKS Corporation</span>
            </v-col>
            <v-col align="center" class="pt-0" cols="12" sm="6">
              <ul class="list-inline">
                <li v-for="link in Links" :key="link.text">
                  <a class="caption" :href="link.ref" target="_blank">{{link.text}}</a>
                </li>
              </ul>
            </v-col>
          </v-row>
        </v-container>
      </v-footer>
    </v-app>
  </div>
</template>

<script>
import Navbar from "@/components/Navbar";

export default {
  components: {
    Navbar
  },
  data() {
    return {
      items: [
        {
          icon: "fab fa-facebook",
          ref: "https://www.facebook.com/AakrutiContest/"
        },
        {
          icon: "fab fa-linkedin",
          ref: "https://www.linkedin.com/showcase/solidworks/"
        },
        {
          icon: "fab fa-twitter",
          ref: "https://twitter.com/solidworks"
        },
        {
          icon: "fab fa-youtube",
          ref: "https://www.youtube.com/solidworks"
        }
      ],
      Links: [
        {
          text: "Terms of Use",
          ref: "https://www.solidworks.com/terms-use"
        },
        {
          text: "Privacy Policy",
          ref: "https://www.solidworks.com/privacy-policy"
        },
        {
          text: "Piracy Prevention",
          ref: "https://www.3ds.com/piracy/"
        },
        {
          text: "License Agreement",
          ref: "https://www.solidworks.com/license-agreement"
        }
      ]
    };
  },
  methods: {
    Top() {
      window.scrollTo({
        top: 0,
        left: 0,
        behavior: "smooth"
      });
    }
  }
};
</script>

<style >
.body-all {
  margin: 0;
  padding: 0;
  font-size: 16px;
  font-family: "3ds", sans-serif;
  text-align: justify !important;
  /* DCDCDC   dbdbdb */
  background-color: #F1F1F1;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-rendering: optimizeLegibility;
}

.list-inline {
  padding-left: 0 !important;
  list-style: none;
}
a {
  cursor: pointer;
  text-decoration: none;
  color: rgba(255, 255, 255, 0.64) !important;
}
a:hover {
  color: rgba(255, 255, 255, 0.9) !important;
}

.list-inline li {
  position: relative;
  color: rgba(255, 255, 255, 0.64) !important;
  display: inline-block !important;
  margin: 0 5px;
}

@font-face {
  font-family: "3ds";
  src: url("https://ui.3ds.com/fonts/3ds/3ds-Regular-v2.woff2") format("woff2");
}

@font-face {
  font-family: "3ds-light";
  src: url("https://ui.3ds.com/fonts/3ds/3ds-Light-v2.woff2") format("woff2");
}

@font-face {
  font-family: "3ds-SemiBold";
  src: url("https://ui.3ds.com/fonts/3ds/3ds-SemiBold-v2.woff2") format("woff2");
}
</style>
