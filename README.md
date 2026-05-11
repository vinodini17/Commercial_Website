# Ex02 Commercial Website
## Date: 11.05.2026

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
### page.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GlowCare - Skincare Products</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Header -->
    <header>
        <h1>GlowCare</h1>
        <nav>
            <a href="#home">Home</a>
            <a href="#products">Products</a>
            <a href="#about">About Us</a>
            <a href="#contact">Contact Details</a>
            <a href="#account">User Account</a>
        </nav>
    </header>

    <!-- Home / Hero Section -->
    <section id="home" class="hero">
        <div class="hero-text">
            <h2>Healthy Skin Starts Here</h2>
            <p>GlowCare brings you premium, dermatologist-tested skincare products that nourish, protect, and revitalize your skin naturally.</p>
            <a href="#products" class="btn">Shop Now</a>
        </div>
    </section>

    <!-- Products Section -->
    <section id="products" class="products">
        <h2>Our Products & Services</h2>
        <div class="product-card">
            <img src="imag1.png" alt="Gentle Cleanser">
            <h3>Gentle Face Cleanser</h3>
            <p>A mild, sulfate-free formula that removes dirt without stripping natural oils.</p>
            <span class="price">₹323.00</span>
        </div>

        <div class="product-card">
            <img src="image2.png" alt="Hydrating Moisturizer">
            <h3>Hydrating Moisturizer</h3>
            <p>Locks in moisture for 24 hours, leaving skin soft and glowing.</p>
            <span class="price">₹299.00</span>
        </div>

        <div class="product-card">
            <img src="image3.png" alt="Vitamin C Serum">
            <h3>Vitamin C Brightening Serum</h3>
            <p>Boosts radiance, reduces dark spots, and improves skin texture.</p>
            <span class="price">₹449.00</span>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="about">
        <h2>About GlowCare</h2>
        <p>At GlowCare, we believe skincare should be simple, effective, and gentle. 
           Our products are made with natural extracts, free from harmful chemicals, and suitable for all skin types.</p>

        <div class="about-content">
            <div>
                <h3>Our Promise</h3>
                <p>We are committed to providing cruelty-free, eco-friendly skincare that delivers visible results without compromising your health or the planet.</p>
            </div>
            <div>
                <h3>Why Choose Us?</h3>
                <ul>
                    <li>✔ Dermatologist Approved</li>
                    <li>✔ 100% Cruelty-Free</li>
                    <li>✔ Natural Ingredients</li>
                    <li>✔ Safe for All Skin Types</li>
                </ul>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact">
        <h2>Contact Details</h2>
        <p>Email: vinodini@glowcare.com</p>
        <p>Phone: +91 98654 32100</p>
        <p>Address: 123 Glow Street, Chennai, India</p>
    </section>

    <!-- User Account Section -->
    <section id="account" class="account">
        <h2>User Account</h2>
        <form>
            <label for="email">Email:</label><br>
            <input type="email" id="email" name="email" required><br><br>
            
            <label for="password">Password:</label><br>
            <input type="password" id="password" name="password" required><br><br>
            
            <button type="submit" class="btn">Login</button>
            <p>New user? <a href="#">Create an account</a></p>
        </form>
    </section>

    <!-- Footer -->
    <footer>
        <div class="social-links">
            <a href="https://facebook.com/glowcare" target="_blank">Facebook</a> |
            <a href="https://instagram.com/glowcare" target="_blank">Instagram</a> |
            <a href="https://twitter.com/glowcare" target="_blank">Twitter</a>
        </div>
        <p>&copy; 2026 GlowCare. All rights reserved.</p>
    </footer>

</body>
</html>
```
### style.css
```
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background: #fdfdfd;
    color: #333;
}

/* Header */
header {
    background: #ff8fa3;
    color: white;
    padding: 15px 20px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

header h1 {
    margin: 0;
}

nav a {
    color: white;
    text-decoration: none;
    margin-left: 20px;
    font-weight: bold;
}

nav a:hover {
    text-decoration: underline;
}

/* Hero Section */
.hero {
    background-color: #fff5f7;
    text-align: center;
    padding: 120px 20px;
    display: flex;
    align-items: center;
    justify-content: center;
}

.hero-text {
    max-width: 600px;
    background: rgba(255, 143, 163, 0.3);
    padding: 20px;
    border-radius: 10px;
}

.hero-text h2 {
    font-size: 2.5rem;
    margin-bottom: 15px;
}

.hero-text p {
    font-size: 1.1rem;
}

.hero h2 {
    font-size: 40px;
}

/* Buttons */
.btn {
    display: inline-block;
    margin-top: 15px;
    padding: 10px 20px;
    background: white;
    color: #ff5f7e;
    text-decoration: none;
    font-weight: bold;
    border-radius: 5px;
    transition: background 0.3s;
}

.btn:hover {
    background: #ffe3e9;
}

/* Products Section */
.products {
    padding: 40px 20px;
    text-align: center;
}

.product-card {
    background: white;
    display: inline-block;
    width: 250px;
    margin: 15px;
    padding: 15px;
    border-radius: 10px;
    box-shadow: 0px 4px 10px rgba(0,0,0,0.1);
}

.product-card img {
    width: 100%;
    border-radius: 10px;
}

.price {
    display: block;
    margin-top: 10px;
    color: #ff5f7e;
    font-weight: bold;
}

/* About Section */
.about {
    padding: 50px 20px;
    background: #fff5f7;
}

.about-content {
    display: flex;
    gap: 30px;
    flex-wrap: wrap;
    margin-top: 20px;
}

.about-content div {
    flex: 1;
    background: white;
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0px 4px 10px rgba(0,0,0,0.1);
}

.about-content h3 {
    color: #ff5f7e;
}

.about-content ul {
    list-style: none;
    padding: 0;
}

.about-content li {
    padding: 5px 0;
}

/* Contact Section */
.contact {
    padding: 40px 20px;
    background: #fff5f7;
    text-align: center;
}

/* User Account Section */
.account {
    padding: 40px 20px;
    background: #ffffff;
    text-align: center;
}

.account form {
    background: #fff5f7;
    padding: 20px;
    border-radius: 10px;
    max-width: 350px;
    margin: 0 auto;
    box-shadow: 0px 4px 10px rgba(0,0,0,0.1);
}

.account input {
    width: 90%;
    padding: 10px;
    margin-top: 5px;
    border: 1px solid #ff8fa3;
    border-radius: 5px;
    outline: none;
}

.account button {
    margin-top: 15px;
    padding: 10px 20px;
    background: #ff8fa3;
    color: white;
    border: none;
    border-radius: 5px;
    font-weight: bold;
    cursor: pointer;
}

.account button:hover {
    background: #ff5f7e;
}

/* Footer */
footer {
    background: #ff8fa3;
    color: white;
    text-align: center;
    padding: 15px;
}

.social-links {
    margin-bottom: 10px;
}

.social-links a {
    color: white;
    margin: 0 8px;
    text-decoration: none;
    font-weight: bold;
}

.social-links a:hover {
    text-decoration: underline;
}
```

## OUTPUT
<img width="1919" height="719" alt="image" src="https://github.com/user-attachments/assets/98b99af0-799a-443d-8de5-8af73e695140" />

<img width="1911" height="846" alt="image" src="https://github.com/user-attachments/assets/73a28c91-c511-4858-8d53-527ba15894e3" />

<img width="1919" height="879" alt="image" src="https://github.com/user-attachments/assets/62dca9c4-5664-451b-a8a8-4b86140ab181" />

<img width="1919" height="1137" alt="image" src="https://github.com/user-attachments/assets/32ec3afe-1071-44b1-8107-03f1b74ec398" />

# RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.




