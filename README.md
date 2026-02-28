<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Umar Fashion</title>

<style>
body{
    margin:0;
    font-family:Arial, sans-serif;
    background:#f5f5f5;
}
header{
    display:flex;
    justify-content:space-between;
    padding:15px 50px;
    background:black;
    color:white;
}
nav a{
    color:white;
    margin-left:20px;
    text-decoration:none;
}
.hero{
    height:60vh;
    background:linear-gradient(to right,#000,#555);
    color:white;
    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;
}
.hero h1{font-size:40px;}
.products{
    display:flex;
    flex-wrap:wrap;
    justify-content:center;
    padding:40px;
}
.card{
    background:white;
    width:250px;
    margin:15px;
    padding:15px;
    text-align:center;
    border-radius:10px;
    box-shadow:0 5px 15px rgba(0,0,0,0.2);
    transition:0.3s;
}
.card:hover{
    transform:scale(1.05);
}
button{
    padding:8px 15px;
    border:none;
    background:black;
    color:white;
    cursor:pointer;
}
button:hover{
    background:orange;
}
.cart-box{
    position:fixed;
    top:0;
    right:-300px;
    width:300px;
    height:100%;
    background:white;
    box-shadow:-5px 0 15px rgba(0,0,0,0.2);
    padding:20px;
    transition:0.4s;
}
.cart-box.active{
    right:0;
}
</style>
</head>

<body>

<header>
<div><b>Umar Fashion</b></div>
<nav>
<a href="#">Home</a>
<a href="#" onclick="toggleCart()">Cart (<span id="count">0</span>)</a>
</nav>
</header>

<section class="hero">
<h1>New Collection 2026</h1>
<p>Style That Defines You</p>
</section>

<section class="products">

<div class="card">
<h3>Premium Shirt</h3>
<p>₹999</p>
<button onclick="addToCart('Premium Shirt',999)">Add to Cart</button>
</div>

<div class="card">
<h3>Denim Jacket</h3>
<p>₹1999</p>
<button onclick="addToCart('Denim Jacket',1999)">Add to Cart</button>
</div>

<div class="card">
<h3>Classic Jeans</h3>
<p>₹1499</p>
<button onclick="addToCart('Classic Jeans',1499)">Add to Cart</button>
</div>

</section>

<div class="cart-box" id="cartBox">
<h2>Your Cart</h2>
<div id="cartItems"></div>
<h3>Total: ₹<span id="total">0</span></h3>
<button onclick="toggleCart()">Close</button>
</div>

<script>
let cart=[];
function addToCart(name,price){
    cart.push({name,price});
    document.getElementById("count").innerText=cart.length;
    updateCart();
}
function updateCart(){
    let items="";
    let total=0;
    cart.forEach(item=>{
        items+=`<p>${item.name} - ₹${item.price}</p>`;
        total+=item.price;
    });
    document.getElementById("cartItems").innerHTML=items;
    document.getElementById("total").innerText=total;
}
function toggleCart(){
    document.getElementById("cartBox").classList.toggle("active");
}
</script>

</body>
</html>
