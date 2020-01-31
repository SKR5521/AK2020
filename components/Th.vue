<template>
  <div>
    <v-container>
      <topic text="AAKRUTI2020 THEMES" />
      <v-row row wrap justify="center" fill-height>
        <v-col cols="12" sm="6" class="py-4" v-for=" itm in cont" :key="itm.id">
          <v-card dark class="bord elevation-6" height="100%">
            <v-card-title class="justify-center text-wrap" >
              <v-row class="fill-height align-center">
                <v-col cols="3">
                  <v-img
                    color="white"
                    max-width="150px"
                    :src="require('../assets/img/themes/' + itm.id + '.svg')"
                  ></v-img>
                </v-col>
                <v-col cols="9">
                  <h6 class="fontz2 text-wrap">{{itm.tag}}</h6>
                </v-col>
              </v-row>
            </v-card-title>
            <v-card-text>
              <div class="py-2">
                <h3 class="fontzd">What to Design?</h3>
                <h4 class="fontz white--text">{{itm.what}}</h4>
              </div>

              <div class="py-2">
                <h3 class="fontzd">How to Design?</h3>
                <h4 class="fontz white--text">{{itm.How}}</h4>
              </div>

              <div class="py-2">
                <h3 class="fontzd">Who will get Benefits?</h3>
                <h4 class="fontz white--text">{{itm.who}}</h4>
              </div>
            </v-card-text>
          </v-card>          
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
import topic from "@/components/topic";
import Subtitle from "@/components/Subtitle";

export default {
  components: {
    topic,
    Subtitle
  },
  data: () => {
    return {
      cont: [
        {
          id: 1,
          tag: "Small Is Big",
          what:
            "Think, Re-engineer, Simulate and validate existing product and optimize it. The product should be lighter, small in size, energy efficient and optimized for performance. Mandatory expectation: You are expected to modify / optimize existing product / device. Hence presenting existing product and how it is optimized is a ‘must’.",
          who: "Future Ready Engineers.",
          How:
            "Using principles of Reverse Engineering 3D Scanning existing product, Topology Optimization, Additive Manufacturing."
        },

        {
          id: 2,
          tag: "Medical Devices with innovation",
          what:
            "What if, we have the medical device(s) which will help patients (rural) in critical situation?  These devices should be cost effective, energy efficient, easy to handle and cheaper. Design device which is innovative and will be a great boon to patients/medical practitioners.",
          who: "Doctor, Physician, Patients.",
          How:
            "Implementing the science of biomedical, bioengineering, human ergonomics, human safety, medical regulatory & norms."
        },

        {
          id: 3,
          tag: "Design Product for rural Entrepreneurship",
          what:
            "If we provide product ideas to rural youth which they can manufacture locally, can we improve their livelihood opportunities? ",
          who: "Farmers, Rural youths, Villagers.",
          How:
            "Can we boost the rural entrepreneurship? In the field of Agriculture, affordable energy for remote places, handicraft, sanitation etc. By developing product ideas with DIY kits."
        },

        {
          id: 4,
          tag: "Stop Pollution at Source",
          what:
            "If we prevent source of pollution, can we create healthier environment and sustainable universe for our future generation?",
          who: "Universal citizens",
          How:
            "Can we eliminate/replace the components?  Which are causing heavy pollution, larger carbon footprint, increasing GHGs by managing eliminating problem at source?"
        }
      ]
    };
  }
};
</script>

<style scoped>
.fontz {
 font-size: calc(14px + 1 * ((100vw - 320px) / 880));
  font-family: '3ds-light';
  text-align: left !important;
  color: #2e2e2e !important;
}

.bord {
  border-radius: 14px;
  background-color: #F5F5F5;
  border-bottom: 10px solid #044b7c;
}
.fontzd {
  font-size: calc(15px + 1 * ((100vw - 320px) / 880));
  font-family: '3ds';
  text-align: left !important;
  color: #253C53;
}

.fontz2 {
  font-size: calc(17px + 5 * ((100vw - 320px) / 880));
  font-family: "3ds-SemiBold";
  text-align: left !important;
  color: #ef5350;
}
/* .bord {
  border: 2px solid #005386;
  border-radius: 30px;
  opacity: 0.9;
  box-shadow: 0 8px 12px 0 rgba(0, 0, 0, 0.3);
} */



.image-hover-highlight {
  -webkit-transition: all 0.5s;
  transition: all 0.5s;
}
.image-hover-highlight:hover {
  border: 2px solid #005386;
  border-radius: 30px;
  background-color: white;
  cursor: pointer;
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
