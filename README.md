# Ex01 Portfolio
## Date: 20-08-2025

## AIM
To create a Portfolio using HTML and CSS.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for introduction, about, projects, and contact details.

### STEP 5
Define global styles for fonts, colors, and layout.

### STEP 6
Style the header, navigation bar, and sections.

### STEP 7
Use Flexbox or CSS Grid for layout design.

### STEP 8
Add hover effects and transitions for interactivity.

### STEP 9
Add Images and Media.

### STEP 10
Use optimized images for a professional look.

### STEP 11
Open the HTML file in a browser to check layout and functionality.

### STEP 12
Fix styling issues and refine content placement.

### STEP 13
Deploy the Portfolio.

### STEP 14
Upload to GitHub Pages for free hosting.

## PROGRAM
### HTML
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <nav>
            <div class="logo">Portf<span>lio</span></div>
            <br>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About Me</a></li>
                <li><a href="#skills">Experience</a></li>
                <li><a href="#contact">Contact Me</a></li>
            </ul>
        </nav>
    </header>

    <section class="hero" id="home">
        <div class="hero-content">
            <h1>Hello, my name is <span class="highlight">Jespiah <span>Shihana!</span></span></h1>
            <p>I'm a Web Developer :)</p>
            <form action="index.html#">
                <input type="email" placeholder="Enter your email">
                <button type="submit">Submit</button>
            </form>
            <!--<a href="mailto:jespiahshihana@gmail.com?subject=Interested to hire you!" target="_blank"><button class="btn">Hire me!</button></a>-->

        </div>


        <div class="hero-image">
            <img src="Gifty.jpg" alt="Profile Picture">
        </div>
    </section>
    <section class="about" id="about">
        <div class="about-image">
            <img src="gifty 1.jpg" alt="Profile Picture">
        </div>
        <div class="about-content">
            <h2>About Me</h2>
            <h3>Developer <span>& Designer</span></h3>
            <p>
                I am a front-end web developer. I can provide clean code and pixel-perfect design. I also make the website more interactive with web animations. I can provide clean code and pixel-perfect design. I also make the website more &amp; more interactive with web animations. A responsive design makes your website accessible to all users, regardless of their device.
            </p>
        </div>
    </section>

    <section class="experience" id="skills">
        <h2>Experience</h2>
        <div class="timeline">
            <div class="timeline-item">
                <span class="year">2024</span>
                <!--<span class="dot"></span>-->
                <div class="details">
                    <h3>Web Developer Intern</h3>
                    <p class="company">Linlax Infotech</p>
                    <p>LINLAX Private Limited is an ITES [Information Technology Enabled Service] Company and incorporated under The Companies Act 1956, in the year 2012 with the objective of developing Software products , E commerce Stores , Portals for Education and undertaking information related activities. We are planned to incorporate our Companies in USA in 2016.</p>
                </div>
            </div>
            <div class="timeline-item">
                <span class="year">2024</span>
                <!--<span class="dot"></span>-->
                <div class="details">
                    <h3>Flipkart Event</h3>
                    <p class="company">Flipkart</p>
                    <p>Participating in the Flipkart Grid event allowed me to apply my skills in coding and problem-solving to real-world challenges, enhancing my understanding of AI and e-commerce. The experience also provided me with valuable teamwork and collaboration opportunities, reinforcing my passion for technology and innovation.</p>
                </div>
            </div>
        </div>
    </section>
    <section id="contact">
    <div style="text-align: center; padding: 20px; background-color: black; color: white;">
        <p style="font-size: 20px;">Contact Me</p>
        <p><strong>Email:</strong> jespiahshihana@gmail.com</p>
        <p><strong>Phone:</strong> 6383349837</p>
        <p><strong>Location:</strong> Thandalam,Chennai</p>
    </div>
    </section>
</body>
</html>
```
### CSS
```
/* home section */
body {
    font-family: 'Arial', sans-serif;
    margin: 0;
    padding: 0;
    background-color: #000;
    color: #fff;
}

header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 50px;
}

.logo {
    font-size: 24px;
    font-weight: bold;
}

.logo span {
    color: #c60f80;
}

.nav-links {
    display: flex;
    list-style: none;
    font-size:20px;
}

.nav-links li {
    margin: 0 15px;
}

.nav-links a {
    text-decoration: none;
    color: #fff;
}

.hero {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 100px 50px;
}

.hero-content {
    max-width: 50%;
}

.hero-content h1 {
    font-size: 52px;
    margin: 0;
    padding-bottom:50px;
}

.hero-content h1 .highlight span {
    color: #c60f80;
}

.hero-content p {
    font-size: 24px;
    margin: 20px 0;
    padding-bottom:20px;
}

.hero-content form {
    display: flex;
    padding-bottom:50px;
}

.hero-content input {
    padding: 10px;
    border: none;
    border-radius: 25px 0 0 25px;
    width: 300px;
}

.hero-content button {
    background-color: #c60f80;
    color: #fff;
    border: none;
    padding: 10px 20px;
    border-radius: 0 25px 25px 0;
    cursor: pointer;
}
.hero-content .btn{
    margin-top: 10px;
    margin-left: 160px;
    
}
.hero-image img {
    border-radius: 50%;
    max-width: 400px;
    height:400px;
    width:500px;
    margin-right:150px;
}

/* about section */
.about {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 100px 50px;
    background-color: #000;
    color: #fff;
}

.about-image {
    max-width: 45%;
}

.about-image img {
    border-radius: 10px;
    max-width: 100%;
    height:500px;
    width:500px;
}

.about-content {
    max-width: 50%;
}

.about-content h2 {
    font-size: 48px;
    margin-bottom: 20px;
}

.about-content h3 {
    font-size: 24px;
    color: #c60f80;
    margin-bottom: 20px;
}

.about-content h3 span {
    color: #fff;
}

.about-content p {
    font-size: 18px;
    line-height: 1.6;
    margin-bottom: 30px;
}

/* experience section */
.experience {
    padding: 80px 50px;
    background-color: #1c1c1c;
    color: #eaeaea;
}

.experience h2 {
    font-size: 48px;
    margin-bottom: 50px;
    color: #fff;
}

.timeline {
    position: relative;
    margin-left: 30px;
}

.timeline-item {
    position: relative;
    margin-bottom: 50px;
}

.timeline-item .year {
    position: absolute;
    left: -100px;
    top: 0;
    font-size: 24px;
    color: #eaeaea;
    margin-left:50px;
}

.timeline-item .dot {
    position: absolute;
    left: -35px;
    top: 8px;
    height: 12px;
    width: 12px;
    background-color: #10b8e7;
    border-radius: 50%;
    margin-left:50px;
}

.timeline-item .details {
    padding-left: 80px;
}

.timeline-item h3 {
    font-size: 28px;
    margin-bottom: 5px;
    color: #fff;
}

.timeline-item .company {
    font-style: italic;
    margin-bottom: 10px;
    color: #c9c9c9;
}

.timeline-item p {
    font-size: 16px;
    line-height: 1.6;
    color: #c9c9c9;
}
```

## OUTPUT
<img width="1903" height="869" alt="image" src="https://github.com/user-attachments/assets/fbaac27a-465e-4040-b46d-599db9cae704" />
<img width="1918" height="866" alt="image" src="https://github.com/user-attachments/assets/c43f2d31-ed51-4f5c-b120-623c821c0a1f" />
<img width="1895" height="852" alt="image" src="https://github.com/user-attachments/assets/e7451756-b829-4b2a-9079-3309f38ba69c" />


## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
