<template>
    <section id="download">

        <div class="row">
            <div class="col-full">
                <h1 class="intro-header aos-init aos-animate" data-aos="fade-up">Download Our App Today!</h1>

                <p class="lead aos-init aos-animate" data-aos="fade-up">
                    Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate
                </p>

                <ul class="download-badges">
                    <li><a href="#" title="" class="badge-appstore aos-init aos-animate" data-aos="fade-up">App Store</a></li>
                    <li><a href="#" title="" class="badge-googleplay aos-init aos-animate" data-aos="fade-up">Play Store</a></li>
                </ul>

            </div>
        </div>

    </section> <!-- end download -->    
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Download extends Vue {
  @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
/* ===================================================================
 *  14. download - (_layout.scss)
 *
 * ------------------------------------------------------------------- */
#download {
  background: #39b54a;
  color: #b2fabc;
  padding-top: 12rem;
  padding-bottom: 12rem;
  text-align: center;
}
#download h1 {
  color: #ffffff;
}
#download h1::before {
  background-color: #2a9038;
  left: 50%;
  -webkit-transform: translateX(-50%);
  -ms-transform: translateX(-50%);
  transform: translateX(-50%);
}
#download .lead {
  color: #b2fabc;
  margin-top: 4.8rem;
}
#download .row {
  max-width: 800px;
}
#download .download-badges {
  list-style: none;
  margin: 0;
  text-align: center;
}
#download .download-badges li {
  display: inline-block;
  margin: 0 7.5px;
  padding-left: 0;
}
#download .download-badges li a {
  display: block;
  width: 230px;
  height: 71px;
  font: 0/0 a;
  text-shadow: none;
  color: transparent;
  background-repeat: no-repeat;
  background-position: center;
  background-size: 230px 71px;
}
#download .download-badges li a.badge-appstore {
  background-image: url("/src/assets/images/appstore");
}
#download .download-badges li a.badge-googleplay {
  background-image: url("/src/assets/images/google-play");
}
/* ------------------------------------------------------------------- 
 * responsive:
 * download
 * ------------------------------------------------------------------- */
@media only screen and (max-width: 768px) {
  #download .download-badges li a {
    width: 194px;
    height: 60px;
    background-size: 194px 60px;
  }
}
</style>
