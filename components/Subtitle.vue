<template>
  <v-container class="py-0">
    <v-row  row justify-space-around>
      <v-col cols="12" py-1 text-xs-center>
        <h1 class=" fontz"  >{{ subtopic }}</h1>
        <div> <span class="break-small"></span></div>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>

export default {
  props: ['subtopic'] 

}
</script>

<style scoped>
/* v-resize-text="{minFontSize: '16px', maxFontSize: '40px'}" */
.break-small {
    background: #105C8E;
    border: 0;
    display: inline-block;
    height: 2px;
    margin: 4px 0 8px;
    width: 50px;
}
.fontz {
  font-size: calc(18px + 8 * ((100vw - 320px) / 880)) !important;
  font-family: '3ds';
  font-weight: 400;
  line-height: 1.5;
  color: #105C8E;
  letter-spacing: -.2px
}
</style>