 <template>
     <div class="home">
        <b-container fluid>
             <div class="section" id="home">
                

                </div>
                <div class="section" id="about">
                    <b-row align-h="center">
                        <b-col class="overlay" sm="3" md="6" lg="5">
                            <h2> <span>About Me</span></h2>
                            <p>
                                Hello! I'm Anthony, a software engineer based in Charlotte, NC 
                                who enjoys devloping projects that survive on the internet. I want to develop 
                                exceptional websites and web apps that provide intuitive, 
                                pixel-perfect user interfaces with efficient and modern backends.
                                </p>
                            <p>
                                Shortly after graduating frome the <a href="https://cci.uncc.edu/" target="_blank" rel="nofollow noopener noreferrer">Univeristy of North Carolina - Charlotte</a>
                                I would like to join and engineering team where I can work on a wide variety of interesting and meaninful projects on a daily basis. 
                            </p>    

                            <p>
                                Here is a few technologies I've come familar with over my software engineering career. 
                            </p>    
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
                
                <div class="section" id="projects">
                <h3> <span>Projects</span></h3>
                <b-carousel
                    id="carousel-1"
                    v-model="slide"
                    :interval="4000"
                    controls
                    indicators
                    background="#ababab"
                    img-width="1024"
                    img-height="480"
                    style="text-shadow: 1px 1px 2px #333;"
                    @sliding-start="onSlideStart"
                    @sliding-end="onSlideEnd"
                    >
                    <!-- Text slides with image -->
                    <b-carousel-slide
                        caption="First slide"
                        text="Nulla vitae elit libero, a pharetra augue mollis interdum."
                        img-src="https://media.giphy.com/media/d2ZhZTK55EA2yvTy/giphy.gif"
                    ></b-carousel-slide>

                    <!-- Slides with custom text -->
                    <b-carousel-slide
                        caption="Second slide"
                        text="Nulla vitae elit libero, a pharetra augue mollis interdum."
                        img-src="https://media.giphy.com/media/d2ZhZTK55EA2yvTy/giphy.gif"
                    ></b-carousel-slide>

                    <!-- Slides with image only -->
                    <b-carousel-slide
                        caption="Third slide"
                        text="Nulla vitae elit libero, a pharetra augue mollis interdum."
                        img-src="https://media.giphy.com/media/d2ZhZTK55EA2yvTy/giphy.gif"
                    ></b-carousel-slide>
                     <b-carousel-slide
                        caption="Forth slide"
                        text="Nulla vitae elit libero, a pharetra augue mollis interdum."
                        img-src="https://media.giphy.com/media/d2ZhZTK55EA2yvTy/giphy.gif"
                    ></b-carousel-slide>
                    </b-carousel>
                </div>
                
                <div class="section" id="contact">
                <h3> <span>Contact Me</span></h3><br>
            <form action="action_page.php">

                <label for="fname">First Name</label><br>
                <input type="text" id="fname" name="firstname" placeholder="Your name..">

                <br><label for="lname">Last Name</label><br>
                <input type="text" id="lname" name="lastname" placeholder="Your last name..">

                <br><label for="email">E-Mail</label><br>
                <input type="email" id="email" name="email" placeholder="Your E-Mail">

                <br><label for="country">Country</label><br>
                <select id="country" name="country">
                <option value="australia">Australia</option>
                <option value="canada">Canada</option>
                <option value="usa">USA</option>
                </select>

                <br><label for="subject">Subject</label><br>
                <textarea id="subject" name="subject" placeholder="Write something.." style="height:200px"></textarea><br>

                <br><input type="submit" value="Submit">

            </form>
            </div>
            </b-container>
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
            } 
        }
    }
            </script>
            <style>
            img{
                max-width: 500px;
            }

            #carousel-1{
                height: calc(100vh - 195px) !important;
                position: relative;
            }

            #carousel-1___BV_inner_, .carousel-item, .carousel-item img{
                height: 100%;
            }
            #about:hover{
            
            transition: all .3s ease-in-out;
            }

          
            .overlay{
                
                padding: 25px;
            }
        

            .section{
                padding-top: 85px;
                padding-left: 20px;
                padding-right: 20px;
                width: 100%;
                min-height: 100vh;
                
                z-index: -1;
            }
            h1, h2, h3, h4, h5 {
            font-family: 'Playfair Display', serif !important;
            margin: auto;
            text-align: center;
            font-size: 40px;
            
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
    background-color: #4CAF50;
    color: white;
    padding: 12px 20px;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    }

    /* When moving the mouse over the submit button, add a darker green color */
input[type=submit]:hover {
    background-color: #45a049;
    }

    #about{
                background-image: linear-gradient(0deg,rgba(0, 0, 0, 0.808)),url(https://media.giphy.com/media/26uf7tKxfa0xfaw48/giphy.gif);
                background-size:cover;
                background-attachment: fixed;
                background-position:center;
                background-color: rgba(0, 0, 0, 0.808);
            }
    #projects{
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
            }
            </style>