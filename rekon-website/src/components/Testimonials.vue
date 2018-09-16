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
                                <img src="images/avatars/user-02.jpg" alt="Author image">
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
                                <img src="images/avatars/user-03.jpg" alt="Author image">
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
                                <img src="images/avatars/user-02.jpg" alt="Author image">
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
                                <img src="images/avatars/user-03.jpg" alt="Author image">
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
                                <img src="images/avatars/user-02.jpg" alt="Author image">
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
                                <img src="images/avatars/user-03.jpg" alt="Author image">
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

</style>
