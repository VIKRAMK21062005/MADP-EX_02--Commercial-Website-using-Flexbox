# Ex02 Commercial Website
## Date:
### Reg no : 212222040180
### Name : Vikram K
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
### index.html

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dairy Milk E-Commerce</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">

</head>
<body>
    <header>
        <nav>
            <div class="logo">Dairy Milk</div>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#products">Product_Details</a></li>
                <li><a href="#buy">Buy Product</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>
    
    <section id="home" class="banner">
        <div class="home-container">
            <div class="home-left">
                <video autoplay muted loop>
                    <source src="images/videoplayback.mp4" type="video/mp4">
                    Your browser does not support the video tag.
                </video>
            </div>
            <div class="home-right">
                <h1>Welcome to Dairy Milk World</h1>
                <p>Dairy Milk is 100% healthy. How? Simple. Cocoa comes from a tree 🌳, 
                trees are plants, and plants are vegetables. That means Dairy Milk is basically a salad! 🥗😂 So, 
                technically, I’m making healthy choices… one delicious bite at a time. 😆🍫</p>
                <a href="#" class="btn">Explore More</a>
            </div>
        </div>
    </section>
    
    <section id="about">
        <div class="a-total">
            <div class="a-title">
                <h2>About Me</h2>
            </div>
           
            <div class="a-container">
                
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Totam delectus, 
                    sunt cum iste beatae explicabo laudantium accusantium voluptatibus quasi repellendus.</p>
                <button><a href="#">About me...</a></button>    
            </div>
            <div class="a-right">
                <img src="images/bike dp.jpg" alt="" id="imgs">
                <div class="social-icons">
                    <a href="#" target="_blank"><i class="fa-brands fa-github"></i></a>
                    <a href="#" target="_blank"><i class="fa-brands fa-linkedin"></i></a>
                    <a href="#" target="_blank"><i class="fa-brands fa-twitter"></i></a>
                </div>
            </div>
        </div>
    </section>
    
    
    
    
    
    <section id="products" class="products">
        <h2>Our Products</h2>
        <div class="product-container">
            <div class="product">
                <img src="images/p1.png" alt="Dairy Milk Classic">
                <h3>Dairy Milk Classic</h3>
                <p>Rich and creamy chocolate bar</p>
            </div>
            <div class="product">
                <img src="images/p2.png" alt="Dairy Milk Silk">
                <h3>Dairy Milk Silk</h3>
                <p>Smooth and premium chocolate</p>
            </div>
            <div class="product">
                <img src="images/p4.png" alt="Dairy Milk Silk">
                <h3>Dairy Milk Silk</h3>
                <p>Smooth and premium chocolate</p>
            </div>
        </div>
    </section>
    
    <section id="buy" class="buy">
        <h2>Buy Now</h2>
        <p>Order your favorite Dairy Milk chocolates now and enjoy the sweetness.</p>
        <button onclick="showForm()">Shop Now</button>

        <div id="orderForm">
            <h3>Order Form</h3>
            <form>
                <input type="text" placeholder="Your Name" required>
                <input type="email" placeholder="Your Email" required>
                <input type="number" placeholder="Quantity" required>
                <div class="form-buttons">
                    <button type="submit">Place Order</button>
                    <button type="button" onclick="hideForm()">Close</button>
                </div>
            </form>
        </div>
    </section>
    
    
    <section id="contact" class="contact">
        <h2>Contact Us</h2>
        <div class="social-icons">
            <a href="#"><i class="fa-brands fa-facebook"></i></a>
            <a href="#"><i class="fa-brands fa-twitter"></i></a>
            <a href="#"><i class="fa-brands fa-instagram"></i></a>
            <a href="#"><i class="fa-brands fa-linkedin"></i></a>
            <a href="#"><i class="fa-solid fa-map-marker-alt"></i></a>
            <a href="#"><i class="fa-solid fa-phone"></i></a>
            <a href="#"><i class="fa-solid fa-envelope"></i></a>

        </div>
    </section>
    
    
    
    <footer>
        <p>&copy; 2025 Dairy Milk. All Rights Reserved.</p>
    </footer>
    <script src="script.js">
        
    </script>
    <script src="https://kit.fontawesome.com/your-fontawesome-kit.js" crossorigin="anonymous"></script>

</body>
</html>
```
### style.css
```

:root{
    --font1: 'Courier New', Courier, monospace;
}
*{
    text-decoration: none;
    position: relative;
}
body {
    font-family: 'Poppins', sans-serif;
    margin: 0;
    padding: 0;
    background: url('images/back_g.png') no-repeat center center fixed;
    background-size: cover;
    color: #fff;
    scroll-behavior: smooth;
    text-decoration: none;
}


header {
    background-color: #1d031e;
    padding: 15px 0;
}

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 80%;
    margin: auto;
}

.logo {
    font-family: var(--font1);
    font-size: 24px;
    font-weight: bold;
    color: #fbe7c6;
    display:flex;
    padding: 5px 10px;
    transition: box-shadow 0.3s ease-in-out;
}

.logo:hover {
    box-shadow: 0px 0px 10px blanchedalmond;
}



nav ul {
    list-style: none;
    display: flex;
    gap: 20px;
}

nav ul li a {
    text-decoration: none;
    color: #fbe7c6;
    font-size: 18px;
    padding-left: 0;
    right: 0;
    margin-right: 0;
}

nav ul li a:hover {
    color: #ffd700;
    text-shadow: 0px 0px 10px blanchedalmond;
    /* border: 1px dotted white;
    padding: auto; */
    
}

.banner {
    display: flex;
    align-items: center;
    justify-content: center; 
    padding: 50px 0%;
    background: url('images/back_g.png') no-repeat center center;
    background-size: cover;
    width: 100%;
    min-height: 100vh;
    color: white;
    text-align: left;
}

/* Home */
.home-container {
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 100%;
    max-width: 1200px;
    margin-bottom: 10%;
}

.home-left video {
    width: 100%;
    max-width: 550px;
    border-radius: 10px;
    box-shadow: 0px 5px 15px rgba(0, 0, 0, 0.2);
}

.home-right {
    max-width: 600px;
    
}

.home-right h1 {
    font-size: 2.5rem;
    margin-bottom: 10px;
}

.home-right p {
    font-size: 1.2rem;
    line-height: 1.6;
    margin-bottom: 15px;
}

.btn {
    display: inline-block;
    padding: 10px 20px;
    background: #5d3fd3;
    color: white;
    font-weight: bold;
    border-radius: 5px;
    transition: 0.3s ease-in-out;
}

.btn:hover {
    background: #876fd5;
}

#home {
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100vh;
}


/* About */

#a-total {
    display: flex;
    flex-direction: column; 
    align-items: center;
    justify-content: center;
    padding: 50px;
    color: white;
}

.a-title {
    width: 100%;
    text-align: center;
    margin-bottom: 20px;
}

.a-title h2 {
    font-size: 30px;
    font-weight: 600;
    color: #fff;
}

.a-total {
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;
    max-width: 1200px;
    margin: auto;
}

.a-container {
    flex: 1;
    text-align: left;
    max-width: 600px;
}

.a-container p {
    font-size: 1.2rem;
    line-height: 1.6;
    margin-bottom: 15px;
}

.a-container button {
    background-color: #ff4500;
    color: white;
    padding: 10px 20px;
    border: none;
    cursor: pointer;
    font-size: 16px;
    border-radius: 5px;
    transition: 0.3s;
}

.a-container button a {
    text-decoration: none;
    color: white;
}

.a-container button:hover {
    background-color: #d33f00;
}

.a-right {
    flex: 1;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.a-right img {
    width: 220px;
    height: 220px;
    border-radius: 10px;
    margin-bottom: 15px;
}

/* Product */
.products {
    text-align: center;
    padding: 50px;
}

.product-container {
    display: flex;
    justify-content: center;
    gap: 20px;
    margin-top: 20px;
}

.product {
    background-color: #fff;
    padding: 20px;
    border-radius: 10px;
    box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.2);
    width: 250px;
    color: #1d031e;
}

.product img {
    max-width: 200px;
    height: 200px;
    border-radius: 10px;

}

.product h3 {
    margin-top: 10px;
}

/* Buy Now */
.buy {
    text-align: center;
    padding: 50px;
    color: white;
}

.buy button {
    background-color: #ffd700;
    border: none;
    padding: 10px 20px;
    font-size: 18px;
    border-radius: 5px;
    cursor: pointer;
}

.buy button:hover {
    background-color: #f5c100;
}

#orderForm {
    display: none;
    margin: 30px auto 0;
    max-width: 400px;
    background-color: white;
    padding: 20px;
    border-radius: 5px;
    box-shadow: 0 0 10px rgba(0,0,0,0.3);
    color: black;
    text-align: left;
}

#orderForm h3 {
    text-align: center;
}

#orderForm input {
    width: 90%;
    padding: 10px;
    font-size: 16px;
    border-radius: 5px;
    border: 1px solid #ccc;
    margin: 10px 0;
}

#orderForm .form-buttons {
    text-align: center;
    margin-top: 15px;
}

#orderForm .form-buttons button {
    padding: 10px 20px;
    font-size: 16px;
    border-radius: 5px;
    border: none;
    margin: 0 5px;
    cursor: pointer;
}

#orderForm .form-buttons button[type="submit"] {
    background-color: #ffd700;
}

#orderForm .form-buttons button[type="submit"]:hover {
    background-color: #f5c100;
}

#orderForm .form-buttons button[type="button"] {
    background-color: #ccc;
}

#orderForm .form-buttons button[type="button"]:hover {
    background-color: #bbb;
}


/* Contact */
.contact {
    text-align: center;
    padding: 50px;
    color: white;
}

.contact h2 {
    font-size: 32px;
    margin-bottom: 20px;
}

.social-icons {
    display: flex;
    justify-content: center;
    gap: 15px;
}

.social-icons a {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 50px; 
    height: 50px;
    border: 2px solid white; 
    border-radius: 10%; 
    text-decoration: none;
    transition: 0.3s ease-in-out;
}

.social-icons a i {
    font-size: 24px;
    color: white;
    transition: 0.3s ease-in-out;
}

.social-icons a:hover {
    background-color: #ff4500;
    border-color: #ff4500;
}

.social-icons a:hover i {
    color: #fff700;
}



/* Footer */
footer {
    text-align: center;
    background: linear-gradient(135deg, #4B0082, #8B5CF6, #FFD700);
    color: white;
    padding: 20px;
}
```
script.js
```
function showForm() {
   document.getElementById("orderForm").style.display = "block";
}

function hideForm() {
   document.getElementById("orderForm").style.display = "none";
}
```

## OUTPUT

### Homepage:
![Screenshot 2025-04-29 101039](https://github.com/user-attachments/assets/cdc74c4e-b13d-42d5-a2f8-6449e33e9b1a)
### AboutPage:
![image](https://github.com/user-attachments/assets/3215d0c9-27fb-4754-ba63-f79d5a641186)
### Products:
![image](https://github.com/user-attachments/assets/705e416a-98dc-4c30-aa89-2e4d56d62b4c)
### Contact & OrderForm:
![image](https://github.com/user-attachments/assets/5e148c87-5505-4d18-9b4d-999a51e1edbd)
### Footer:
![image](https://github.com/user-attachments/assets/8f6736ae-be68-4aa9-934c-10d7d7faec91)


## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
