# ktc-terra-chic-website

index.html

<!DOCTYPE html>
<html>
<head>

<title>KTC Terra Chic</title>

<link rel="stylesheet" href="style.css">

</head>

<body>


<!-- NAVBAR -->
<div class="navbar">

<h1>KTC Terra Chic</h1>

<div class="menu">

<a href="index.html">Home</a>
<a href="products.html">Products</a>

</div>

</div>


<!-- FULL WIDTH SLIDER IMAGE -->
<div class="slider">

<img src="jewel1.png">

</div>


<!-- ABOUT SECTION -->
<div class="about">

<div class="about-text">

<h2>About KTC Terra Chic</h2>

<p>

Welcome to KTC Terra Chic ,where tradition meets elegance in every handcrafted piece.
We specialize in premium terracotta jewellery that blends earthy charm with modern sophistication.
Designed for women who appreciate autenticity and sustainability,our collections celebrate timeless beauty 
and cultural artistry. We offers eco-friendly handmade terracotta jewellery.  
Each piece is handcrafted with care,giving you elegance,tradition,  
and affordable luxury.


</p>

</div>

<div class="about-img">

<img src="logo.jpeg">

</div>

</div>



<!-- SHOP NOW BUTTON -->
<div class="shopnow-container">

<a href="products.html?show=collection">

<button class="shopnow-main">

    SHOP NOW ➜

</button>

</a>

</div>



<!-- COLLECTION SECTION -->
<h2 class="collection-title">Our Collections</h2>

<div class="vertical-images">

<div class="card">

<img src="Jewel2.png">

<p>Traditional Necklace – ₹650</p>

</div>


<div class="card">

<img src="jewel3.jpeg">

<p>Designer Jewellery – ₹349</p>

</div>


<div class="card">

<img src="jewe4.jpeg">

<p>Terracotta Earrings – ₹199</p>

</div>

</div>

<!-- Seemore BUTTON-->
<div class="seemore-container">

<a href="products.html?show=collection">

<button class="seemore-main">

See More

</button>

</a>

</div>



<!-- FOOTER -->
<footer class="footer">

<p>Crafting Uniqueness, Celebrating Togetherness</p>

<p>
24, Lotus Street, Anna Nagar, Chennai-600017<br>
kanisha@gmail.com | +91 9876543210<br>
Instagram: @ktc_fashions<br>
Facebook:@ktc_fashions

</p>

</footer>


</body>
</html>

products.html 
<!DOCTYPE html>
<html>
<head>

<title>KTC Terra Chic Products</title>

<link rel="stylesheet" href="style.css">

<script>

/* DROPDOWN FUNCTION */

function showView(value)
{

document.getElementById("collection").style.display="none";
document.getElementById("three").style.display="none";

document.getElementById(value).style.display="grid";

}


/* AUTO OPEN COLLECTION WHEN SHOP NOW CLICKED */

window.onload = function()
{

const params = new URLSearchParams(window.location.search);

if(params.get("show") === "collection")
{
document.getElementById("collection").style.display="grid";
}

}

</script>

</head>


<body>


<!-- NAVBAR -->
<div class="navbar">

<h1>KTC Terra Chic</h1>

<div class="menu">

<a href="index.html">Home</a>
<a href="products.html">Products</a>

</div>

</div>



<!-- DROPDOWN -->
<div class="dropdown">

<select onchange="showView(this.value)">

<option value="collection">Grid showView</option>

<option value="three">Featured Collection</option>

</select>

</div>



<!-- COLLECTION GRID -->
<div id="collection" class="grid">

<div class="card">

<img src="jewel5.jpeg">

<h3>Classic Necklace</h3>

<p>₹399</p>

<button>Add to Cart</button>

</div>



<div class="card">

<img src="jewel6.jpeg">

<h3>Handmade Set</h3>

<p>₹379</p>

<button>Add to Cart</button>

</div>



<div class="card">

<img src="jewel7.jpeg">

<h3>Premium Jewellery</h3>

<p>₹999</p>

<button>Add to Cart</button>

</div>



<div class="card">

<img src="jewel3.jpeg">

<h3>Designer Necklace</h3>

<p>₹349</p>

<button>Add to Cart</button>

</div>



<div class="card">

<img src="jewel8.jpeg">

<h3>Terracotta Earrings</h3>

<p>₹399</p>

<button>Add to Cart</button>

</div>



<div class="card">

<img src="jewel9.jpeg">

<h3>Luxury Collection</h3>

<p>₹999</p>

<button>Add to Cart</button>

</div>


</div>



<!-- FEATURED COLLECTION -->
<div id="three" class="grid">

<div class="card">

<img src="jewel12.jpeg">

<p>₹319</p>

<button>Add to Cart</button>

</div>


<div class="card">

<img src="jewel10.jpeg">

<p>₹499</p>

<button>Add to Cart</button>

</div>


<div class="card">

<img src="jewel11.jpeg">

<p>₹299</p>

<button>Add to Cart</button>

</div>

</div>



<!-- FOOTER -->
<footer class="footer">

<p>Crafting Uniqueness, Celebrating Togetherness</p>

<p>
24, Lotus Street, Anna Nagar, Chennai<br>
kanisha@gmail.com | +91 9876543210<br>
Instagram: @ktc_fashions
</p>

</footer>


</body>
</html>

style.css
body
{

margin:0;

font-family:Great Vibes;

background:#f5efe6;

}


/* NAVBAR */
.navbar
{

background:#5a2d2d;

color:#D4AF37;

text-align:center;

padding:20px;

}

.menu a
{

color:white;

margin:10px;

text-decoration:none;

font-size:18px;

}



/* SLIDER */
.slider img
{

width:100%;

height:500px;

object-fit:cover;

}



/* ABOUT */
.about
{

display:flex;

justify-content:space-around;

align-items:center;

padding:40px;

}

.about img
{

width:300px;

}



/* SHOP NOW BUTTON */
.shopnow-container
{

text-align:center;

margin:30px;

}

.shopnow-main
{

background:#8B5E3C;

color:white;

padding:15px 40px;

border:none;

font-size:18px;

cursor:pointer;

border-radius:6px;

}

.shopnow-main:hover
{

background:#D4AF37;

color:black;

}



/* COLLECTION */
.collection-title
{

text-align:center;

margin-top:30px;

}

.vertical-images
{

display:flex;

flex-direction:column;

align-items:center;

gap:20px;

margin-bottom:40px;

}



/* GRID */
.grid
{

display:grid;

grid-template-columns:repeat(3,1fr);

gap:20px;

padding:30px;

}


/* CARD */
.card
{

background:white;

padding:15px;

text-align:center;

border-radius:8px;

box-shadow:0 0 10px gray;

}

.card img
{

width:100%;

height:250px;

object-fit:cover;

}

.card button
{

background:#5a2d2d;

color:white;

border:none;

padding:10px;

cursor:pointer;

margin-top:10px;

}



/* DROPDOWN */
.dropdown
{

text-align:center;

margin:20px;

}

/* See More BUTTON */
.seemore-container
{

text-align:center;

margin:20px;

}

.seemore-main
{

background:#8B5E3C;

color:white;

padding:10px 20px;

border:none;

font-size:16px;

cursor:pointer;

border-radius:5px;

}

.seemore-main:hover
{

background:#D4AF37;

color:black;

}


/* FOOTER */
.footer
{

background:#5a2d2d;

color:white;

text-align:center;

padding:20px;

margin-top:40px;

}

