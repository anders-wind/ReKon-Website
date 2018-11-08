<template>
  <v-app>
    <v-content app>
      <v-container fluid fill-height>
        <v-layout align-center justify-center class="back">
          <v-layout column align-center>
            <v-container style="width: 70vw">
              <v-img src="./img/logo.png"></v-img>
            </v-container>
            <h1 class="font-weight-light">Fully Automated Account Reconciliation</h1>
            <h2 class="font-weight-light">
              For more contact us at
              <b>awis@itu.dk</b>
            </h2>
          </v-layout>
        </v-layout>
      </v-container>
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
.back {
  background-image: url('/img/background.png');
  background-size: 95%;
  background-position: center;
}
</style>

