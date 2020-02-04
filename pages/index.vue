<template>
  <div>
    <Homehero />

    <div class="py-5 back">
      <v-container id="first">
        <v-row row>
          <v-col cols="12">
            <p
              data-aos="zoom-in-up"
              class="fontz py-1 mb-0 font-italic"
              v-for="item in about"
              :key="item"
            >{{ item }}</p>
          </v-col>
        </v-row>
      </v-container>
    </div>

    <Theme />

    <v-container>
      <v-row justify="center" align="center">
        <v-col cols="12" sm="4">
          <v-img class="mx-auto" max-width="250px" :src="require('../assets/img/think.svg')"></v-img>
        </v-col>
        <v-col cols="12" sm="8">
          <p
            class="bottomtext mb-0 text-wrap py-2"
          >Wear your 'Thinking Hat' and start thinking about themes & product which you want to design and gear up to participate in AAKRUTI 2020.</p>
        </v-col>
      </v-row>

      <v-row justify="center" align="center">
        <v-col cols="12" sm="8">
          <p
            class="bottomtext mb-0 text-wrap py-2"
          >Brain storm with your buddies and come up with Innovative project that makes a difference and prepare write-up for your concept. Once the registration window opens, you will be able to submit your registration quickly.</p>
        </v-col>

        <v-col cols="12" sm="4">
          <v-img class="mx-auto" max-width="250px" :src="require('../assets/img/think2.svg')"></v-img>
        </v-col>
      </v-row>
      <v-row>
        <v-col cols="12">
          <p
            class="bottomtext mb-0 text-wrap py-2"
          >Registration open soon in March 2020 first week. Stay tuned for AAKRUTI website and FaceBook Page.</p>
        </v-col>
      </v-row>
    </v-container>

    <!-- <v-layout row wrap justify-center align-center>
        <v-flex xs12 md3 class="pa-1">
          <zonecard Tname = 'ARG-Bots' Tid='10913396847' member1='gyan' member2='bharat' college='Narsi Munji pune'/>
        </v-flex>
      <v-flex xs12 md3 class="pa-1">
          <zonecard Tname = 'ARG-Bots' Tid='10913396847' member1='gyan' member2='bharat' college='Narsi Munji pune'/>
        </v-flex>
        <v-flex xs12 md3 class="pa-1">
          <zonecard Tname = 'ARG-Bots' Tid='10913396847' member1='gyan' member2='bharat' college='Narsi Munji pune'/>
        </v-flex>
        <v-flex xs12 md3 class="pa-1">
          <zonecard Tname = 'ARG-Bots' Tid='10913396847' member1='gyan' member2='bharat' college='Narsi Munji pune'/>
        </v-flex>
    </v-layout>-->
    <!-- <v-layout row wrap>
        <v-flex class="px-1 py-2" xs12 md4 justify-center text-xs-center>
          <v-card class="bord" height="100%">
            <v-card-text text-xs-center>
              <h1 class="fontz22 pb-3">ZONE 1 - NORTH - DELHI</h1>
              <p
                class="fontz"
              >UT-Delhi, Jammu & Kashmir, Haryana, Punjab, Himachal Pradesh, Uttar Pradesh, Uttarakhand, Rajasthan, West Bengal, Bihar, UT-Chandigarh, Arunachal Pradesh, Assam, Meghalaya, Manipur, Nagaland, Tripura, Jharkhand, Sikkim, Odisha</p>
            </v-card-text>
          </v-card>
        </v-flex>
        <v-flex class="px-1 py-2" xs12 md4 justify-center text-xs-center>
          <v-card class="bord" height="100%">
            <v-card-text text-xs-center>
              <h1 class="fontz22 pb-3">ZONE 2 - SOUTH - CHENNAI</h1>
              <p
                class="fontz"
              >Andhra Pradesh, Telangana, Tamil Nadu, Kerala, Karnataka, UT-Andaman and Nicobar Islands, UT-Pondicherry-Puducherry, UT-Lakshadweep</p>
            </v-card-text>
          </v-card>
        </v-flex>
        <v-flex class="px-1 py-2" xs12 md4 justify-center text-xs-center>
          <v-card class="bord" height="100%">
            <v-card-text text-xs-center>
              <h1 class="fontz22 pb-3">ZONE 3 - CENTRAL - AHMEDABAD</h1>
              <p
                class="fontz"
              >Maharashtra, Gujarat, Madhya Pradesh, Goa, UT-Daman and Diu, UT-Dadra and Nagar Haveli, Chhattisgarh</p>
            </v-card-text>
          </v-card>
        </v-flex>
    </v-layout>-->
    <!-- 
      <v-layout row wrap>
        <v-flex xs12 justify-center text-xs-center>
          <v-btn round outline router to="/process/#idzone">Read More</v-btn>
        </v-flex>
    </v-layout>-->

    <!-- <v-layout row wrap>
        <v-flex xs12 md6>
          <v-layout column wrap>
            <v-flex xs12 class="py-2">
              <v-card class="elevation-10">
                <v-card-title class="text-xs-center pb-0">
                  <h1 class="fontz22 grey--text text--darken-3">ZONE 1 - NORTH - DELHI</h1>
                </v-card-title>
                <v-card-text>
                  <h1
                    class="fontz2 grey--text text--darken-1"
                  >UT-Delhi, Jammu & Kashmir, Haryana, Punjab, Himachal Pradesh, Uttar Pradesh, Uttrakhand, Rajasthan, West Bengal, Bihar, UT-Chandigarh, Arunachal Pradesh, Assam, Meghalaya, Manipur, Nagaland, Tripura, Jharkhand, Sikkim, Odisha</h1>
                </v-card-text>
              </v-card>
            </v-flex>
            <v-flex xs12 class="py-2">
              <v-card class="elevation-10">
                <v-card-title class="text-xs-center pb-0">
                  <h1 class="fontz22 grey--text text--darken-3">ZONE 2 - SOUTH - CHENNAI</h1>
                </v-card-title>
                <v-card-text>
                  <h1
                    class="fontz2 grey--text text--darken-1"
                  >Andhra Pradesh, Telangana, Tamil Nadu, Kerala, Karnataka, UT-Andaman and Nicobar Islands, UT-Pondicherry-Puducherry, UT-Lakshadweep</h1>
                </v-card-text>
              </v-card>
            </v-flex>
            <v-flex xs12 class="py-2">
              <v-card class="elevation-10">
                <v-card-title class="text-xs-center pb-0">
                  <h1 class="fontz22 grey--text text--darken-3">ZONE 3 - CENTRAL - AHMEDABAD</h1>
                </v-card-title>
                <v-card-text>
                  <h1
                    class="fontz2 grey--text text--darken-1"
                  >Maharashtra, Gujarat, Madhya Pradesh, Goa, UT-Daman and Diu, UT-Dadra and Nagar Haveli, Chhattisgarh</h1>
                </v-card-text>
              </v-card>
            </v-flex>
            <v-flex xs12>
              <v-btn class="fontzd" round outline router to="/Process/#idzone">Read More</v-btn>
            </v-flex>
          </v-layout>
        </v-flex>
        <v-layout row wrap>
          <v-flex xs12 class="pa-2">
            <v-img contain :src="require('~/assets/img/india.jpg')"></v-img>
          </v-flex>
        </v-layout>
    </v-layout>-->
  </div>
</template> 

<script>
import Homehero from '@/components/HomeHero'
import topic from '@/components/topic'
import Theme from '@/components/Th'
import Subtitle from '@/components/Subtitle'

export default {
  components: {
    Homehero,
    Subtitle,
    topic,
    Theme
  },

  data: () => ({
    about: [
      'AAKRUTI is Dassault Systèmes SOLIDWORKS Corporation Nationwide Product Design Contest. AAKRUTI was launched in 2011 and has received tremendous response from all over India in the last 9 years. Each year brings forth a different theme with students surpassing the expectations with their innovative designs and ideas.',
      'The objective of AAKRUTI is to reach out to the engineering colleges and universities across India and make them aware about latest trends in the Product Design and Manufacturing domain. AAKRUTI encourages students to showcase their design skills, creativity and innate talent and to use this contest as a platform to design a product that can be commercially manufactured which can eventually benefit the nation.',
      'Dassault Systèmes will offer a limited period license of SOLIDWORKS education edition to all the registered teams to design and simulate their product ideas.'
    ]
  })
}
</script>

<style scoped>
.back {
  background-color: white;
  color: #01406c;
  /* background-color: rgb(119, 119, 119); */
}
.bottomtext {
  font-size: calc(16px + 5 * ((100vw - 320px) / 880));
  font-family: '3ds';
  text-align: left !important;
  color: #2f2e41;
}

.fontz {
  font-size: calc(12px + 4 * ((100vw - 320px) / 880));
  font-family: '3ds-light';
  font-weight: 500;
  line-height: 1.5;
  letter-spacing: -0.2px;
}
.fontz2 {
  font-size: calc(12px + 4 * ((100vw - 320px) / 880));
  font-family: '3ds';
}

.fontz22 {
  font-size: calc(15px + 4 * ((100vw - 320px) / 880)) !important;
  font-family: '3ds';
}

.bord {
  border: 2px solid #005386;
  border-radius: 30px;
  opacity: 0.9;
  box-shadow: 0 8px 12px 0 rgba(0, 0, 0, 0.3);
}

.image-hover-highlight {
  -webkit-transition: all 0.5s;
  transition: all 0.5s;
}
.image-hover-highlight:hover {
  border: 2px solid #005386;
  border-radius: 30px;
  opacity: 0.9;
  box-shadow: 0 6px 10px 0 rgba(0, 0, 0, 0.2);
  filter: brightness(130%);
  -webkit-filter: brightness(130%);
  -moz-filter: brightness(130%);
  -o-filter: brightness(130%);
  -ms-filter: brightness(130%);
  -webkit-transition: all 0.5s;
  transition: all 0.5s;
}
</style>
