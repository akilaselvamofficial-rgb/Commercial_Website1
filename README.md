# Ex02 Commercial Website
## Date:01-08-2025

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
```
index.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Groom & Loom | Home</title>

    <link rel="stylesheet" href="style.css">
</head>

<body>

    <!-- Header -->
    <header>

        <div class="logo">
            Groom & Loom
        </div>

        <nav>
            <ul>
                <li><a href="index.html" class="active">Home</a></li>
                <li><a href="products.html">Products</a></li>
                <li><a href="about.html">About</a></li>
                <li><a href="contact.html">Contact</a></li>
            </ul>
        </nav>

    </header>

    <!-- Hero Section -->

    <section class="hero">

        <div class="overlay"></div>

        <div class="hero-content">

            <h3>WELCOME TO</h3>

            <h1>Groom & Loom</h1>

            <h2>New Fashion Collection 2026</h2>

            <p>
                Discover premium quality clothing for men and women.
                Upgrade your style with our latest fashion trends.
            </p>

            <a href="products.html" class="btn">
                Shop Now
            </a>

        </div>

    </section>

    <!-- Featured Products -->

    <section class="featured">

        <h2>Featured Products</h2>

        <div class="product-container">

            <div class="product-card">

                <img src="p1.png" alt="Shirt">

                <h3>URB_N Men Textured Shirt</h3>

                <p class="price">₹899</p>

                <button>Buy Now</button>

            </div>

            <div class="product-card">

                <img src="p2.png" alt="Shirt">

                <h3>Men Regular Fit Solid Shirt</h3>

                <p class="price">₹599</p>

                <button>Buy Now</button>

            </div>

            <div class="product-card">

                <img src="p3.png" alt="Shirt">

                <h3>URB_N Men Printed Resort Shirt</h3>

                <p class="price">₹699</p>

                <button>Buy Now</button>

            </div>

        </div>

    </section>

    <!-- Why Choose Us -->

    <section class="why-us">

        <h2>Why Choose Groom & Loom?</h2>

        <div class="features">

            <div class="feature-box">

                <h3>Premium Quality</h3>

                <p>High-quality fabrics with stylish designs.</p>

            </div>

            <div class="feature-box">

                <h3>Free Shipping</h3>

                <p>Free delivery on selected orders.</p>

            </div>

            <div class="feature-box">

                <h3>Easy Returns</h3>

                <p>7-day hassle-free return policy.</p>

            </div>

            <div class="feature-box">

                <h3>Secure Payment</h3>

                <p>100% safe and secure online payments.</p>

            </div>

        </div>

    </section>

    <!-- Footer -->

    <footer>

        <p>

            © 2026 Groom & Loom |
            Designed by AKILA S (212225220008)

        </p>

    </footer>
</body>
</html>

style.css
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, Helvetica, sans-serif;
}

body{
    background:#f5f5f5;
    color:#333;
}

/* ==========================
   HEADER
========================== */

header{
    background:#111;
    color:white;
    display:flex;
    justify-content:space-between;
    align-items:center;
    padding:20px 8%;
    position:sticky;
    top:0;
    z-index:1000;
}

.logo{
    font-size:32px;
    font-weight:bold;
    color:#ff4d4d;
    letter-spacing:2px;
}

nav ul{
    display:flex;
    list-style:none;
}

nav ul li{
    margin-left:25px;
}

nav ul li a{
    text-decoration:none;
    color:white;
    font-size:18px;
    padding:10px 18px;
    border-radius:5px;
    transition:.3s;
}

nav ul li a:hover,
nav ul li a.active{
    background:#ff4d4d;
}

/* ==========================
   HERO
========================== */

.hero{
    position:relative;
    height:90vh;
    background:url("i6.png") center center/cover no-repeat;
    display:flex;
    justify-content:center;
    align-items:center;
}

.overlay{
    position:absolute;
    width:100%;
    height:100%;
    background:rgba(0,0,0,.45);
}

.hero-content{
    position:relative;
    text-align:center;
    color:white;
    z-index:2;
}

.hero-content h3{
    font-size:24px;
    letter-spacing:5px;
    margin-bottom:10px;
}

.hero-content h1{
    font-size:65px;
    color:#ff4d4d;
    margin-bottom:15px;
}

.hero-content h2{
    font-size:42px;
    margin-bottom:20px;
}

.hero-content p{
    font-size:20px;
    width:700px;
    max-width:90%;
    margin:auto;
    line-height:1.7;
}

/* ==========================
   BUTTON
========================== */

.btn{
    display:inline-block;
    margin-top:45px;
    padding:15px 40px;
    background:#ff4d4d;
    color:white;
    text-decoration:none;
    border-radius:6px;
    font-size:18px;
    transition:.3s;
}

.btn:hover{
    background:#111;
}

/* ==========================
   FEATURED PRODUCTS
========================== */

.featured{
    padding:80px 8%;
    text-align:center;
    background:white;
}

.featured h2{
    font-size:42px;
    margin-bottom:50px;
}

.product-container{
    display:flex;
    justify-content:center;
    gap:35px;
    flex-wrap:wrap;
}

.product-card{
    width:320px;
    background:white;
    border-radius:10px;
    overflow:hidden;
    box-shadow:0 5px 15px rgba(0,0,0,.15);
    transition:.3s;
}

.product-card:hover{
    transform:translateY(-10px);
}

.product-card img{
    width:100%;
    height:360px;
    object-fit:cover;
}

.product-card h3{
    padding:18px 15px 8px;
    font-size:22px;
}

.price{
    color:#ff4d4d;
    font-size:24px;
    font-weight:bold;
    margin-bottom:15px;
}

.product-card button{
    margin-bottom:20px;
    padding:12px 30px;
    background:#ff4d4d;
    color:white;
    border:none;
    border-radius:5px;
    cursor:pointer;
    font-size:17px;
    transition:.3s;
}

.product-card button:hover{
    background:#111;
}

/* ==========================
   WHY CHOOSE US
========================== */

.why-us{
    background:#f8f8f8;
    padding:80px 8%;
    text-align:center;
}

.why-us h2{
    font-size:40px;
    margin-bottom:45px;
}

.features{
    display:flex;
    justify-content:center;
    gap:25px;
    flex-wrap:wrap;
}

.feature-box{
    width:250px;
    background:white;
    padding:30px;
    border-radius:10px;
    box-shadow:0 5px 15px rgba(0,0,0,.1);
    transition:.3s;
}

.feature-box:hover{
    transform:translateY(-8px);
}

.feature-box h3{
    color:#ff4d4d;
    margin-bottom:15px;
}

.feature-box p{
    line-height:1.6;
}

/* ==========================
   FOOTER
========================== */

footer{
    background:#111;
    color:white;
    text-align:center;
    padding:25px;
    margin-top:30px;
}

/* ==========================
   RESPONSIVE
========================== */

@media(max-width:992px){

    header{
        flex-direction:column;
        padding:20px;
    }

    nav ul{
        margin-top:15px;
    }

    .hero-content h1{
        font-size:50px;
    }

    .hero-content h2{
        font-size:30px;
    }

    .hero-content p{
        width:90%;
        font-size:18px;
    }

    .product-container{
        justify-content:center;
    }
}

@media(max-width:768px){

    nav ul{
        flex-direction:column;
        align-items:center;
    }

    nav ul li{
        margin:10px 0;
    }

    .hero{
        height:75vh;
    }

    .hero-content h1{
        font-size:40px;
    }

    .hero-content h2{
        font-size:25px;
    }

    .featured h2,
    .why-us h2{
        font-size:32px;
    }

    .product-card{
        width:90%;
    }

    .feature-box{
        width:90%;
    }
}
```

## OUTPUT
![alt text](<Screenshot 2026-08-01 134741.png>)
![alt text](<Screenshot 2026-08-01 134819.png>)
![alt text](<Screenshot 2026-08-01 134902.png>)
![alt text](<Screenshot 2026-08-01 134932.png>)
![alt text](<Screenshot 2026-08-01 134951.png>)
![alt text](<Screenshot 2026-08-01 135012.png>)
![alt text](<Screenshot 2026-08-01 135025.png>)
![alt text](<Screenshot 2026-08-01 135049.png>)
![alt text](<Screenshot 2026-08-01 135111.png>)
![alt text](<Screenshot 2026-08-01 135306.png>)
![alt text](<Screenshot 2026-08-01 135329.png>)
## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
