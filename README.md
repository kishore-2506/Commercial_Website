# Ex02 Commercial Website
## Date:
## Date: 27.02.26

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM

## HTML
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Innovexa Solutions</title>
    <link rel="stylesheet" href="style.css">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>
<!-- HEADER -->
<header>
    <div class="logo">Innovexa</div>
    <nav>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#products">Products</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#contact">Contact</a></li>
            <li><a href="#account" class="btn">Account</a></li>
        </ul>
    </nav>
</header>
<!-- HERO SECTION -->
<section id="home" class="hero">
    <div class="hero-content">
        <h1>Innovative Digital Solutions</h1>
        <p>We help businesses grow with modern technology and smart design.</p>
        <a href="#products" class="cta-btn">Explore Services</a>
    </div>
</section>
<!-- PRODUCTS / SERVICES -->
<section id="products" class="section">
    <h2>Our Services</h2>
    <div class="card-container">
        <div class="card">
            <img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085" alt="Web Development">
            <h3>Web Development</h3>
            <p>Responsive and modern websites tailored to your business needs.</p>
        </div>
        <div class="card">
            <img src="https://images.unsplash.com/photo-1551434678-e076c223a692" alt="App Development">
            <h3>App Development</h3>
            <p>High-performance mobile and web applications.</p>
        </div>
        <div class="card">
            <img src="https://images.unsplash.com/photo-1532619187608-e5375cab36aa" alt="Digital Marketing">
            <h3>Digital Marketing</h3>
            <p>Boost your brand with data-driven marketing strategies.</p>
        </div>
    </div>
</section>
<!-- ABOUT -->
<section id="about" class="section light">
    <h2>About Us</h2>
    <p>
        Innovexa Solutions is a technology-driven company delivering high-quality
        digital services. We focus on innovation, reliability, and customer satisfaction.
    </p>
</section>
<!-- CONTACT -->
<section id="contact" class="section">
    <h2>Contact Us</h2>
    <div class="contact-container">
        <div>
            <p>Email: contact@Innovexa.com</p>
            <p>Phone: +91 98765 43210</p>
            <p>Location: Chennai, India</p>
        </div>
        <form>
            <input type="text" placeholder="Your Name" required>
            <input type="email" placeholder="Your Email" required>
            <textarea placeholder="Your Message"></textarea>
            <button type="submit">Send Message</button>
        </form>
    </div>
</section>
<!-- ACCOUNT -->
<section id="account" class="section light">
    <h2>User Account</h2>
    <form class="account-form">
        <input type="text" placeholder="Username">
        <input type="password" placeholder="Password">
        <button type="submit">Login</button>
    </form>
</section>
<!-- FOOTER -->
<footer>
    <div class="social">
        <a href="#">Facebook</a>
        <a href="#">Instagram</a>
        <a href="#">LinkedIn</a>
        <a href="#">Twitter</a>
    </div>
    <p>© 2026 Innovexa Solutions. All Rights Reserved.</p>
</footer>
</body>
</html>
```

## CSS
```
/* GLOBAL STYLES */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    color: #333;
}
.section {
    padding: 60px 10%;
    text-align: center;
}
.light {
    background: #f4f4f4;
}
/* HEADER */
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 10%;
    background: #111;
    color: white;
    position: sticky;
    top: 0;
}
.logo {
    font-size: 24px;
    font-weight: bold;
}
nav ul {
    display: flex;
    list-style: none;
}
nav ul li {
    margin-left: 20px;
}
nav a {
    color: white;
    text-decoration: none;
    transition: 0.3s;
}
nav a:hover {
    color: #00bcd4;
}
.btn {
    background: #00bcd4;
    padding: 6px 12px;
    border-radius: 4px;
}
/* HERO */
.hero {
    background: url("https://images.unsplash.com/photo-1508780709619-79562169bc64") no-repeat center center/cover;
    height: 90vh;
    display: flex;
    align-items: center;
    justify-content: center;
    color: white;
    text-align: center;
}
.cta-btn {
    display: inline-block;
    margin-top: 20px;
    padding: 10px 20px;
    background: #00bcd4;
    color: white;
    text-decoration: none;
    border-radius: 5px;
    transition: 0.3s;
}
.cta-btn:hover {
    background: #0097a7;
}
/* CARDS */
.card-container {
    display: flex;
    gap: 20px;
    margin-top: 40px;
    justify-content: center;
    flex-wrap: wrap;
}
.card {
    background: white;
    width: 300px;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 5px 15px rgba(0,0,0,0.1);
    transition: transform 0.3s ease;
}
.card img {
    width: 100%;
    border-radius: 6px;
}
.card:hover {
    transform: translateY(-10px);
}
/* CONTACT */
.contact-container {
    display: flex;
    gap: 40px;
    justify-content: center;
    margin-top: 30px;
    flex-wrap: wrap;
}
form input, form textarea {
    width: 100%;
    padding: 10px;
    margin: 10px 0;
}
form button {
    padding: 10px 20px;
    background: #00bcd4;
    color: white;
    border: none;
    cursor: pointer;
}
form button:hover {
    background: #0097a7;
}
/* FOOTER */
footer {
    background: #111;
    color: white;
    padding: 20px;
    text-align: center;
}
.social a {
    margin: 0 10px;
    color: #00bcd4;
    text-decoration: none;
}
.social a:hover {
    text-decoration: underline;
}
```
## OUTPUT

<img width="1879" height="916" alt="1" src="https://github.com/user-attachments/assets/cf68a535-1110-4c7e-9d47-dd87197df90c" />

<img width="1886" height="891" alt="2" src="https://github.com/user-attachments/assets/f862146e-e524-40d4-9b9d-763341bd0bd0" />

<img width="1880" height="912" alt="3" src="https://github.com/user-attachments/assets/03f239e2-12c9-4d3f-8956-2fa749b07eff" />

<img width="1879" height="902" alt="4" src="https://github.com/user-attachments/assets/f516e774-2926-4d3d-ac89-9e0f043540f0" />

## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
