# Ex.07 Restaurant Website
## Date:20/12/2025
## ref no : 25009157
## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
~~~
home.html 

<!DOCTYPE html>
<html>
<head>
    <title>Leafora</title>
    <link rel="stylesheet" href="index.css">
</head>
<body>
<header>
    <h1>Leafora  Veg Restaurant</h1>
</header>

<nav>
    <a href="home.html">Home</a>
    <a href="menu.html">Menu</a>
    <a href="admin.html">Administration</a>
    <a href="contact.html">Contact Us</a>
</nav>

<section>
    <img src="rest.png" alt="Restaurant Banner" style="width:80%; max-width:400px; border-radius:7px;">
    <h2>Welcome to Leafora Veg</h2>
    <p>Fresh vegetarian flavors, modern dining experience, and cozy vibes.</p>
</section>

</body>
</html>

menu.html

<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>Leafora Veg - Menu</title>
    <link rel="stylesheet" href="index.css">
</head>
<body>
<header>
    <h1>Leafora Veg Restaurant</h1>
</header>

<nav>
    <a href="home.html">Home</a>
    <a href="menu.html">Menu</a>
    <a href="admin.html">Administration</a>
    <a href="contact.html">Contact Us</a>
</nav>

<section>
    <h2>Our Vegetarian Menu</h2>
    <div class="menu-grid">
        <div class="card"><img src="paneer.png"><p>Paneer Butter Masala - ₹250</p></div>
        <div class="card"><img src="naan.jpeg"><p>Naan - ₹100</p></div>
        <div class="card"><img src="rice.jpg"><p>Veg Friedrice - ₹180</p></div>
        <div class="card"><img src="noodle.jpg"><p>Veg Noodles - ₹150</p></div>
        <div class="card"><img src="tikka.jpg"><p>Paneer Tikka - ₹200</p></div>
        <div class="card"><img src="biryani.jpeg"><p>Veg Biryani - ₹170</p></div>
    </div>
</section>

</body>
</html>

admin.html

<!DOCTYPE html>
<html>
<head>
    <title>GreenLeaf Veg - Administration</title>
    <link rel="stylesheet" href="index.css">
</head>
<body>
<header>
    <h1> Leafora </h1> Veg Restaurant</h1>
</header>

<nav>
    <a href="home.html">Home</a>
    <a href="menu.html">Menu</a>
    <a href="admin.html">Administration</a>
    <a href="contact.html">Contact Us</a>
</nav>

<section>
    <h2>Meet Our Team</h2>
    <div class="team-grid">
        <div class="card"><img src="cook.jpeg"><p>Person 1 - Head Chef</p></div>
        <div class="card"><img src="man.jpeg"><p>Person 2 - Manager</p></div>
    </div>
</section>

</body>
</html>

contact.html

<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>GreenLeaf Veg - Contact Us</title>
    <link rel="stylesheet" href="index.css">
</head>
<body>
<header>
    <h1>Leafora Veg Restaurant</h1>
</header>

<nav>
    <a href="home.html">Home</a>
    <a href="menu.html">Menu</a>
    <a href="admin.html">Administration</a>
    <a href="contact.html">Contact Us</a>
</nav>

<section>
    <div class="contact-container">
        <h2>Contact Us</h2>
        <p><b>Address:</b> 123 Green Street, Veg City, Tamil Nadu 600201</p>
        <p><b>Phone:</b> +91 9876543210</p>
        <p><b>Email:</b> contact@leafora.com</p>
        <p><b>Opening Hours:</b> Mon-Sun: 10:00 AM - 11:00 PM</p>
    </div>
</section>
</body>
</html>

index.css

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    margin: 0;
    color: #0A2540;

    background-image:
        linear-gradient(rgba(255,255,255,0.7), rgba(255,255,255,0.7)),
        url("background.jpg");
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
}


/* Header */
header {
    background: linear-gradient(
        90deg,
        #03073e,   /* dark navy */
        #07108a,   /* medium blue */
        #2f3be8    /* light blue */
    ); 
    color: #ffffff;
    padding: 22px;
    text-align: center;
    letter-spacing: 1px;
}

/* Navigation */
nav {
    background-color: #020b21; 
    text-align: center;
}

nav a {
    color: #ffffff;
    text-decoration: none;
    margin: 0 18px;
    padding: 10px;
    display: inline-block;
    font-weight: 600;
    transition: 0.3s ease;
}

nav a:hover {
    background-color: #4DA3FF; /* sky blue hover */
    color: #0A2540;
    border-radius: 6px;
}

/* Section */
section {
    padding: 40px;
    text-align: center;
}

/* Headings */
h2 {
    font-family: 'Courgette', cursive;
    color: #163A5F; /* rich blue */
    font-weight: 700;
    letter-spacing: 0.5px;
}

/* Grid Layout */
.menu-grid, .team-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 25px;
    max-width: 1000px;
    margin: 30px auto;
    text-align: center;
}

/* Cards */
.card {
    background-color: #f1f6f8;
    padding: 18px;
    border-radius: 14px;
    box-shadow: 0 9px 17px rgba(173, 5, 228, 0.12);
    color: #030357;
    font-weight: 600;
    border: 4px solid #1a32c7fc; 
    transition: transform 0.3s ease;
}

.card:hover {
    transform: translateY(-6px);
}

/* Images */
.card img {
    width: 90px;
    height: 110px;
    object-fit: cover;
    border-radius: 18px;
}

/* Footer */
footer {
    background-color: #0A2540;
    color: #ffffff;
    text-align: center;
    padding: 18px;
    font-size: 14px;
    letter-spacing: 0.5px;
}

/* Contact Section */
.contact-container {
    max-width: 800px;
    margin: 0 auto;
    text-align: left;
    padding: 25px;
    background-color: #ffffff;
    border-radius: 14px;
    box-shadow: 0 8px 18px rgba(0,0,0,0.12);
    border: 6px dashed #a50bd8; 
}


.contact-container h2 {
    text-align: center;
    color: #0A2540;
}

.contact-container p {
    font-size: 18px;
    margin: 12px 0;
    color: #163A5F;
}

.contact-container b {
    color: #0A2540;
}
.logo {
  border: 3px solid #0a0a0a00;
  padding: 15px;
  border-radius: 15px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.2);
}
~~~
## OUTPUT:
<img width="1048" height="461" alt="Screenshot 2025-12-26 134633" src="https://github.com/user-attachments/assets/dbcae8cb-d80e-463e-8bbd-3ec26d67f321" />
<img width="1043" height="485" alt="Screenshot 2025-12-26 134652" src="https://github.com/user-attachments/assets/4ae98249-800b-4a04-aa63-d08d03102fde" />
<img width="1035" height="474" alt="Screenshot 2025-12-26 134714" src="https://github.com/user-attachments/assets/fdf28d23-4c6d-405e-a9b5-26d1dd2a6d61" />
<img width="1047" height="474" alt="Screenshot 2025-12-26 134725" src="https://github.com/user-attachments/assets/d0c39bf6-e869-4230-ac65-6a9a9a57c9ec" />
## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
