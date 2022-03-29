<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.0/css/all.min.css">
    <link rel="stylesheet" href="https://unicons.iconscout.com/release/v4.0.0/css/line.css">
    <link rel="stylesheet" href="swiper-bundle.min.css">
    <link rel="stylesheet" href="https://unpkg.com/swiper/swiper-bundle.min.css"/>
    <style>
      *{
    font-family: "Poppins", sans-serif;
    padding: 0;
    margin: 0;
    box-sizing: border-box;
    list-style: none;
    text-decoration: none;
    scroll-behavior: smooth;
}
:root{
    --bg-color: #ffffff;
    --primary: #01a29c;
    --hover: #008170;
    --h1-font: 2.4rem;
    --h2-font: 1.8rem;
    --p-font: 1.2rem;
    --spacing: 1px;
    --m-1: 0.4rem;
    --m-4: 2rem;
}
body::-webkit-scrollbar{
    width: 0.25rem;
}
body::-webkit-scrollbar-track{
    background: #2c3e50;
}
body::-webkit-scrollbar-thumb{
    background: var(--primary);
}
html{
    background: #1c2834;
    color: #fff;
}
section{
    /* padding: 50px 200px; */
    padding: 0 9%;
    width: 100%;
}
header{
    position: fixed;
    width: 100%;
    top: 0;
    right: 0;
    z-index: 1000;
    display: flex;
    align-items: center;
    justify-content: flex-end;
    background: var(--bg-color);
    padding: 18px 200px;
    box-shadow: 0 0.5rem 50rem rgba(0, 0, 0, 0.1);
}
.logo{
    text-transform: uppercase;
    font-size: 1.4rem;
    font-weight: 600;
    color: var(--primary);
}
.navbar{
    display: flex;
}
.navbar a{
    font-size: 1rem;
    padding: 10px 20px;
    color: #222435;
    font-weight: 500;
}
header .navbar a:hover{
    background: var(--primary);
    color: #fff;
}
#menu-icon{
    font-size: 2rem;
    cursor: pointer;
    display: none;
}
.home{
    position: relative;
    width: 100%;
    min-height: 100vh;
    color: #222435;
    display: flex;
    align-items: center;
    background-color: var(--bg-color);
    /* background: url(https://images.pexels.com/photos/3778133/pexels-photo-3778133.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940) no-repeat;  */
    background: url(https://images.pexels.com/photos/218863/pexels-photo-218863.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=1280&w=853) no-repeat;
    background-size: cover;
    background-position: right center;
}
.home-text{
    max-width: 500px;
}
.home-text h1{
    font-size: var(--h1-font);
    letter-spacing: var(--spacing);
    color: #e7eafb;
}
.home-text span{
    color: var(--primary);
}
.home-text h2{
    font-size: var(--h2-font);
    margin: var(--m-1) 0;
    letter-spacing: var(--spacing);
    color: #e7eafb;
}
.home-text p{
    font-size: var(--p-font);
    margin-bottom: var(--m-4);
    line-height: 22px;
    max-width: 71%;
    color: #e7eafb;
}
.btn{
    padding: 10px 22px;
    background: var(--primary);
    color: #fff;
}
.btn:hover{
    background: var(--hover);
}
.about{
    width: 100%;
    min-height: 84vh;
    display: flex;
    align-items: center;
    justify-content: space-between;
}
.about-img{
    width: 500px;
    height: 400px;
}
.about-img img{
    width: 100%;
    height: 100%;
    object-fit: contain;
    object-position: center;
}
.about-text{
  max-width: 50%;  
}
.about-text h2{
    font-size: var(--h2-font);
    color: var(--primary); 
}
.about-text h1{
    font-size: var(--h1-font);
    font-weight: 600;
}
.about-text p{
    font-size: var(--p-font);
    margin: 1rem 0 var(--m-4);
    text-align: justify;
    font-weight: 300;
}
.skills{
    width: 100%;
    min-height: 84vh;
}
.skills-content{
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 100%;
}
.skills-img{
    width: 500px;
    height: 400px;
    /* margin-top: 7.6rem; */
}
.skills-img img{
    height: 100%;
    width: 100%;
    object-fit: cover;
    object-position: center;
}
.skills-bars{
    display: flex;
    flex-direction: column;
    width: 50%;
}
/* .skills-text h2 {
    font-weight: 600;
}
.skills-text p{
    font-size: var(--p-font);
    margin: 1rem 0
} */
.skills-box{
    position: relative;
    background: #2c3e50;
    margin: 1rem 0;
    height: 3.4rem;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 0 10px;
    border-radius: 10px;

}
.skills-box i{
    display: flex;
    align-items: center;
    font-size: 20px;
    font-weight: 600;
    color: #01a29c;
}
.skills-box h3{
    margin-left: 1rem;
    font-size: 1rem;
    font-weight: 600;
    font-style: normal;
}
.percent-bar{
    position: absolute;
    left: 0;
    bottom: 0;
    background: var(--primary);
    height: 0.34rem;
    border-radius: 10px;
}

.heading{
    display: flex;
    justify-content: center;
    padding: 1.4rem 0;
}
.heading h1{
    font-size: var(--h1-font);
    font-weight: 600;
    border-bottom: 2px solid var(--primary);
}
.html-bar{
   width: 94%; 
   transition: all 1.5s;
}
.css-bar{
   width: 84%;
   transition: all 1.5s; 
   animation: text 0.6s ease-in-out;
}
.js-bar{
    width: 65%; 
    transition: all 1.5s;
}
.react-bar{
    width: 60%; 
    transition: all 1.5s;
}
.angular-bar{
    width: 40%;
    transition: all 2.5s; 
}
.portfolio-content{
    display: flex;
    height: auto;
    align-items: center;
    justify-content: space-between;
}

.p-box{
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 300px;
    height: auto;
    background: #2c3e50;
    margin: 20px 0 20px 0;
    padding: 40px;
    text-align: center;
}
.p-box:hover{
    background: var(--primary);
    transition: 0.5s ease;
}
.p-box a{
    margin-top: 1.5rem;
}
.p-img{
    width: 70px;
    height: 70px;
}
.p-img img{
    width: 100%;
    height: 100%;
    border-radius: 50%;
    border: 4px solid --primary;
}
.p-box h2 {
    font-size: var(--h2-font);
    font-weight: 600;
    margin: 10px 0;
}
.p-box p{
    font-size: var(--p-font);
    font-weight: 400;
}



.contact-content{
    display: flex;
    align-items: center;
    justify-content: space-around;
}
.contact-button{
    display: flex;
    align-items: center;
    justify-content: space-around;
}
.contact-info{
    max-width: 500px;
}
.info-box{
    display: flex;
    align-items: center;
    margin: 1rem 0;
}
.info-box i{
    font-size: 20px;
    color: var(--primary);
}
.info-box p{
    margin-left: 1rem;
    font-weight: 400;
}
.social{
    display: flex;
    align-items: center;
}
.social a{
    margin-right: 1rem;
}
form{
    max-width: 360px;
    margin-top: 4rem;
}
form input, 
form textarea{
    width: 100%;
    font-size: 14px;
    padding: 1rem;
    border-radius: 0.5rem;
    border: none;
    outline: none;
    margin-bottom: 12px;
    background: #2c3e50;
    color: var(--primary);
    border-bottom: 1px solid var(--primary);
}
form textarea{
    height: 200px;
    resize: none;
}
.contact-button{
    max-width: 100px;
    font: 600;
    background: var(--primary);
    color: #fff;
    text-transform: uppercase;
    letter-spacing: 1px;
    cursor: pointer;
}
@media (max-width: 991px){
    header{
        padding: 15px 80px;
    }
    section{
        padding: 50px 80px;
    }
    .about-text{
        max-width: 444px;
    }
    .about-img{
        width: 300px;
        height: 300px;
    }
    .skills-bars{
        max-width: 420px;
    }
    .skills-img{
        width: 400px;
        height: 300px;
        margin-top: 6rem;
    }
/* .skills-box{
    flex: 1;
    } */
}
@media (max-width: 820px){
    :root{
        --h1-font: 2rem;
        --h2-font: 1rem;
        --m4-4: 1.4rem;
    }
    header{
        padding: 13px 65px;
    }
    section{
        padding: 50px 65px;
    }
    .about{
        flex-direction: column;
    }
    .about-img{
        width: 240px;
        height: 300px;
    }
    .p-box{
        flex: 1;
    }
    .skills-content{
        flex-direction: column;
    }
}
@media (max-width: 768px){
    #menu-icon{
        display: initial;
        color: #222435;
    }
    header .navbar{
        position: absolute;
        top: 100%;
        left: 0;
        right: 0;
        display: flex;
        flex-direction: column;
        text-align: center;
        background: var(--bg-color);
        clip-path: polygon(0 0, 100% 0, 100% 0, 0 0);
        transition: 0.5s ease;
    }
    header .navbar.active{
        clip-path: polygon(0 0, 100% 0, 100% 100%, 0 100%);
    }
    .navbar a {
        margin: 1rem;
        padding: 1.5rem;
        display: block;
        background: #fff;
        border-left: 4px solid #222435;
    }
    .home{
        background: #2c3e50;
        justify-content: center;
    }
    .home-text{
        max-width: 410px;
    }
    .contact-content{
        flex-direction: column;
    }
}
@media (max-width: 670px) {
    header{
        padding: 10px 34px;
    }
    section{
        padding: 50px 34px;
    }
    .skills-img{
        width: 320px;
    }
}
    </style>
</head>
<body>
    <header>
        <div id="menu-icon" class="fas fa-bars"></div>

        <ul class="navbar">
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#skills">Skills</a></li>
            <li><a href="#portfolio">Portfolio</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </header>

    <section class="home" id="home">
            <div class="home-text">
                <h1>Helo, I'm <br><span>Aleh Buhayevich</span></h1>
                <h2>FrontEnd-Developer</h2>
                <p></p>
                <a href="https://t.me/olegbugaevich" class="btn">CONTACT ME</a>
            </div>
    </section>
    <section class="about" id="about">
        <div class="about-img">
            <img src="IMG_0536.jpg" alt="logo">
        </div>
        <div class="about-text">
            <h2>About me</h2>
            <p>My name is Aleh, I would like to apply for the role of 
                Junior Frontend Developer that is currently looking for 
                in the Internet.</p>
            <p>As you can see from my attached CV, 
                I have over 9 years experience in the oil Industry, 
                but one years ago I understood that I need to change direction 
                job and start to work in IT-sphere. </p>
            <p> During this period I finished one-years Frontend-Developer course 
                in It-Step School.
                In the process of training I was receive the following skills: HTML, CSS, (Grid, Flex, Bootstrap), JavaScript, 
                React, Material-UI, Git, GitHub</p>
            <a href="CV_BUHAYEVICH ALEH.pdf" class="btn">Download CV</a>
        </div>
    </section>
    <section class="skills" id="skills">
        <div class="heading">
            <h1>SKILLS</h1>
        </div>
        <div class="skills-content">
            <div class="skills-bars">
                <div class="skills-box">
                    <i class="fab fa-html5"><h3>HTML</h3></i>
                    <span>94%</span>
                    <div class="percent-bar html-bar" data-progress="94"></div>
                </div>
                <div class="skills-box">
                    <i class="fab fa-css3"><h3>CSS</h3></i>
                    <span>84%</span>
                    <div class="percent-bar css-bar" data-progress="84"></div>
                </div>
                <div class="skills-box">
                    <i class="fab fa-js"><h3>JavaScript</h3></i>
                    <span>65%</span>
                    <div class="percent-bar js-bar" data-progress="65"></div>
                </div>
                <div class="skills-box">
                    <i class="uil uil-react"><h3>REACT</h3></i>
                    <span>60%</span>
                    <div class="percent-bar react-bar" data-progress="60"></div>
                </div>
                <div class="skills-box">
                    <i class="fab fa-angular"><h3>ANGULAR</h3></i>
                    <span>40%</span>
                    <div class="percent-bar angular-bar" data-progress="40"></div>
                </div>
            </div>
            <div class="skills-img">
                <img src="https://images.pexels.com/photos/1181271/pexels-photo-1181271.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940" alt="Мои навыки">
            </div>
        </div>
    </section>


    <section class="portfolio" id="portfolio">
        <div class="heading">
            <h1>PORTFOLIO</h1>
        </div>

        <div class="portfolio-content">
            <div class="p-box">
                <div class="p-img">
                    <img src="#" alt="">
                </div>
                <h2>Прогноз погоды</h2>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Suscipit fugiat odio provident pariatur fugit. Necessitatibus id minus eveniet nulla, assumenda corrupti, possimus harum reprehenderit officia itaque placeat enim in rem?</p>
                <a href="#" class="btn">DEMO</a>
            </div>
            <div class="p-box">
                <div class="p-img">
                    <img src="#" alt="">
                </div>
                <h2>Поисковик фильмов</h2>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Suscipit fugiat odio provident pariatur fugit. Necessitatibus id minus eveniet nulla, assumenda corrupti, possimus harum reprehenderit officia itaque placeat enim in rem?</p>
                <a href="#" class="btn">DEMO</a>
            </div>
            <div class="p-box">
                <div class="p-img">
                    <img src="" alt="">
                </div>
                <h2>Салон красоты</h2>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Suscipit fugiat odio provident pariatur fugit. Necessitatibus id minus eveniet nulla, assumenda corrupti, possimus harum reprehenderit officia itaque placeat enim in rem?</p>
                <a href="#" class="btn">DEMO</a>
            </div>
        </div>
    </section>

    

    <section class="contact" id="contact">
        <div class="heading">
            <h1>CONTACTS</h1>
        </div>
        <div class="contact-content">
            <div class="contact-info">
                <div class="info-box">
                    <i class="fas fa-phone-alt"></i>                        
                    <p>+375 29 599-97-20</p>
                </div>
                <div class="info-box">
                    <i class="fas fa-envelope-open"></i>
                    <p>olegbugaevich@gmail.com</p>
                </div>
                <div class="info-box">
                    <i class="fas fa-map-marker-alt"></i>
                    <p>Minsk, Belarus</p>
                </div>
                <div class="info-box social">
                    <a href="https://www.github.com/"><i class="fab fa-github"></i></a>
                    <a href="https://www.facebook.com/olegbugaevich"><i class="fab fa-facebook"></i></a>
                    <a href="https://www.linkedin.com/in/oleg-bugaevich-0a2b991a4?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base_contact_details%3BeXr8RPzqS328uNgu2TmFCA%3D%3D/"><i class="fab fa-linkedin-in"></i></a>
                    <a href="https://t.me/olegbugaevich"><i class="fab fa-telegram"></i></a>
                    
                </div>
            </div>
            <div class="contact-form">
                <form action="" onsubmit="sendEmail(); reset(); return false;">
                    <input type="text" placeholder="Your Name" required>
                    <input type="email" placeholder="Enter Your Email" required>
                    <textarea name="" id="" cols="30" rows="10" placeholder="Write your message here..."></textarea>
                    <input type="submit" value="Send" class="contact-button">
                </form>
            </div>
        </div>
    </section>
</body>
</html>
