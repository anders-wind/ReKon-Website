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
            <v-btn
              flat
              @click="$vuetify.goTo('#problem', { offset: -150, easing: 'easeInOutCubic',})"
            >See more</v-btn>
          </v-layout>
        </v-parallax>
      </section>
      <section id="problem">
        <v-layout column wrap="" class="my-5" align-center justify-start>
          <v-flex xs12 sm4 class="my-3">
            <div class="text-xs-center">
              <h2 class="font-weight-light bigger">The Problem</h2>
            </div>
          </v-flex>
          <v-flex xs12>
            <v-container grid-list-xl>
              <v-layout row wrap="">
                <v-flex xs12 md6>
                  <h1 class="bigger">Identifying matching transactions between two ledger accounts</h1>
                  <ul class="no-bullet">
                    <li class="font-weight-light bigger spacing">
                      <v-icon large class="aligned-icon">access_time</v-icon>&emsp;Time and resource consuming
                    </li>
                    <li class="font-weight-light bigger spacing">
                      <v-icon large class="aligned-icon">report_problem</v-icon>&emsp;High risk of impacting company value
                    </li>
                    <li class="font-weight-light bigger spacing">
                      <v-icon large class="aligned-icon">dashboard</v-icon>&emsp;Challenging task
                    </li>
                    <li class="font-weight-light bigger spacing">
                      <v-icon large class="aligned-icon">highlight_off</v-icon>&emsp;Error prone process
                    </li>
                  </ul>
                </v-flex>
                <v-flex xs12 md6>
                  <v-img src="./img/ReconciliationExample.png" style="width:40vw"></v-img>
                </v-flex>
              </v-layout>
            </v-container>
          </v-flex>
        </v-layout>
      </section>
      <section class="dark-section">
        <v-layout column wrap="" class="my-5" align-center>
          <v-flex xs12 sm4 class="my-3">
            <div class="text-xs-center">
              <h2 class="font-weight-light bigger">Our Solution</h2>
            </div>
          </v-flex>
          <v-flex xs12>
            <v-container grid-list-xl>
              <v-layout row wrap="" align-start>
                <v-flex xs12 md6>
                  <v-card dark class="elevation-0 transparent">
                    <v-card-title primary-title class="layout justify-center">
                      <div class="headline text-xs-center">Resolved</div>
                    </v-card-title>
                    <v-card-text>
                      <ul class="no-bullet">
                        <li class="font-weight-light bigger spacing">Supports many-to-many matches</li>
                        <li
                          class="font-weight-light bigger spacing"
                        >Only values necessary for finding matches</li>
                        <li
                          class="font-weight-light bigger spacing"
                        >Quick integration and easy to deploy</li>
                        <li
                          class="font-weight-light bigger spacing"
                        >Independent from any specific ERP solution</li>
                      </ul>
                    </v-card-text>
                  </v-card>
                </v-flex>
                <v-flex xs12 md6>
                  <v-card dark class="elevation-0 transparent">
                    <v-card-title primary-title class="layout justify-center">
                      <div class="headline text-xs-center">Competition</div>
                    </v-card-title>
                    <v-card-text>
                      <ul class="no-bullet">
                        <li
                          class="font-weight-light bigger spacing"
                        >Only supports one-to-one matches</li>
                        <li class="font-weight-light bigger spacing">Highly relied on metadata</li>
                        <li
                          class="font-weight-light bigger spacing"
                        >Integration heavy, due to metadata dependency</li>
                        <li class="font-weight-light bigger spacing">Bound to a specific ERP vendors</li>
                      </ul>
                    </v-card-text>
                  </v-card>
                </v-flex>
              </v-layout>
            </v-container>
          </v-flex>
        </v-layout>
      </section>
      <section>
        <v-container grid-list-xl>
          <v-layout row wrap="" justify-center class="my-5">
            <v-flex xs12 sm5>
              <v-card class="elevation-0 transparent">
                <v-card-title primary-title class="layout justify-center">
                  <div class="headline">Company info</div>
                </v-card-title>
                <v-card-text class="small">
                  <p>
                    We are looking for partners who want to participate in the creation of a full solution.
                    Currently, we have seen the system perform reconciliation on a few real world cases successfully.
                    Now we seek the opportunity to try the algorithms in a broader real world setting, and obtain a better understanding of the core value propositions, so we can develop the right product.
                    Investors, partners, pilot customers, and advisors are equally valuable at this early stage.
                  </p>
                  <p>We are just at the beginning of our journey and there are many problems to tackle along the way, but we believe Resolved has a great potential in the future of automated finance.</p>
                </v-card-text>
              </v-card>
            </v-flex>
            <v-flex xs12 sm4 offset-sm1>
              <v-card class="elevation-0 transparent">
                <v-card-title primary-title class="layout justify-center">
                  <div class="headline">Contact us</div>
                </v-card-title>
                <v-card-text
                  class="small"
                >If you are interested in hearing more about us, don't hesitate to reach us</v-card-text>
                <v-list class="transparent">
                  <v-list-tile>
                    <v-list-tile-action>
                      <v-icon class="blue--text text--lighten-2">phone</v-icon>
                    </v-list-tile-action>
                    <v-list-tile-content>
                      <v-list-tile-title>41 36 48 07</v-list-tile-title>
                    </v-list-tile-content>
                  </v-list-tile>
                  <v-list-tile>
                    <v-list-tile-action>
                      <v-icon class="blue--text text--lighten-2">place</v-icon>
                    </v-list-tile-action>
                    <v-list-tile-content>
                      <v-list-tile-title>Copenhagen, DK</v-list-tile-title>
                    </v-list-tile-content>
                  </v-list-tile>
                  <v-list-tile>
                    <v-list-tile-action>
                      <v-icon class="blue--text text--lighten-2">email</v-icon>
                    </v-list-tile-action>
                    <v-list-tile-content>
                      <v-list-tile-title>awis@itu.dk</v-list-tile-title>
                    </v-list-tile-content>
                  </v-list-tile>
                </v-list>
              </v-card>
            </v-flex>
          </v-layout>
        </v-container>
      </section>
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
.medium {
  font-size: 1.5em;
}
.small {
  font-size: 1.2em;
}
.no-bullet {
  list-style-type: none;
}
.spacing {
  margin-top: 0.8em;
}
.aligned-icon {
  margin: -0px;
}
</style>

