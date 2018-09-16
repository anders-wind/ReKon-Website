<template>
    <footer>

        <div class="footer-main">
            <div class="row">  

                <div class="col-three md-1-3 tab-full footer-info">            

                    <div class="footer-logo"></div>

                    <p>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque in ipsum id orci porta dapibus. Vivamus magna justo, lacinia eget consectetur sed, convallis at tellus. 
                    </p>

                    <ul class="footer-social-list">
                        <li>
                            <a href="#"><i class="fa fa-facebook-square"></i></a>
                        </li>
                        <li>
                            <a href="#"><i class="fa fa-twitter"></i></a>
                        </li>
                        <li>
                            <a href="#"><i class="fa fa-behance"></i></a>
                        </li>
                        <li>
                            <a href="#"><i class="fa fa-dribbble"></i></a>
                        </li>
                        <li>
                            <a href="#"><i class="fa fa-instagram"></i></a>
                        </li>
                    </ul>
                    
                    
                </div> <!-- end footer-info -->

                <div class="col-three md-1-3 tab-1-2 mob-full footer-contact">

                    <h4>Contact</h4>

                    <p>
                    1600 Amphitheatre Parkway<br>
                    Mountain View, CA <br>
                    94043 US<br>		        
                    </p>

                    <p>
                    someone@dazzlesite.com <br>
                    Phone: (+63) 555 1212 <br>
                    Fax: (+63) 555 0100    
                    </p>                    

                </div> <!-- end footer-contact -->  

                <div class="col-two md-1-3 tab-1-2 mob-full footer-site-links">

                    <h4>Site Links</h4>

                    <ul class="list-links">
                        <li><a href="#">Home</a></li>
                        <li><a href="#">About Us</a></li>
                        <li><a href="#">Blog</a></li>
                        <li><a href="#">FAQ</a></li>
                        <li><a href="#">Terms</a></li>
                        <li><a href="#">Privacy Policy</a></li>
                    </ul>	      		
                            
                </div> <!-- end footer-site-links --> 

                <div class="col-four md-1-2 tab-full footer-subscribe">

                    <h4>Our Newsletter</h4>

                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>

                    <div class="subscribe-form">
                
                        <form id="mc-form" class="group" novalidate="true">

                            <input type="email" value="" name="EMAIL" class="email" id="mc-email" placeholder="Email Address" required=""> 
                
                            <input type="submit" name="subscribe" value="Send">
                
                            <label for="mc-email" class="subscribe-message"></label>
                
                        </form>

                    </div>	      		
                            
                </div> <!-- end footer-subscribe -->         

            </div> <!-- /row -->
        </div> <!-- end footer-main -->


      <div class="footer-bottom">

      	<div class="row">

      		<div class="col-twelve">
	      		<div class="copyright">
		         	<span>© Copyright Anders Wind 2018.</span> 
		         	<span>Design by <a href="http://www.styleshout.com/">styleshout</a></span>		         	
		         </div>

		         <div id="go-top" style="display: block;">
		            <a class="smoothscroll" title="Back to Top" href="#top"><i class="fa fa-chevron-up"></i></a>
		         </div>         
	      	</div>

      	</div> <!-- end footer-bottom -->     	

      </div>

    </footer>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Footer extends Vue {
  @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
/* ===================================================================
 *  15. footer styles - (_site-layout.scss)
 *
 * ------------------------------------------------------------------- */
footer {
  padding-top: 9rem;
  padding-bottom: 4.2rem;
  font-size: 1.5rem;
  line-height: 2.7rem;
  color: rgba(255, 255, 255, 0.25);
}
footer a,
footer a:visited {
  color: #39b54a;
}
footer a:hover,
footer a:focus {
  color: white;
}
footer h4 {
  color: white;
  font-size: 1.5rem;
  padding-bottom: 2.4rem;
  margin-bottom: 2.4rem;
  position: relative;
}
footer h4::before {
  content: "";
  display: block;
  width: 120px;
  height: 1px;
  background-color: rgba(255, 255, 255, 0.05);
  position: absolute;
  left: 0;
  bottom: 0;
}
footer ul {
  list-style: none;
  margin: 0;
}
footer ul li {
  padding-left: 0;
}
footer ul a,
footer ul a:visited {
  color: rgba(255, 255, 255, 0.25);
}
.footer-logo {
  display: block;
  margin: 0 0 5.4rem 0;
  padding: 0;
  outline: 0;
  border: none;
  width: 93px;
  height: 21px;
  background: url("../assets/images/logo.png") no-repeat center;
  background-size: 93px 21px;
  font: 0/0 a;
  text-shadow: none;
  color: transparent;
  -webkit-transition: all 0.5s ease-in-out;
  transition: all 0.5s ease-in-out;
}
.footer-social-list {
  font-size: 1.8rem;
  margin-top: -1.5rem;
  margin-bottom: 3rem;
}
.footer-social-list li {
  display: inline-block;
  margin-right: 8px;
}
.footer-social-list li:last-child {
  margin-right: 0;
}
.footer-site-links .list-links {
  margin-bottom: 3rem;
}
.footer-subscribe .subscribe-form {
  margin: 0;
  padding: 0;
  position: relative;
}
.footer-subscribe #mc-form {
  width: 100%;
}
.footer-subscribe #mc-form input[type="email"] {
  width: 100%;
  height: 5.4rem;
  padding: 1.2rem 100px 1.2rem 60px;
  background: url(../assets/images/email-icon.png) 20px center no-repeat,
    rgba(0, 0, 0, 0.1);
  background-size: 24px 16px, auto;
  margin-bottom: 1.8rem;
  color: rgba(255, 255, 255, 0.5);
}
.footer-subscribe #mc-form input[type="email"]:focus {
  color: #ffffff;
}
.footer-subscribe #mc-form input[type="submit"] {
  position: absolute;
  top: 0;
  right: 0;
  color: #ffffff;
  background: #39b54a;
  border-color: #39b54a;
  border-radius: 0 0.5rem 0.5rem 0;
  padding: 0 15px;
}
.footer-subscribe #mc-form label {
  color: #ffffff;
  font-family: "montserrat-regular", sans-serif;
  font-size: 1.3rem;
  padding: 0 2rem;
}
.footer-subscribe #mc-form label i {
  padding-right: 6px;
}
.footer-subscribe #mc-form ::-webkit-input-placeholder {
  color: rgba(255, 255, 255, 0.2);
}
.footer-subscribe #mc-form :-moz-placeholder {
  color: rgba(255, 255, 255, 0.2); /* Firefox 18- */
}
.footer-subscribe #mc-form ::-moz-placeholder {
  color: rgba(255, 255, 255, 0.2); /* Firefox 19+ */
}
.footer-subscribe #mc-form :-ms-input-placeholder {
  color: rgba(255, 255, 255, 0.2);
}
.footer-subscribe #mc-form .placeholder {
  color: rgba(255, 255, 255, 0.2) !important;
}
.footer-bottom {
  margin-top: 6.6rem;
  text-align: center;
}
.footer-bottom .copyright span {
  display: inline-block;
}
.footer-bottom .copyright span::after {
  content: "|";
  display: inline-block;
  padding: 0 1rem 0 1.2rem;
  color: rgba(255, 255, 255, 0.1);
}
.footer-bottom .copyright span:last-child::after {
  display: none;
}

/* ------------------------------------------------------------------- 
 * go to top
 * ------------------------------------------------------------------- */
#go-top {
  position: fixed;
  bottom: 30px;
  right: 30px;
  z-index: 600;
  display: none;
}
#go-top a,
#go-top a:visited {
  text-decoration: none;
  border: 0 none;
  display: block;
  height: 60px;
  width: 60px;
  line-height: 60px;
  text-align: center;
  background: black;
  color: rgba(255, 255, 255, 0.5);
  text-align: center;
  text-transform: uppercase;
  border-radius: 5px;
  -webkit-transition: all 0.3s ease-in-out;
  transition: all 0.3s ease-in-out;
}
#go-top a i,
#go-top a:visited i {
  font-size: 18px;
  line-height: inherit;
}
#go-top a:hover,
#go-top a:focus {
  color: #ffffff;
}
/* ------------------------------------------------------------------- 
 * responsive:
 * footer 
 * ------------------------------------------------------------------- */
@media only screen and (max-width: 1024px) {
  .footer-main > .row {
    max-width: 800px;
  }
  .footer-info,
  .footer-contact,
  .footer-site-links {
    margin-bottom: 1.2rem;
  }
  .footer-subscribe {
    clear: both;
  }
}
@media only screen and (max-width: 768px) {
  .footer-main > .row {
    max-width: 600px;
  }
  .footer-logo {
    margin-left: auto;
    margin-right: auto;
  }
  .footer-info {
    text-align: center;
  }
  #go-top {
    bottom: 0;
    right: 0;
  }
  #go-top a,
  #go-top a:visited {
    border-radius: 5px 0 0 0;
  }
}
@media only screen and (max-width: 600px) {
  .footer-main .row {
    max-width: 480px;
  }
  .footer-main h4 {
    padding-bottom: 0;
    margin-bottom: 2.4rem;
  }
  .footer-main h4::before {
    display: none;
  }
  .footer-main ul.list-links {
    width: 80%;
    display: block;
    margin-left: auto;
    margin-right: auto;
  }
  .footer-main ul.list-links li a {
    display: block;
    border-bottom: 1px solid rgba(255, 255, 255, 0.03);
    padding: 0.6rem 0;
  }
  .footer-main ul.list-links li:first-child a {
    border-top: 1px solid rgba(255, 255, 255, 0.03);
  }
  .footer-contact,
  .footer-site-links,
  .footer-subscribe {
    text-align: center;
  }
  .footer-bottom {
    padding-bottom: 0.6rem;
  }
  .footer-bottom .copyright span {
    display: block;
  }
  .footer-bottom .copyright span::after {
    display: none;
  }
}
</style>
