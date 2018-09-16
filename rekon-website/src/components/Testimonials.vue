<template>
    <section id="testimonials">

        <div class="row">
            <div class="col-twelve">
                <h1 class="intro-header aos-init aos-animate" data-aos="fade-up">What They Say About Our App.</h1>
            </div>   		
        </div>   	

        <div class="row owl-wrap">

            <div id="testimonial-slider" data-aos="fade-up" class="aos-init aos-animate">

                <div class="slides owl-carousel owl-loaded owl-drag">

                     

                     

                <div class="owl-stage-outer owl-height" style="height: 466px;"><div class="owl-stage" style="transform: translate3d(-1800px, 0px, 0px); transition: all 0s ease 0s; width: 5400px;"><div class="owl-item cloned" style="width: 900px;"><div>
                        <p>
                        Your work is going to fill a large part of your life, and the only way to be truly satisfied is
                        to do what you believe is great work. And the only way to do great work is to love what you do.
                        If you haven't found it yet, keep looking. Don't settle. As with all matters of the heart, you'll know when you find it.
                        </p> 

                        <div class="testimonial-author">
                                <img src="../assets/images/avatars/user-02.jpg" alt="Author image">
                                <div class="author-info">
                                    Steve Jobs
                                    <span class="position">CEO, Apple.</span>
                                </div>
                        </div>                 
                    </div></div><div class="owl-item cloned" style="width: 900px;"><div>
                        <p>
                        This is Photoshop's version  of Lorem Ipsum. Proin gravida nibh vel velit auctor aliquet.
                        Aenean sollicitudin, lorem quis bibendum auctor, nisi elit consequat ipsum, nec sagittis sem
                        nibh id elit. Duis sed odio sit amet nibh vulputate cursus a sit amet mauris.    
                        </p>

                        <div class="testimonial-author">
                                <img src="../assets/images/avatars/user-03.jpg" alt="Author image">
                                <div class="author-info">
                                    John Doe
                                    <span>CEO, ABC Corp.</span>
                                </div>
                        </div>                                         
                    </div></div><div class="owl-item active" style="width: 900px;"><div>
                        <p>
                        Your work is going to fill a large part of your life, and the only way to be truly satisfied is
                        to do what you believe is great work. And the only way to do great work is to love what you do.
                        If you haven't found it yet, keep looking. Don't settle. As with all matters of the heart, you'll know when you find it.
                        </p> 

                        <div class="testimonial-author">
                                <img src="../assets/images/avatars/user-02.jpg" alt="Author image">
                                <div class="author-info">
                                    Steve Jobs
                                    <span class="position">CEO, Apple.</span>
                                </div>
                        </div>                 
                    </div></div><div class="owl-item" style="width: 900px;"><div>
                        <p>
                        This is Photoshop's version  of Lorem Ipsum. Proin gravida nibh vel velit auctor aliquet.
                        Aenean sollicitudin, lorem quis bibendum auctor, nisi elit consequat ipsum, nec sagittis sem
                        nibh id elit. Duis sed odio sit amet nibh vulputate cursus a sit amet mauris.    
                        </p>

                        <div class="testimonial-author">
                                <img src="../assets/images/avatars/user-03.jpg" alt="Author image">
                                <div class="author-info">
                                    John Doe
                                    <span>CEO, ABC Corp.</span>
                                </div>
                        </div>                                         
                    </div></div><div class="owl-item cloned" style="width: 900px;"><div>
                        <p>
                        Your work is going to fill a large part of your life, and the only way to be truly satisfied is
                        to do what you believe is great work. And the only way to do great work is to love what you do.
                        If you haven't found it yet, keep looking. Don't settle. As with all matters of the heart, you'll know when you find it.
                        </p> 

                        <div class="testimonial-author">
                                <img src="../assets/images/avatars/user-02.jpg" alt="Author image">
                                <div class="author-info">
                                    Steve Jobs
                                    <span class="position">CEO, Apple.</span>
                                </div>
                        </div>                 
                    </div></div><div class="owl-item cloned" style="width: 900px;"><div>
                        <p>
                        This is Photoshop's version  of Lorem Ipsum. Proin gravida nibh vel velit auctor aliquet.
                        Aenean sollicitudin, lorem quis bibendum auctor, nisi elit consequat ipsum, nec sagittis sem
                        nibh id elit. Duis sed odio sit amet nibh vulputate cursus a sit amet mauris.    
                        </p>

                        <div class="testimonial-author">
                                <img src="../assets/images/avatars/user-03.jpg" alt="Author image">
                                <div class="author-info">
                                    John Doe
                                    <span>CEO, ABC Corp.</span>
                                </div>
                        </div>                                         
                    </div></div></div></div><div class="owl-nav disabled"><div class="owl-prev">prev</div><div class="owl-next">next</div></div><div class="owl-dots"><div class="owl-dot active"><span></span></div><div class="owl-dot"><span></span></div></div></div> <!-- end slides -->

            </div> <!-- end testimonial-slider -->         
            
        </div> <!-- end flex-container -->

    </section> <!-- end testimonials -->
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Testimonials extends Vue {
  @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
/* ===================================================================
 *  13. testimonials - (_layout.scss)
 *
 * ------------------------------------------------------------------- */
#testimonials {
  background: #ffffff;
  padding: 15rem 0 9rem;
  text-align: center;
  min-height: 600px;
}
#testimonials h1::before {
  left: 50%;
  -webkit-transform: translateX(-50%);
  -ms-transform: translateX(-50%);
  transform: translateX(-50%);
}
#testimonials .owl-wrap {
  width: 80%;
  max-width: 900px;
  margin: 4.2rem auto 0;
}
#testimonial-slider {
  margin: 0 0 3rem 0;
  position: relative;
}
#testimonial-slider .slides {
  padding-bottom: 3rem;
}
#testimonial-slider p {
  font-family: "muli-regular", sans-serif;
  font-size: 3.2rem;
  line-height: 1.5;
  color: #303030;
}
#testimonial-slider p::before,
#testimonial-slider p::after {
  display: inline-block;
  font-family: "muli-regular", serif;
  font-size: 3.6rem;
  line-height: 1;
  position: relative;
  top: 0.3rem;
}
#testimonial-slider p::before {
  content: "\201C";
}
#testimonial-slider p::after {
  content: "\201D";
}
#testimonial-slider .testimonial-author {
  margin-top: 4.2rem;
}
#testimonial-slider .testimonial-author img {
  width: 7.4rem;
  height: 7.4rem;
  margin: 0 auto 1.2rem auto;
  display: block;
  border-radius: 50%;
}
#testimonial-slider .testimonial-author .author-info {
  display: inline-block;
  vertical-align: middle;
  text-align: center;
  font-family: "montserrat-semibold", sans-serif;
  font-size: 1.9rem;
  margin-top: 0.9rem;
  margin-bottom: 3rem;
  color: #151515;
}
#testimonial-slider .testimonial-author .author-info span {
  display: block;
  font-family: "muli-bold", sans-serif;
  font-size: 1.6rem;
  line-height: 1.313;
  letter-spacing: 0;
  text-transform: none;
  color: rgba(0, 0, 0, 0.5);
  margin-top: 0.3rem;
}
/* owl dots */
#testimonial-slider .owl-nav {
  margin-top: 1.8rem;
  margin-bottom: 1.5rem;
  text-align: center;
  -webkit-tap-highlight-color: transparent;
}
#testimonial-slider .owl-nav [class*="owl-"] {
  color: #ffffff;
  font-family: "montserrat-regular", sans-serif;
  font-size: 1.4rem;
  height: 3rem;
  line-height: 3rem;
  margin: 0.6rem;
  padding: 0 10px;
  background: rgba(0, 0, 0, 0.5);
  display: inline-block;
  cursor: pointer;
  border-radius: 3px;
  -webkit-transition: all 0.3s ease-in-out;
  transition: all 0.3s ease-in-out;
}
#testimonial-slider .owl-nav [class*="owl-"]:hover {
  background: rgba(0, 0, 0, 0.7);
  color: #ffffff;
  text-decoration: none;
}
#testimonial-slider .owl-nav .disabled {
  background: rgba(0, 0, 0, 0.2);
  cursor: default;
}
#testimonial-slider .owl-nav.disabled + .owl-dots {
  margin-top: 1.8rem;
}
#testimonial-slider .owl-dots {
  text-align: center;
  -webkit-tap-highlight-color: transparent;
}
#testimonial-slider .owl-dots .owl-dot {
  display: inline-block;
  zoom: 1;
  *display: inline;
}
#testimonial-slider .owl-dots .owl-dot span {
  width: 9px;
  height: 9px;
  background-color: #959595;
  margin: 9px 9px;
  display: block;
  -webkit-backface-visibility: visible;
  backface-visibility: visible;
  transition: opacity 200ms ease;
  border-radius: 50%;
  -webkit-transition: all 0.3s ease-in-out;
  transition: all 0.3s ease-in-out;
}
#testimonial-slider .owl-dots .owl-dot.active span,
#testimonial-slider .owl-dots .owl-dot:hover span {
  background-color: #39b54a;
}
/* ------------------------------------------------------------------- 
 * responsive:
 * testimonials
 * ------------------------------------------------------------------- */
@media only screen and (max-width: 1024px) {
  #testimonial-slider p {
    font-size: 3rem;
  }
}
@media only screen and (max-width: 768px) {
  #testimonial-slider p {
    font-size: 2.6rem;
  }
  #testimonial-slider .testimonial-author img {
    width: 6.6rem;
    height: 6.6rem;
  }
  #testimonial-slider .testimonial-author .author-info {
    font-size: 1.8rem;
  }
  #testimonial-slider .testimonial-author .author-info span {
    font-size: 1.5rem;
  }
}
@media only screen and (max-width: 600px) {
  #testimonials .owl-wrap {
    width: 90%;
  }
  #testimonial-slider p {
    font-size: 2.4rem;
  }
}
@media only screen and (max-width: 400px) {
  #testimonials .owl-wrap {
    width: 100%;
  }
  #testimonial-slider p {
    font-size: 2rem;
  }
}
</style>
