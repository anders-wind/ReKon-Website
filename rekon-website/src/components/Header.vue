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
export default class Header extends Vue {
  @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#header {
  width: 100%;
  height: 72px;
  background-color: #111111;
  position: fixed;
  left: 50%;
  -webkit-transform: translateX(-50%);
  -ms-transform: translateX(-50%);
  transform: translateX(-50%);
  z-index: 501;
}

/* ------------------------------------------------------------------- 
 * header logo - (_site-layout.css) 
 * ------------------------------------------------------------------- */

.header-logo {
  position: absolute;
  left: 40px;
  top: 50%;
  -webkit-transform: translateY(-50%);
  -ms-transform: translateY(-50%);
  transform: translateY(-50%);
  -webkit-transition: all 1s ease-in-out;
  transition: all 1s ease-in-out;
  z-index: 501;
}

.header-logo a {
  display: block;
  margin: 0;
  padding: 0;
  outline: 0;
  border: none;
  width: 97px;
  height: 22px;
  background: url("../assets/images/logo.png") no-repeat center;
  background-size: 97px 22px;
  font: 0/0 a;
  text-shadow: none;
  color: transparent;
  -webkit-transition: all 0.5s ease-in-out;
  transition: all 0.5s ease-in-out;
}

/* ------------------------------------------------------------------- 
 * menu trigger - (_site-layout.css) 
 * ------------------------------------------------------------------- */

.header-menu-toggle {
  display: none;
  position: fixed;
  right: 32px;
  top: 15px;
  height: 42px;
  width: 42px;
  line-height: 42px;
  font-family: "montserrat-regular", sans-serif;
  font-size: 1.4rem;
  text-transform: uppercase;
  letter-spacing: 0.2rem;
  color: rgba(255, 255, 255, 0.5);
  -webkit-transition: all 0.3s ease-in-out;
  transition: all 0.3s ease-in-out;
}

.header-menu-toggle:hover,
.header-menu-toggle:focus {
  color: #ffffff;
}

.header-menu-toggle span {
  display: block;
  width: 24px;
  height: 2px;
  margin-top: -1px;
  position: absolute;
  left: 9px;
  top: 50%;
  right: auto;
  bottom: auto;
  background-color: white;
  -webkit-transition: all 0.5s ease-in-out;
  transition: all 0.5s ease-in-out;
  font: 0/0 a;
  text-shadow: none;
  color: transparent;
}

.header-menu-toggle span::before,
.header-menu-toggle span::after {
  content: "";
  width: 100%;
  height: 100%;
  background-color: inherit;
  position: absolute;
  left: 0;
  -webkit-transition: all 0.5s ease-in-out;
  transition: all 0.5s ease-in-out;
}

.header-menu-toggle span::before {
  top: -9px;
}

.header-menu-toggle span::after {
  bottom: -9px;
}

.header-menu-toggle.is-clicked span {
  background-color: rgba(255, 255, 255, 0);
  -webkit-transition: all 0.1s ease-in-out;
  transition: all 0.1s ease-in-out;
}

.header-menu-toggle.is-clicked span::before,
.header-menu-toggle.is-clicked span::after {
  background-color: white;
}

.header-menu-toggle.is-clicked span::before {
  top: 0;
  -webkit-transform: rotate(135deg);
  -ms-transform: rotate(135deg);
  transform: rotate(135deg);
}

.header-menu-toggle.is-clicked span::after {
  bottom: 0;
  -webkit-transform: rotate(225deg);
  -ms-transform: rotate(225deg);
  transform: rotate(225deg);
}

/* ------------------------------------------------------------------- 
 * navigation - (_layout.scss) 
 * ------------------------------------------------------------------- */

#header-nav-wrap {
  font-family: "montserrat-medium", sans-serif;
  font-size: 14px;
  position: absolute;
  top: 0;
  right: 40px;
}

#header-nav-wrap .header-main-nav {
  display: inline-block;
  list-style: none;
  height: 72px;
  margin: 0 1rem 0 0;
}

#header-nav-wrap .header-main-nav li {
  display: inline-block;
  padding-left: 0;
  margin-right: 1.5rem;
}

#header-nav-wrap .header-main-nav li a {
  display: block;
  line-height: 72px;
}

#header-nav-wrap .header-main-nav li a,
#header-nav-wrap .header-main-nav li a:visited {
  color: rgba(255, 255, 255, 0.45);
}

#header-nav-wrap .header-main-nav li a:hover,
#header-nav-wrap .header-main-nav li a:focus {
  color: #ffffff;
}

#header-nav-wrap .header-main-nav li.current a {
  color: #ffffff;
}

#header-nav-wrap .cta {
  height: 3.6rem;
  line-height: calc(3.6rem - 0.6rem);
  padding: 0 1.5rem;
  font-family: "montserrat-medium", sans-serif;
  font-size: 14px;
  text-transform: none;
  letter-spacing: normal;
  margin: 0;
}

/* ------------------------------------------------------------------- 
 * responsive:
 * header
 * ------------------------------------------------------------------- */

@media only screen and (max-width: 1230px) {
  #header {
    max-width: none;
  }
}

@media only screen and (max-width: 768px) {
  .header-logo a {
    width: 88px;
    height: 20px;
    background-size: 88px 20px;
  }
  #header-nav-wrap {
    display: none;
    height: auto;
    width: 100%;
    right: auto;
    left: 0;
    background-color: #111111;
    padding: 120px 40px 54px;
  }
  #header-nav-wrap .header-main-nav {
    display: block;
    height: auto;
    margin: 0 0 4.2rem 0;
    border-top: 1px solid rgba(255, 255, 255, 0.03);
  }
  #header-nav-wrap .header-main-nav li {
    display: block;
    margin: 0;
    padding: 0;
    border-bottom: 1px solid rgba(255, 255, 255, 0.03);
  }
  #header-nav-wrap .header-main-nav li a {
    padding: 18px 0;
    line-height: 18px;
  }
  #header-nav-wrap .cta {
    height: 42px;
    line-height: calc(42px - 0.6rem);
    padding: 0 30px;
  }
  .header-menu-toggle {
    display: block;
  }
}

@media only screen and (max-width: 600px) {
  #header-nav-wrap .cta {
    display: block;
    padding: 0 20px;
  }
}

@media only screen and (max-width: 400px) {
  .header-menu-toggle {
    right: 24px;
  }
}

/* -------------------------------------------------------------------
 * make sure the menu is visible on larger screens
 * ------------------------------------------------------------------- */

@media only screen and (min-width: 769px) {
  #header-nav-wrap {
    display: block !important;
  }
}
</style>
