# PORTFOLIO
<!DOCTYPE html>
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
