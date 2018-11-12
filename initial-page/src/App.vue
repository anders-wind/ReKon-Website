<template>
  <v-app>
    <v-content app>
      <section>
        <v-parallax src="./img/background.png" height="950">
          <v-layout column align-center justify-center class="parallax-default">
            <div style="width: 70vw">
              <v-img src="./img/logo.png"></v-img>
            </div>
            <h1 class="font-weight-light bigger">Fully Automated Account Reconciliation</h1>
            <h2 class="font-weight-light">
              For more contact us at
              <b>awis@itu.dk</b>
            </h2>
          </v-layout>
        </v-parallax>
      </section>
      <!-- <section class="dark-section">
        <v-layout column wrap="" class="my-5" align-center>
          <v-flex xs12 sm4 class="my-3">
            <div class="text-xs-center">
              <h2 class="headline">The best way to start developing</h2>
              <span class="subheading">Cras facilisis mi vitae nunc</span>
            </div>
          </v-flex>
        </v-layout>
      </section>
      <section>
        <v-layout column wrap="" class="my-5" align-center>
          <v-flex xs12 sm4 class="my-3">
            <div class="text-xs-center">
              <h2 class="headline">The best way to start developing</h2>
              <span class="subheading">Cras facilisis mi vitae nunc</span>
            </div>
          </v-flex>
        </v-layout>
      </section>-->
    </v-content>
  </v-app>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component({
  components: {},
})
export default class App extends Vue {}
</script>

<style lang="scss">
.parallax-default {
  color: #181818;
}
.dark-section {
  background-color: #181818;
  color: whitesmoke;
}
.bigger {
  font-size: 2em;
}
</style>

