# PORTFOLIO<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio</title>
    <link rel="stylesheet" href="stylee.css">
    <script src="https://kit.fontawesome.com/a973db36d5.js" crossorigin="anonymous"></script>
</head>

<body>
    <section id="navbar">
        <div class="nav-logo">
            <img src="https://cdn2.vectorstock.com/i/thumb-large/19/41/initial-pa-letter-logo-creative-typography-vector-35581941.jpg" alt="logo">
        </div>
        <nav class="nav-btn">
            <ul id="sidemenu">
            <div class="nav-item"><a href="#header">HOME</a></div>
            <div class="nav-item"><a href="#about">ABOUT</a></div>
            <div class="nav-item"><a href="/blog.html">BLOG</a></div>
            <div class="nav-item"><a href="/contact.html">CONTACT </a></div>
            <i class="fas fa-times" onclick="closeMenu()"></i>
            <!-- <i class="fa-solid fa-bars nav-icon" onclick="openMenu()"></i>
            <i class="fa-solid fa-xmark nav-icon" onclick="closeMenu()"></i> -->
            </ul>
            <i class="fas fa-bars" onclick="openMenu()"></i>
        </nav>
    </section>

    <section id="header">
        <div>
            <img class="head-img" src="akshat3.jpg" alt="logo">
        </div>
        <div>
            <h1 class="head-h1">AKSHAT PANDEY</h1>
            <h3 class="head-h2">I'm a Web</h3>
            <h3 class="head-h3">Developer</h3>
            <p class="head-p1">Currently enroled as a student in the KIET GROUP OF INSTITUTIONS GZB, a technical
                institute affiliated to Dr.APJ Abdul Kalam Technical University Lucknow pursuing an undergraduate degree.
                I am interested in Tech fields and seeking the exciting opportunity related to the same.
            </p>
            <a href="./src/AkshatCV.docx" download class="btn">Download CV</a>
        </div>

    </section>

    <section id="about">
        <div class="about-img">
            <img class="head-img" src="akshat1.jpg" width:50px; height:90px; position:right alt="logo">
        </div>
        <div class="about">
            <h1 class="about-h1">About <span>Me</span></h1>
            <h3 class="about-h2">Hello I'm Akshat Pandey</h3>
            <p class="about-p1">A Recent college graduating seeking an entry-level position in the field of IT. 
                Possesses a strong academic record, eager to put my skills to work in a professional setting.
                Gained valuable experience through internships and volunteer work.</p>
            <div class="tab-titles">
                <p class="tab-links active-link" onclick="opentab('Skills')">Skills</p>
                <p class="tab-links"onclick="opentab('Experience')">Experience</p>
                <p class="tab-links"onclick="opentab('Education')">Education</p>
            </div>
            <div class="tab-contents active-tab" id="Skills">
                <ul>
                    <li><span>UI?UX</span><br>Desigining Web/App interfaces</li>
                    <li><span>Web Development</span><br>Desigining Web/App development</li>
                    <li><span>App Development</span><br>Desigining Building Android/iOS apps</li>
                </ul>
            </div>
            <div class="tab-contents" id="Experience">
                <ul>
                    <li><span>2022- Current</span><br>Desigining Web Portfolio</li>
                    <li><span>2019-2020</span><br>Done 12th board with 91.4%</li>
                    <li><span>2017-2018</span><br>Done high school with 92.6%</li>
                </ul>
            </div>
            <div class="tab-contents" id="Education">
                <ul>
                    <li><span>2022-Current</span><br>Desigining My first Project</li>
                </ul>
            </div>
            <!-- <div class="about-icon">
                <i class="fa-brands fa-whatsapp"></i>
                <i class="fa-brands fa-instagram"></i>
                <i class="fa-brands fa-linkedin"></i>
            </div> -->
        </div>
    </section>

    <section id="footer">
        <div>
            <ul>
                <li><i class="fa-solid fa-location-dot"></i><span> KIET,Delhi-NCR, Ghaziabad-Meerut Road
                        Ghaziabad-201206</span></li>
                <li><i class="fa-solid fa-phone"></i><span> +91 7302821512</span></li>
                <li><i class="fa-solid fa-envelope"></i><span> santoshandom7922@gmail.com</span></li>
                <li><i class="fa-brands fa-github"></i><span> Github</span></li>
            </ul>
        </div>
        <div>
            <h1 class="about-h2" style="text-align: center;">Connect with me</h1>
            <ul>
                <li><i class="fa-brands fa-whatsapp"></i><span>Whatsapp</span>
                <li><i class="fa-brands fa-instagram"></i><span>Instagram</span> </li>
                <li> <i class="fa-brands fa-linkedin"></i><span>Linkedin</span></li>
            </ul>
        </div>
    </section>
    <!-- <hr> -->

    <script>
        var tablinks=document.getElementsByClassName("tab-links");
        var tabcontents=document.getElementsByClassName("tab-contents");

        function opentab(tabname){
            for(tablink of tablinks){
                tablink.classList.remove("active-link");
            }
            for(tabcontents of tabcontents){
                tabcontents.classList.remove("active-tab");
            }
            event.currentTarget.classList.add("active-link");
            document.getElementById(tabname).classList.add("active-tab");
        }
    </script>
    <script>
        var sidemeu = document.getElementById("sidemenu");

        function openmenu(){
            sidemeu.style.right="0";
        }
        function closemenu(){
            sidemeu.style.right="-200px";
        }
    </script>
    <script>
        const scriptURL = 'https://script.google.com/macros/s/AKfycbxn1x9gvkmWAzoMu6B2J9t1yBwwnQrQ9_bzy3FbExVaXzdirUUhWS5NGZEq5GfaMkRE3Q/exec'
        const form = document.forms['submit-to-google-sheet']
      
        form.addEventListener('submit', e => {
          e.preventDefault()
          fetch(scriptURL, { method: 'POST', body: new FormData(form)})
            .then(response => console.log('Success!', response))
            .catch(error => console.error('Error!', error.message))
        })
      </script>
</body>
</html>









body {
  color: grey;
  font-family: "Poppins", sans-serif;
  font-size: 14px;
  font-weight: 300;
  line-height: 1.625em;
  margin: 0;
}

/* Navbar css start */

#navbar {
  display: flex;
  justify-content: space-between;
  margin: 1%;
  cursor: pointer;
}

.nav-btn {
  display: flex;
  margin: 0 1% 0 10%;
  cursor: pointer;
  
}

.nav-logo {
  margin-left: 32px;
}

.nav-item {
  margin-left: 50px;
  margin-right: 50px;
  font-size: 20px;
  justify-items: center;
  cursor: pointer;
}

.btn{
  background: -webkit-linear-gradient(0deg, #8490ff 0%, #62bdfc 100%);
    font-size: 20px;
    border: none;
    color: #fff;
    font-weight: 500;
    border-radius: 6px;
    padding: 10px;
}


.buttons button:hover{ 
  background-color: rgb(63, 6, 6);
  color: #6bcf0d ;
}

a {
  text-decoration: none;
}

nav.fa-solid {
  display: none;
}

i.fas{
  display: none;
}

/* @media screen and (max-width: 480px) {
  .nav-btn{
      display: none;
      cursor: pointer;
  }
  i.fas{
    display:block;
    font-size: 25px;
  }
} */
  /* nav .fa-solid {
      display: block;
      position:absolute;
      top:25px;
      left:25px;
  }
  nav ul{
      background-color: #62bdfc;
      position: fixed;
      top:0;
      height: 100vh;
      right: -200px;
      padding-top: 50px;
      transition: right .5s;
      z-index: 2;
  }
} */

/* Navbar css ends */

/* Header css start */
#header {
  display: flex;
  padding: 10px 60px;
  background-color: black;
  border-radius: 1.5%;
}

.head-img {
  width: 90%;
  border-radius: 18px;
  /* height: 10; */
}

.head-h1 {
  font-size: 30px;
}

.head-h2 {
  font-size: 70px;
  color: #fff;
}

.head-h3 {
  font-size: 70px;
}

.head-p1 {
  font-size: 20px;
  margin-bottom: 45px;
}

/* @media screen and (max-width: 480px) {
  #header {
      display: block;
  }

  .head-h2,
  .head-h1,
  .head-h3 {
      line-height: 60px;
      font-size: 40px;
  }
} */

/* Header css ends */

/* About section css started */
#about {
  display: flex;
}

.about {
  margin: 5%;
  /* text-align: center; */
}

.about-h1 {
  font-size: 60px;
}

.about-h2 {
  font-size: 30px;
}

.about-p1 {
  font-size: 20px;
}

.about-img {
  margin: 5%;
}

.about-icon {
  font-size: 30px;
  font-weight: 900;
}

/* @media screen and (max-width: 480px) {
  #about {
      display: block;
  }
} */

/* About section css ends */

/* Footer section section css start */
#footer {
  display: flex;
  background-color: black;
  justify-content: space-evenly;
  border-radius: 5px;
  padding: 20px;
}

li {
  list-style: none;
  margin-bottom: 20px;
}

.fa-solid,
.fa-brands {
  font-size: 40px;
  margin-right: 10px;
}

ul {
  padding: 0;
}


/* @media screen and (max-width: 480px) {
  #footer {
      display: block;
  }
} */

                                                /* .contactform */

.contactform{
  padding: 0 34px;
  padding-top: 144px; 
  font-family:'Fira Sans', sans-serif ;
}

.contactform div{
  width: 16vw;
  border-radius: 5px;
  margin: 6px 0;
  padding: 3px;
}

.mb-3 {
  display: flex;
  flex-direction: column;
  padding: 10px 0;
  width: 26vw;
  border-radius: 5px;
  margin: 6px 0 0 0;
  padding: 3px;
}

div.main{
  margin: 30px;
}
div#emailHelp {
  font-size: 12px;
  color: midnightblue;
  margin: 0 5px;
  padding: 3px 0 0 0;
}

#form-check{
  flex-direction: row;
}

#form-check input{
  width: 24px;
  margin: 3px 0;
}

/* .nav-item{
  transform: translate(-443px, 0px);
  position: absolute;
} */

.tab-titles{
  display: flex;
  margin: 20px 0 40px;
}
.tab-links{
  margin-right: 50px;
  font-size: 18px;
  font-weight: 500;
  cursor: pointer;
  position: relative;
}
.tab-links::after{
  content: '';
  width: 0;
  height: 3px;
  background: #ff004f;
  position: absolute;
  left: 0;
  bottom: -8px;
  transition: 0.5s;
}
.tab-links.active-link::after{
  width: 50%;
}
div.tab-contents ul li{
  list-style: disc;
  margin: 10px 0;
}
div.tab-contents ul li span{
  color:#080210;
  font-size: 14px;
}
.tab-contents{
  display: none;
}
.tab-contents.active-tab{
  display: block;
}


@media only screen and (max-width: 600px) {
  #header {
      display: block;
  }

  .head-h2,
  .head-h1,
  .head-h3 {
      line-height: 60px;
      font-size: 40px;
  }
  i.fas{
    display: block;
    font-size: 25px;
  }
  nav ul{
    background: #ff004f;
    position: fixed;
    top: 0;
    right: -200px; 
    width: 200px;
    height: 100vh;
    padding-top: 50px;
    z-index: 2;
  }
  nav ul li{
    display: block;
    margin: 25px;
  }
  nav ul i.fas{
    position: absolute;
    top: 25px;
    left: 25px;
    cursor: pointer;
  }
  .tab-links{
    font-size: 16px;
    margin-right: 20px;
  }
  #footer {
    display: block;
}

#about {
  display: block;
}

#form{
  display: block;
}
}
#msg{
  color: #61b752;
  margin-top: 16px;
  display: block;
}






