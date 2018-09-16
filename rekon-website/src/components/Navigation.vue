<template>
   <header id="header" class="row">   
   		<div class="header-logo">
	        <a href="index.html">Dazzle</a>
	    </div>

	   	<nav id="header-nav-wrap">
			<ul class="header-main-nav">
				<li class=""><a class="smoothscroll" href="#home" title="home">Home</a></li>
                <li class=""><a class="smoothscroll" href="#about" title="about">About</a></li>
				<li class=""><a class="smoothscroll" href="#pricing" title="pricing">Pricing</a></li>
				<li class="current"><a class="smoothscroll" href="#testimonials" title="testimonials">Testimonials</a></li>
				<li class=""><a class="smoothscroll" href="#download" title="download">Download</a></li>	
			</ul>

            <a href="#" title="sign-up" class="button button-primary cta">Sign Up</a>
		</nav>

		<a class="header-menu-toggle" href="#"><span>Menu</span></a>    	
   </header> <!-- /header -->
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Navigation extends Vue {
  @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
