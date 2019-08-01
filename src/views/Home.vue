 
<template>
	<div>
		<b-container id="home">
			<b-row  align-h="center" align-v="center">
				<b-col class="home-content">
					<h3>Hi, my name is </h3>
					<h2>Anthony Peterson
						<span style="padding-left:.08em;">.</span>
					</h2>
					<br>
						<h1>I build things for the web
							<span style="padding-left:.05em;">.</span>
						</h1>
						<p>I'm a passionate software engineer based in Charlotte, NC who's always challenging myself to improve my skills, whether that be in my programming or video game playing.</p>
						<p>Check out my 
							<a v-on:click="scrollTo('preScroll',1,'work')">work</a> below and feel free to 
							<a v-on:click="scrollTo('preScroll',2,'contact')">contact me</a> via email.
						</p>
					</b-col>
				</b-row>
				<div id="scrollAlert" v-on:click="scrollTo(null,null,'carousel-wrapper')">
					<h5>SCROLL DOWN</h5>
					<img src="../assets/DownIcon.png" width="25px" height="20px"/>
				</div>
			</b-container>
			<div class="home">
				<div class="email__EmailContainer-sc-2epoq-0 eGMGzG">
					<div>
						<div class="email__EmailLinkWrapper-sc-2epoq-1 hUtUVZ fade-enter-done">
							<a href="mailto:antmpeterson@gmail.com" class="email__EmailLink-sc-2epoq-2 dzAcvq">Antmpeterson@gmail.com</a>
						</div>
					</div>
				</div>
				<div data-v-bbb28d14="" class="social-links-container">
					<div data-v-bbb28d14="">
						<ul data-v-bbb28d14="" class="social-links-list">
							<li data-v-bbb28d14="" class="social-links-item">
								<a data-v-bbb28d14="" href="https://github.com/antmpeterson" target="_blank" rel="nofollow noopener noreferrer" aria-label="Github" class="social-link-item-icon">
									<svg data-v-bbb28d14=""
										xmlns="http://www.w3.org/2000/svg" role="img" viewBox="0 0 438.549 438.549">
										<title data-v-bbb28d14="">Github</title>
										<path data-v-bbb28d14="" d="M409.132,114.573c-19.608-33.596-46.205-60.194-79.798-79.8C295.736,15.166,259.057,5.365,219.271,5.365 c-39.781,0-76.472,9.804-110.063,29.408c-33.596,19.605-60.192,46.204-79.8,79.8C9.803,148.168,0,184.854,0,224.63 c0,47.78,13.94,90.745,41.827,128.906c27.884,38.164,63.906,64.572,108.063,79.227c5.14,0.954,8.945,0.283,11.419-1.996 c2.475-2.282,3.711-5.14,3.711-8.562c0-0.571-0.049-5.708-0.144-15.417c-0.098-9.709-0.144-18.179-0.144-25.406l-6.567,1.136 c-4.187,0.767-9.469,1.092-15.846,1c-6.374-0.089-12.991-0.757-19.842-1.999c-6.854-1.231-13.229-4.086-19.13-8.559 c-5.898-4.473-10.085-10.328-12.56-17.556l-2.855-6.57c-1.903-4.374-4.899-9.233-8.992-14.559 c-4.093-5.331-8.232-8.945-12.419-10.848l-1.999-1.431c-1.332-0.951-2.568-2.098-3.711-3.429c-1.142-1.331-1.997-2.663-2.568-3.997 c-0.572-1.335-0.098-2.43,1.427-3.289c1.525-0.859,4.281-1.276,8.28-1.276l5.708,0.853c3.807,0.763,8.516,3.042,14.133,6.851 c5.614,3.806,10.229,8.754,13.846,14.842c4.38,7.806,9.657,13.754,15.846,17.847c6.184,4.093,12.419,6.136,18.699,6.136 c6.28,0,11.704-0.476,16.274-1.423c4.565-0.952,8.848-2.383,12.847-4.285c1.713-12.758,6.377-22.559,13.988-29.41 c-10.848-1.14-20.601-2.857-29.264-5.14c-8.658-2.286-17.605-5.996-26.835-11.14c-9.235-5.137-16.896-11.516-22.985-19.126 c-6.09-7.614-11.088-17.61-14.987-29.979c-3.901-12.374-5.852-26.648-5.852-42.826c0-23.035,7.52-42.637,22.557-58.817 c-7.044-17.318-6.379-36.732,1.997-58.24c5.52-1.715,13.706-0.428,24.554,3.853c10.85,4.283,18.794,7.952,23.84,10.994 c5.046,3.041,9.089,5.618,12.135,7.708c17.705-4.947,35.976-7.421,54.818-7.421s37.117,2.474,54.823,7.421l10.849-6.849 c7.419-4.57,16.18-8.758,26.262-12.565c10.088-3.805,17.802-4.853,23.134-3.138c8.562,21.509,9.325,40.922,2.279,58.24 c15.036,16.18,22.559,35.787,22.559,58.817c0,16.178-1.958,30.497-5.853,42.966c-3.9,12.471-8.941,22.457-15.125,29.979 c-6.191,7.521-13.901,13.85-23.131,18.986c-9.232,5.14-18.182,8.85-26.84,11.136c-8.662,2.286-18.415,4.004-29.263,5.146 c9.894,8.562,14.842,22.077,14.842,40.539v60.237c0,3.422,1.19,6.279,3.572,8.562c2.379,2.279,6.136,2.95,11.276,1.995 c44.163-14.653,80.185-41.062,108.068-79.226c27.88-38.161,41.825-81.126,41.825-128.906 C438.536,184.851,428.728,148.168,409.132,114.573z"></path>
									</svg>
								</a>
							</li>
							<li data-v-bbb28d14="" class="social-links-item">
								<a data-v-bbb28d14="" href="https://www.linkedin.com/in/anthony-peterson-473767129/" target="_blank" rel="nofollow noopener noreferrer" aria-label="Linkedin" class="social-link-item-icon">
									<svg data-v-bbb28d14=""
										xmlns="http://www.w3.org/2000/svg" role="img" viewBox="0 0 430.117 430.117">
										<title data-v-bbb28d14="">LinkedIn</title>
										<path data-v-bbb28d14="" d="M430.117,261.543V420.56h-92.188V272.193c0-37.271-13.334-62.707-46.703-62.707 c-25.473,0-40.632,17.142-47.301,33.724c-2.432,5.928-3.058,14.179-3.058,22.477V420.56h-92.219c0,0,1.242-251.285,0-277.32h92.21 v39.309c-0.187,0.294-0.43,0.611-0.606,0.896h0.606v-0.896c12.251-18.869,34.13-45.824,83.102-45.824 C384.633,136.724,430.117,176.361,430.117,261.543z M52.183,9.558C20.635,9.558,0,30.251,0,57.463 c0,26.619,20.038,47.94,50.959,47.94h0.616c32.159,0,52.159-21.317,52.159-47.94C103.128,30.251,83.734,9.558,52.183,9.558z M5.477,420.56h92.184v-277.32H5.477V420.56z"></path>
									</svg>
								</a>
							</li>
						</ul>
					</div>
				</div>
				<b-container fluid>
					<div class="section" id="about">
						<b-row align-h="center">
							<b-col class="overlay" sm="3" md="6" lg="5">
								<h2>
									<span>About Me</span>
								</h2>
								<p>
                                Hello! I'm Anthony, a software engineer based in Charlotte, NC 
                                who enjoys devloping projects that survive on the internet. I want to develop 
                                exceptional websites and web apps that provide intuitive, 
                                pixel-perfect user interfaces with efficient and modern backends.
                                </p>
								<p>
                                Shortly after graduating frome the 
									<a href="https://cci.uncc.edu/" target="_blank" rel="nofollow noopener noreferrer">Univeristy of North Carolina - Charlotte</a>
                                I would like to join and engineering team where I can work on a wide variety of interesting and meaninful projects on a daily basis. 
                            
								</p>
								<h3>Technical Skills</h3>
								<div class="skill-wrapper">
									<ul class="about-skill-container">
										<li class="about-skill">Java</li>
										<li class="about-skill">C++</li>
										<li class="about-skill">HTML &amp; (S)CSS</li>
										<li class="about-skill">JavaScript (ES6+)</li>
										<li class="about-skill">TypeScript</li>
										<li class="about-skill">Angular</li>
										<li class="about-skill">React</li>
										<li class="about-skill">Vue</li>
										<li class="about-skill">Node.js</li>
										<li class="about-skill">Express</li>
									</ul>
								</div>
							</b-col>
							<b-col sm="3" md="6" lg="5">
								<div>
									<a href = " https://github.com/antmpeterson">
										<img src="../assets/IMG_0519.jpg" width="100%" alt="Responsive image"/>
									</a>
								</div>
							</b-col>
						</b-row>
					</div>
						<div class="caro-contain" id = "caro-contain">
							<div id="carousel-wrapper" >
								<div id="carousel">
									<div class="section" id="slide1">
										<b-container fluid >
											<h4>Portfilo Website</h4>
                                            <b-row align-h="center">
                                            <b-col class="overlay" sm="3" md="6" lg="5">
                                                <p>
                                                    This is one of my first projects. It was created in a Vue framework and written in HTML5, CSS, and JavaScript. 
                                                    The overall project was started so I could display my programming skills, while also creating a way to get my name thrown into the programming industry. 
                                                </p>
                                                <p>


                                                    The code for this project can be seen on my Github. Try clicking the photo of me above or using the social link located on the lefthand side of the screen. 

                                                </p>
                                            </b-col>
                                            <b-col sm="3" md="6" lg="5">
                                                <img src="../assets/png.png" width="100%" alt="Responsive image"/>
                                            </b-col>
                                            </b-row>  
										</b-container>
									</div>
									<div class="section" id="slide2">
										<b-container fluid>
											<h4>PrestigePlug.com</h4>
                                            <b-row align-h="center">
                                            <b-col class="overlay" sm="3" md="6" lg="5">
                                                <p>
                                                    The PrestigePlug website was the second programming project that I took on. I created this website for a local Charlotte entrepreneur. 
                                                    It also was built in a Vue environment with similar languages such as HTML5, 
                                                    CSS, and JavaScript. However, in this project I let my creative side shine with 
                                                    custom logos and images that were created in Adobe Photoshop and Illustrator.
                                                </p>
                                                <p>
                                                    This website is not currently up and running yet. Although you can keep up with my progress on this site all the code will be on my Github.  
                                                </p>

                                            </b-col>
                                            <b-col sm="3" md="6" lg="5">
                                                <img src="../assets/FINAL.png" width="100%" alt="Responsive image"/>
                                            </b-col>  
                                            </b-row>
										</b-container>
									</div>
									<div class="section" id="slide3">
										<b-container fluid>
											<h4>Event Manger Application</h4>
                                            <b-row align-h="center">
                                            <b-col class="overlay" sm="3" md="6" lg="5">
                                                <p>
                                                    This is the most recent project that I have taken on. So far no code has been published this project is still in 
                                                    the pre-planning phase. As of now, this application will be a phone app that allows the user to publish events to a
                                                     calendar and send notifications as the date gets closer. Once the ball gets rolling on this project all the necessary
                                                     code will be published on my Github.
                                                </p>
                                            </b-col>
                                            <b-col sm="3" md="6" lg="5">
                                                <img src="https://media.giphy.com/media/oFDSjMfe11iiOgQRfY/giphy.gif" width="100%" alt="Responsive image"/>
                                            </b-col> 
                                            </b-row> 
										</b-container>
									</div>
								</div>
							</div>
							<div id="slide-changer">
								<div id="slide-1" v-on:click="scrollTo('slide1')" class="selected"></div>
								<div id="slide-2" v-on:click="scrollTo('slide2')"></div>
								<div id="slide-3" v-on:click="scrollTo('slide3')"></div>
							</div>
						</div>
					<div class="section" id="contact">
						<h3>
							<span>Contact Me</span>
						</h3>
						<br>
							<form action="action_page.php">
								<input type="text" id="fname" name="firstname" placeholder="Your name..">
									<br>
										<input type="text" id="lname" name="lastname" placeholder="Your last name..">
											<br>
												<input type="email" id="email" name="email" placeholder="Your E-Mail">
													<br>
														<textarea id="subject" name="subject" placeholder="Write something.." style="height:200px"></textarea>
														<br>
															<br>
																<a href="mailto:antmpeterson@gmail.com">
																	<input type="submit" value="Submit">
																	</a>
																</form>
															</div>
														</b-container>
													</div>
												</div>
											</template>
											<script>
            // @ is an alias to /src
            import $ from "jquery";

            export default {
            
                data() {
                    return {
                    slide: 0,
                    sliding: null
                }
            },
            methods: {
            onSlideStart(slide) {
            this.sliding = true
            },
            onSlideEnd(slide) {
            this.sliding = false
            } ,

            scrollTo(element) {

        this.selectedSlide.classList.remove('selected');

        var carousel = document.getElementById('carousel-wrapper');

          switch(element){
            case 'slide1':
              this.selectedSlide = this.slide1;
              this.counter = 0;
              document.getElementById('slide-1').classList.add('selected');
              carousel.scroll({
                left: 0, 
                behavior: 'smooth'
              });
              break;
            case 'slide2':
              this.selectedSlide = this.slide2;
              this.counter = 1;
              document.getElementById('slide-2').classList.add('selected');
              carousel.scroll({
                left: window.innerWidth, 
                behavior: 'smooth'
              });
              break;
            case 'slide3':
              this.selectedSlide = this.slide3;
              this.counter = 2;
              document.getElementById('slide-3').classList.add('selected');
              carousel.scroll({
                left: window.innerWidth * 2, 
                behavior: 'smooth'
              });
              break;
          }
    } ,








resizeSnap(){
      document.getElementById('carousel-wrapper').scroll({
        left: window.innerWidth * this.counter
      });
    } 
    

 
        } ,
        mounted(){
      this.slide1 = document.getElementById('slide-1');
      this.slide2 = document.getElementById('slide-2');
      this.slide3 = document.getElementById('slide-3');
      this.selectedSlide = this.slide1;
      this.selectedSlide.classList.add('selected');
      window.scroll({
        top: 0, 
        left: 0
      });
  }
    }
            </script>
											<style>

#home{
  width: 100vw;
  padding: 0px 2em;
  top: 0px;
}

#home *{
    text-align: left ;
    
}

#home .row{
  height: 100vh;
}
.home-content *{
  max-width: 600px;
  margin: auto !important;
}

.home-content p{
  max-width: 600px;
}
#home h3{
  font-size: 1.0em;
  color: rgb(255, 193, 47) !important;
  margin-bottom: 8px;
}
#home h1, #home h2{
  font-size: 2.5em;
  font-weight: 900;
  padding: 0px 20px;
}

#home h3, #home h2{
  padding: 0px 20px;
}

#home h1{
  margin-top: -.42em !important;
  margin-bottom: 30px !important;
  color: rgb(146, 152, 185) !important;
}

#scrollAlert{
  position: absolute;
  left: 50%;
  bottom: 50px;
  transform: translateX(-50%);
  animation-name: hover;
  animation-duration: 2s;
  animation-fill-mode: both;
  animation-timing-function: ease-out;
  animation-iteration-count: infinite;
  animation-direction: alternate-reverse;
  text-align:center;
}

#home h5{
  font-size: .9em;
  margin-bottom: 3px;
}

@keyframes hover {
  from{
    transform: translateX(-50%);
  }
  to{
    transform: translate(-50%, 30%);
  }
}

@keyframes slide {
  0%{
    width: 0px;
    height: 0px;
    border-radius: 100vw;
    opacity: 1;
  }
  100%{
    width: 120vw;
    height: 120vw;
    border-radius: 0px;
    opacity: 1;
  }
}




   .social-links-container{
        width: 40px;
        display: block !important;
        position: fixed;
        z-index: 10;
        bottom: 0px;
        left: 40px;
        color: rgb(168, 178, 209);
    }    

    .social-links-list {
        display: flex;
        flex-direction: column;
        -webkit-box-align: center;
        align-items: center;
        margin-bottom: 0px !important; 
         z-index: 10;

    }

    .social-links-list::after {
        content: "";
        display: block;
        width: 1.2px;
        height: 90px;
        background-color: rgb(168, 178, 209);
        margin: 0px auto;
        margin-top: 35px;
         z-index: 10;
    }

    ul, ol {
        padding: 0px;
        margin: 0px;
        list-style: none;
    }

    li {
      

        display: list-item;
        text-align: -webkit-match-parent;
    }

    .social-links-item {
        padding: 10px;
    }



    .social-links-item svg {
        width: 18px;
        height: 18px;
        fill: currentcolor;
        vertical-align: middle;
    }

            img{
                max-width: 500px;
            }

           
            #about:hover{
            
            transition: all .3s ease-in-out;
            }

          
            .overlay{
                
                padding: 20px;
            }
        

            .section{
                padding-top: 85px;
                padding-left: 20px;
                padding-right: 20px;
                width: 100%;
                min-height: 100vh;
                box-sizing: border-box;
                z-index: -1;
            }
            h1, h2, h3, h4, h5 {
            font-family: 'Playfair Display', serif !important;
            margin: auto;
            text-align: center;
            position: relative;
            color: rgb(230, 241, 255);
            
            }
            
            *, ::before, ::after {
                box-sizing: inherit;
            }
            p {
                display: block;
                margin-block-start: 1em;
                margin-block-end: 1em;
                margin-inline-start: 0px;
                margin-inline-end: 0px;
                margin: 0px 0px 15px;
                padding: 20px;
                text-align: left;
                font-size: 20px !important;
            }
.eGMGzG {
    width: 40px;
    position: fixed;
    bottom: 0px;
    right: 40px;
    color: rgb(168, 178, 209);
     z-index: 10;
}

.dzAcvq {
    font-family: "SF Mono", "Fira Code", "Fira Mono", "Roboto Mono", "Lucida Console", Monaco, monospace;
    font-size: 12px;
    letter-spacing: 0.5px;
    -webkit-writing-mode: vertical-rl;
    writing-mode: vertical-rl;
    margin: 20px auto;
    padding: 10px;
     z-index: 10;
}

.hUtUVZ::after {
    content: "";
    display: block;
    width: 2px;
    height: 90px;
    background-color: rgb(168, 178, 209);
    margin: 0px auto;
     z-index: 10;
}

input[type=text], select, textarea {
    width: 50%; /* Full width */
    padding: 12px; /* Some padding */  
    border: 1px solid #ccc; /* Gray border */
    border-radius: 4px; /* Rounded borders */
    box-sizing: border-box; /* Make sure that padding and width stays in place */
    margin-top: 6px; /* Add a top margin */
    margin-bottom: 16px; /* Bottom margin */
    resize: vertical /* Allow the user to vertically resize the textarea (not horizontally) */
    }
input[type=email] {
    width: 50%; /* Full width */
    padding: 12px; /* Some padding */  
    border: 1px solid #ccc; /* Gray border */
    border-radius: 4px; /* Rounded borders */
    box-sizing: border-box; /* Make sure that padding and width stays in place */
    margin-top: 6px; /* Add a top margin */
    margin-bottom: 16px; /* Bottom margin */
    resize: vertical /* Allow the user to vertically resize the textarea (not horizontally) */
    }


    /* Style the submit button with a specific background color etc */
input[type=submit] {
    background-color:rgb(255, 193, 47) !important;
    color: white;
    padding: 12px 20px;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    }

    /* When moving the mouse over the submit button, add a darker green color */
input[type=submit]:hover {
    background-color: rgb(158, 113, 9) !important;
    }
.skill-wrapper{
  margin: auto;
  display: inline-block;
  
}


.about-skill-container{
 
  display: grid;
  grid-template-columns: minmax(140px, 150px) minmax(140px, 150px);
  margin-top: 20px;
  overflow: hidden;
  
  
}

.about-skill{
  position: relative;
  margin-bottom: 10px;
  margin-left: 0px;
  width: 150px;
  text-decoration: none;
}

.about-skill::before {
    content: "▹";
    position: absolute;
    left: 0px;
    color: rgb(255, 193, 47);
    font-size: 14px;
    padding-top: 9px;
    line-height: 12px;
    
}

h3 hr{
  position: absolute;
  background-color:rgba(82, 82, 82, 0.726);
  display: inline-block;
  width: calc(50% - 95px);
  right: 0px;
  padding: .5px;

}

h3 hr:first-child{
  position: absolute;
  left: 0px;
  background-color:rgba(82, 82, 82, 0.726);
  display: inline-block;
  margin-left: 15px;
  width: calc(50% - 110px);
  padding: .5px;
}
ul.about-skill{
    text-decoration: none;

}


    #about{
                background-image: linear-gradient(0deg,rgba(0, 0, 0, 0.808)),url(https://media.giphy.com/media/26uf7tKxfa0xfaw48/giphy.gif);
                background-size:cover;
                background-attachment: fixed;
                background-position:center;
                background-color: rgba(0, 0, 0, 0.808);
            }
    #caro-contain{
                background-image: linear-gradient(0deg,rgba(0, 0, 0, 0.808)),url(https://media.giphy.com/media/26uf7tKxfa0xfaw48/giphy.gif);
                background-size:cover;
                background-attachment: fixed;
                background-position:center;
                background-color: rgba(0, 0, 0, 0.808);
            }
    #contact{
                background-image: linear-gradient(0deg,rgba(0, 0, 0, 0.808)),url(https://media.giphy.com/media/26uf7tKxfa0xfaw48/giphy.gif);
                background-size:cover;
                background-attachment: fixed;
                background-position:center;
                background-color: rgba(0, 0, 0, 0.808);
                margin: 25px;
                
            }

            @media only screen and (max-width : 1024px) {
                .social-links-container, .eGMGzG{
                    display: none !important;
                }
            }
            .caro-contain{
  max-width: 100vw;
  max-height: 100vh;
  position: relative;
}


#carousel-wrapper{
  height: 100vh;
  overflow: hidden;
  overflow-y: scroll;
  position: relative;
}

#carousel{
  width: 301vw;
}

#carousel .section{
  width: 100vw;
  float: left;
  padding-top: 120px;
}


#slide-changer{
  width:100vw;
  height:50px;
  box-sizing: border-box;
  padding-top: 8px;
  position: absolute;
  bottom: 0em;
  left: 50%;
  transform: translateX(-50%);
  z-index: 0;
  background-color: rgba(255, 193, 47, 0.74);
  
}

#slide-changer div{
  width: 11px;
  height: 11px;
  background-color: rgba(255, 255, 255, 0.801);
  display: inline-block;
  margin: 10px 15px;
  transform: rotate(45deg);
}

.selected{
  background-color: rgba(0, 0, 0, 0.911) !important;
  pointer-events: none;
}

#slide-changer div:hover{
  cursor: pointer;
}
#about img {
    padding-top: 25px;
}

#caro-contain img {
    padding-top: 25px;
}
#about h3 {
    margin-top: 0px !important ;
    font-size: 28px !important ;
}
#contact h3 {
    margin: 50px !important;
}
            </style>