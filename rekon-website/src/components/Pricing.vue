<template>
    <section id="pricing">
        <div class="row pricing-content">

            <div class="col-four pricing-intro">
                <h1 class="intro-header aos-init aos-animate" data-aos="fade-up">Our Pricing Options</h1>

                <p data-aos="fade-up" class="aos-init aos-animate">Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium. 
                </p>
            </div>

            <div class="col-eight pricing-table">
                <div class="row">

                    <div class="col-six plan-wrap">
                        <div class="plan-block aos-init aos-animate" data-aos="fade-up"> 

                            <div class="plan-top-part">
                                <h3 class="plan-block-title">Lite Plan</h3>
                                <p class="plan-block-price"><sup>$</sup>25</p>
                                <p class="plan-block-per">Per Month</p>
                            </div>

                            <div class="plan-bottom-part">
                                <ul class="plan-block-features">
                                    <li><span>3GB</span> Storage</li>
                                    <li><span>10GB</span> Bandwidth</li>	                  
                                    <li><span>5</span> Databases</li>		                  
                                    <li><span>30</span> Email Accounts</li>
                                </ul>

                                <a class="button button-primary large" href="">Get Started</a>
                            </div>  
                     
                        </div>
                    </div> <!-- end plan-wrap -->

                    <div class="col-six plan-wrap">
                        <div class="plan-block primary aos-init aos-animate" data-aos="fade-up">

                            <div class="plan-top-part">
                                <h3 class="plan-block-title">Pro Plan</h3>
                                <p class="plan-block-price"><sup>$</sup>50</p>
                                <p class="plan-block-per">Per Month</p>
                            </div>

                            <div class="plan-bottom-part">
                                <ul class="plan-block-features">
                                    <li><span>5GB</span> Storage</li>
                                    <li><span>20GB</span> Bandwidth</li>	                  
                                    <li><span>15</span> Databases</li>		                  
                                    <li><span>70</span> Email Accounts</li>
                                </ul>

                                <a class="button button-primary large" href="">Get Started</a>
                            </div>

                        </div>
                    </div> <!-- end plan-wrap -->

                </div>               
            </div> <!-- end pricing-table -->

        </div> <!-- end pricing-content -->
    </section> <!-- end pricing -->
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Pricing extends Vue {
  @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
/* ===================================================================
 *  12. pricing - (_layout.scss)
 *
 * ------------------------------------------------------------------- */
#pricing {
  background: #ebebeb;
  padding-top: 15rem;
  padding-bottom: 12rem;
}
#pricing h1 {
  margin-bottom: 3.6rem;
}
.pricing-intro {
  padding-top: 0.6rem;
}
.pricing-table {
  text-align: center;
}
.pricing-table .plan-block {
  background: #ffffff;
  border-radius: 5px;
  padding: 4.8rem 4rem 5.4rem;
  margin-bottom: 4.8rem;
}
.pricing-table .plan-block:after {
  content: "";
  display: table;
  clear: both;
}
.pricing-table .plan-block .plan-block-title {
  font-family: "Montserrat", sans-serif;
  font-size: 2.4rem;
  margin-bottom: 3.6rem;
}
.pricing-table .plan-block .plan-block-price {
  font-family: "Montserrat", sans-serif;
  font-weight: 620;
  font-size: 7.8rem;
  color: #151515;
  line-height: 1;
  margin-bottom: 0;
}
.pricing-table .plan-block .plan-block-price sup {
  font-family: "Montserrat", sans-serif;
  font-size: 3rem;
  top: -3.6rem;
  margin-right: 3px;
}
.pricing-table .plan-block .plan-block-per {
  margin-top: -0.6rem;
  margin-bottom: 0;
  font-family: "Montserrat", sans-serif;
  font-weight: 620;
  font-size: 1.7rem;
}
.pricing-table .plan-block .plan-block-features {
  list-style: none;
  margin: 0 2rem 4.2rem;
  border-top: 1px solid rgba(0, 0, 0, 0.1);
  font-size: 1.6rem;
  line-height: 2.4rem;
}
.pricing-table .plan-block .plan-block-features li {
  padding: 1.2rem 0;
  border-bottom: 1px solid rgba(0, 0, 0, 0.1);
}
.pricing-table .plan-block .plan-block-features li span {
  color: #39b54a;
  font-family: "muli", sans-serif;
  font-weight: bold;
}
.pricing-table .plan-block.primary {
  background: #39b54a;
  color: rgba(255, 255, 255, 0.8);
}
.pricing-table .plan-block.primary .plan-block-title,
.pricing-table .plan-block.primary .plan-block-price {
  color: #ffffff;
}
.pricing-table .plan-block.primary .plan-block-features {
  border-top: 1px solid rgba(255, 255, 255, 0.2);
}
.pricing-table .plan-block.primary .plan-block-features li {
  border-bottom: 1px solid rgba(255, 255, 255, 0.2);
}
.pricing-table .plan-block.primary .plan-block-features li span {
  color: #ffffff;
}
.pricing-table .plan-block.primary .button.button-primary {
  background: #ffffff;
  color: #151515;
  border-color: #ffffff;
}
.pricing-table .plan-block.primary .button.button-primary:hover,
.pricing-table .plan-block.primary .button.button-primary:focus {
  color: #39b54a;
}
.pricing-table .plan-bottom-part {
  margin-top: 3rem;
}
/* ------------------------------------------------------------------- 
 * responsive:
 * pricing 
 * ------------------------------------------------------------------- */
@media only screen and (max-width: 1024px) {
  #pricing .pricing-content > [class*="col"] {
    width: 100% !important;
    float: none !important;
    clear: both !important;
    margin-left: 0;
    margin-right: 0;
  }
  #pricing [class*="col"].pricing-intro {
    text-align: center;
    margin-left: auto;
    margin-right: auto;
    max-width: 650px;
  }
  #pricing [class*="col"].pricing-intro h1::before {
    left: 50%;
    -webkit-transform: translateX(-50%);
    -ms-transform: translateX(-50%);
    transform: translateX(-50%);
  }
  #pricing [class*="col"].pricing-table {
    margin-top: 5.4rem;
    max-width: 650px;
    margin-left: auto;
    margin-right: auto;
  }
}
@media only screen and (max-width: 768px) {
  .pricing-table .plan-wrap {
    width: 100% !important;
    float: none !important;
    clear: both !important;
    margin-left: 0;
    margin-right: 0;
  }
  .pricing-table .plan-top-part,
  .pricing-table .plan-bottom-part {
    float: left;
  }
  .pricing-table .plan-top-part {
    width: 41.66667%;
    margin-top: 1.2rem;
  }
  .pricing-table .plan-bottom-part {
    width: 58.33333%;
  }
}
@media only screen and (max-width: 600px) {
  #pricing [class*="col"].pricing-table {
    max-width: 360px;
  }
  #pricing .plan-top-part,
  #pricing .plan-bottom-part {
    width: 100% !important;
    float: none !important;
    clear: both !important;
    margin-left: 0;
    margin-right: 0;
  }
}
</style>
