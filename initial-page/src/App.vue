<template>
  <v-app>
    <v-content app>
      <section id="hero">
        <v-parallax src="./img/background.png" height="950" jumbotron>
          <v-layout column align-center justify-center class="parallax-default">
            <div style="width: 70vw">
              <v-img src="./img/logo.png"></v-img>
            </div>
            <h1
              class="text-xs-center font-weight-light bigger"
            >Fully Automated Account Reconciliation</h1>
            <h2 class="text-xs-center font-weight-light">
              For more contact us at
              <b>anders-wind@outlook.com</b>
            </h2>
            <v-btn
              flat
              @click="$vuetify.goTo('#problem', { offset: -150, easing: 'easeInOutCubic',})"
            >See more</v-btn>
          </v-layout>
        </v-parallax>
      </section>
      <section id="problem">
        <v-layout column wrap class="my-5" align-center justify-start>
          <v-flex xs12 sm4 class="my-3">
            <div class="text-xs-center">
              <h2 class="font-weight-light bigger">The Problem</h2>
            </div>
          </v-flex>
          <v-flex xs12>
            <v-container grid-list-xl>
              <v-layout row wrap>
                <v-flex xs12 md6>
                  <h1 class="med-big">Identifying matching transactions between two ledger accounts</h1>
                  <v-list class="transparent" three-line>
                    <v-list-tile>
                      <v-list-tile-action>
                        <v-icon large>access_time</v-icon>
                      </v-list-tile-action>
                      <v-list-tile-content class="big-list-text">Time and resource consuming</v-list-tile-content>
                    </v-list-tile>
                    <v-list-tile>
                      <v-list-tile-action>
                        <v-icon large>report_problem</v-icon>
                      </v-list-tile-action>
                      <v-list-tile-content
                        class="big-list-text"
                      >High risk of impacting company value</v-list-tile-content>
                    </v-list-tile>
                    <v-list-tile>
                      <v-list-tile-action>
                        <v-icon large>dashboard</v-icon>
                      </v-list-tile-action>
                      <v-list-tile-content class="big-list-text">Challenging task</v-list-tile-content>
                    </v-list-tile>
                    <v-list-tile>
                      <v-list-tile-action>
                        <v-icon large>highlight_off</v-icon>
                      </v-list-tile-action>
                      <v-list-tile-content class="big-list-text">Error prone process</v-list-tile-content>
                    </v-list-tile>
                  </v-list>
                </v-flex>
                <v-flex xs12 md6 sm12 style="min-width:50vh">
                  <v-img src="./img/ReconciliationExample.png"></v-img>
                </v-flex>
              </v-layout>
            </v-container>
          </v-flex>
        </v-layout>
      </section>
      <section id="solution" class="dark-section">
        <v-layout column wrap class="my-5" align-center>
          <v-flex xs12 sm4 class="my-3">
            <div class="text-xs-center">
              <h2 class="font-weight-light bigger">Our Solution</h2>
            </div>
          </v-flex>
          <v-flex xs12>
            <v-container grid-list-xl>
              <v-layout row wrap align-start>
                <v-flex xs12 md6>
                  <v-card dark class="elevation-0 transparent">
                    <v-card-title primary-title class="layout justify-center">
                      <div class="headline text-xs-center">Resolved</div>
                    </v-card-title>
                    <v-card-text>
                      <v-list class="transparent" three-line>
                        <v-list-tile>
                          <v-list-tile-action>
                            <v-icon large>playlist_add_check</v-icon>
                          </v-list-tile-action>
                          <v-list-tile-content class="big-list-text">Supports many-to-many matches</v-list-tile-content>
                        </v-list-tile>
                        <v-list-tile>
                          <v-list-tile-action>
                            <v-icon large>exposure</v-icon>
                          </v-list-tile-action>
                          <v-list-tile-content
                            class="big-list-text"
                          >Only values necessary for finding matches</v-list-tile-content>
                        </v-list-tile>
                        <v-list-tile>
                          <v-list-tile-action>
                            <v-icon large>sync</v-icon>
                          </v-list-tile-action>
                          <v-list-tile-content
                            class="big-list-text"
                          >Quick integration and easy to deploy</v-list-tile-content>
                        </v-list-tile>
                        <v-list-tile>
                          <v-list-tile-action>
                            <v-icon large>link_off</v-icon>
                          </v-list-tile-action>
                          <v-list-tile-content
                            class="big-list-text"
                          >Independent from any specific ERP solution</v-list-tile-content>
                        </v-list-tile>
                      </v-list>
                    </v-card-text>
                  </v-card>
                </v-flex>
                <v-flex xs12 md6>
                  <v-card dark class="elevation-0 transparent">
                    <v-card-title primary-title class="layout justify-center">
                      <div class="headline text-xs-center">Competition</div>
                    </v-card-title>
                    <v-card-text>
                      <v-list class="transparent" three-line>
                        <v-list-tile>
                          <v-list-tile-action>
                            <v-icon large>drag_handle</v-icon>
                          </v-list-tile-action>
                          <v-list-tile-content
                            class="big-list-text"
                          >Only supports one-to-one matches</v-list-tile-content>
                        </v-list-tile>
                        <v-list-tile>
                          <v-list-tile-action>
                            <v-icon large>format_size</v-icon>
                          </v-list-tile-action>
                          <v-list-tile-content class="big-list-text">Highly relied on metadata</v-list-tile-content>
                        </v-list-tile>
                        <v-list-tile>
                          <v-list-tile-action>
                            <v-icon large>sync_problem</v-icon>
                          </v-list-tile-action>
                          <v-list-tile-content class="big-list-text">Integration heavy</v-list-tile-content>
                        </v-list-tile>
                        <v-list-tile>
                          <v-list-tile-action>
                            <v-icon large>link</v-icon>
                          </v-list-tile-action>
                          <v-list-tile-content class="big-list-text">Bound to a specific ERP vendors</v-list-tile-content>
                        </v-list-tile>
                      </v-list>
                    </v-card-text>
                  </v-card>
                </v-flex>
              </v-layout>
            </v-container>
          </v-flex>
        </v-layout>
      </section>
      <section id="contact">
        <v-container grid-list-xl>
          <v-layout row wrap justify-center class="my-5">
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
                      <v-list-tile-title>anders-wind@outlook.com</v-list-tile-title>
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
import { Component, Prop, Vue } from "vue-property-decorator";

@Component({
  components: {}
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
  font-size: 2.5em;
}
.med-big {
  font-size: 2em;
}
.big-list-text {
  font-size: 1.6em;
  font-weight: 300 !important;
  overflow: initial;
}
.medium {
  font-size: 1.5em;
}
.small {
  font-size: 1.2em;
}
</style>

