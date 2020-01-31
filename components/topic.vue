<template>
  <v-container fluid>
    <v-row>
      <v-col align="center" justify="center" cols="12">
        <h4 class="fontz">{{ text }}</h4>
        <div>
          <span class="break-small"></span>
        </div>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  props: {
    text: {
      type: String,
      default: "Set_Topic"
    },
  },
}
</script>

<style scoped>
/* v-resize-text="{ratio: '1.2',minFontSize: '20px', maxFontSize: '50px'}" #01548A; */
.break-small {
  background: #e31818;
  border: 0;
  display: inline-block;
  height: 3px;
  margin: 4px 0 10px;
  width: 70px;
}

.fontz {
  font-size: calc(24px + 10 * ((100vw - 320px) / 880)) !important;
  font-family: '3ds';
  font-weight: 300;
  line-height: 1.5;
  color: #e31818;
  letter-spacing: -0.2px;
}
</style>