<!DOCTYPE html>
<html>
<head>
<title>Umar Galaxy Emperor | Ultra Luxury</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Segoe UI',sans-serif;
scroll-behavior:smooth;
}

body{
background:black;
color:white;
overflow-x:hidden;
animation:fadeIn 2s ease-in;
}

/* Galaxy Background */
body::before{
content:"";
position:fixed;
width:200%;
height:200%;
background:
radial-gradient(white 1px, transparent 1px),
radial-gradient(#d4af37 1px, transparent 1px);
background-size:50px 50px;
animation:moveStars 60s linear infinite;
z-index:-1;
opacity:0.3;
}

@keyframes moveStars{
from{transform:translate(0,0);}
to{transform:translate(-500px,-500px);}
}

/* Navbar */
nav{
position:fixed;
width:100%;
padding:18px;
text-align:center;
background:rgba(0,0,0,0.8);
backdrop-filter:blur(10px);
z-index:1000;
}

nav a{
color:#d4af37;
margin:20px;
text-decoration:none;
font-size:18px;
letter-spacing:1px;
transition:0.4s;
}

nav a:hover{
color:white;
}

/* Hero */
header{
height:100vh;
display:flex;
flex-direction:column;
justify-content:center;
align-items:center;
text-align:center;
padding:20px;
}

header h1{
font-size:65px;
background:linear-gradient(90deg,#d4af37,#fff,#d4af37);
-webkit-background-clip:text;
color:transparent;
animation:glow 3s infinite alternate;
}

@keyframes glow{
from{text-shadow:0 0 15px gold;}
to{text-shadow:0 0 35px #d4af37;}
}

header p{
font-size:22px;
opacity:0.85;
margin-top:15px;
}

.btn{
margin-top:30px;
padding:14px 40px;
background:#d4af37;
border:none;
border-radius:30px;
font-weight:bold;
cursor:pointer;
transition:0.4s;
}

.btn:hover{
background:white;
transform:scale(1.1);
}

/* Sections */
section{
padding:100px 20px;
text-align:center;
}

h2{
color:#d4af37;
font-size:38px;
margin-bottom:40px;
}

/* Products */
.products{
display:flex;
flex-wrap:wrap;
justify-content:center;
gap:35px;
}

.card{
background:rgba(255,255,255,0.05);
backdrop-filter:blur(15px);
width:280px;
border-radius:20px;
overflow:hidden;
box-shadow:0 15px 40px rgba(212,175,55,0.4);
transition:0.5s;
}

.card:hover{
transform:translateY(-20px) scale(1.08);
box-shadow:0 25px 60px rgba(212,175,55,0.7);
}

.card img{
width:100%;
}

.card h3{
margin:15px 0 5px;
}

.price{
color:#d4af37;
font-weight:bold;
margin-bottom:15px;
}

/* Contact */
.contact-box{
background:rgba(255,255,255,0.05);
backdrop-filter:blur(15px);
padding:40px;
border-radius:20px;
display:inline-block;
box-shadow:0 15px 40px rgba(212,175,55,0.4);
}

/* Footer */
footer{
background:black;
padding:30px;
color:#777;
text-align:center;
}

/* AI Chatbox */
.chat-btn{
position:fixed;
bottom:25px;
right:25px;
background:#d4af37;
color:black;
border:none;
border-radius:50%;
width:60px;
height:60px;
font-size:22px;
cursor:pointer;
box-shadow:0 5px 20px rgba(212,175,55,0.6);
z-index:9999;
}

.chat-box{
position:fixed;
bottom:100px;
right:25px;
width:320px;
background:rgba(0,0,0,0.9);
border-radius:20px;
box-shadow:0 10px 40px rgba(212,175,55,0.6);
display:none;
flex-direction:column;
overflow:hidden;
z-index:9999;
}

.chat-header{
background:#d4af37;
color:black;
padding:12px;
text-align:center;
font-weight:bold;
}

.chat-messages{
height:250px;
overflow-y:auto;
padding:10px;
font-size:14px;
}

.chat-input{
display:flex;
border-top:1px solid #333;
}

.chat-input input{
flex:1;
padding:10px;
border:none;
outline:none;
background:black;
color:white;
}

.chat-input button{
background:#d4af37;
border:none;
padding:10px;
cursor:pointer;
}

.message{margin:8px 0;}
.user{color:#d4af37;}
.bot{color:white;}

@keyframes fadeIn{
from{opacity:0;}
to{opacity:1;}
}
</style>
</head>

<body>

<nav>
<a href="#home">Home</a>
<a href="#about">Empire</a>
<a href="#collection">Collection</a>
<a href="#contact">Contact</a>
</nav>

<header id="home">
<h1>Umar Galaxy Emperor</h1>
<p>Beyond Luxury • Beyond Fashion • Beyond Limits</p>
<button class="btn" onclick="document.getElementById('collection').scrollIntoView()">Enter The Empire</button>
</header>

<section id="about">
<h2>The Royal Empire</h2>
<p>Umar Galaxy Emperor is a symbol of elite fashion and cosmic luxury lifestyle.</p>
</section>

<section id="collection">
<h2>Ultra Pro Max Collection</h2>

<div class="products">

<div class="card">
<img src="https://images.unsplash.com/photo-1523381210434-271e8be1f52b">
<h3>Cosmic Royal Shirt</h3>
<p class="price">₹2999</p>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1512436991641-6745cdb1723f">
<h3>Galaxy Emperor Jacket</h3>
<p class="price">₹5999</p>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1490481651871-ab68de25d43d">
<h3>Infinity Crown Sneakers</h3>
<p class="price">₹4999</p>
</div>

</div>
</section>

<section id="contact">
<h2>Contact The Emperor</h2>
<div class="contact-box">
<p>📧 Email: mohammadumarlone42@gmail.com</p>
<p>📍 Location: Kupwara, Jammu & Kashmir</p>
<p>📞 Phone: 9876543210</p>
</div>
</section>

<footer>
<p>© 2026 Umar Galaxy Emperor | All Rights Reserved</p>
</footer>

<button class="chat-btn" onclick="toggleChat()">💬</button>

<div class="chat-box" id="chatBox">
<div class="chat-header">Emperor AI Assistant</div>
<div class="chat-messages" id="chatMessages"></div>
<div class="chat-input">
<input type="text" id="userInput" placeholder="Ask something...">
<button onclick="sendMessage()">Send</button>
</div>
</div>

<script>
function toggleChat(){
var box=document.getElementById("chatBox");
box.style.display=box.style.display==="flex"?"none":"flex";
}

function sendMessage(){
var input=document.getElementById("userInput");
var messages=document.getElementById("chatMessages");

if(input.value.trim()==="") return;

messages.innerHTML += "<div class='message user'>You: "+input.value+"</div>";

let reply="Welcome to Umar Galaxy Emperor 👑";
let text=input.value.toLowerCase();

if(text.includes("price")) reply="Our premium prices start from ₹2999 👑";
else if(text.includes("location")) reply="We are located in Kupwara, Jammu & Kashmir 📍";
else if(text.includes("contact")) reply="Email us at mohammadumarlone42@gmail.com 📧";
else if(text.includes("hello") || text.includes("hi")) reply="Greetings Emperor 👑 How may I assist you?";
else reply="Our royal team will respond soon 👑";

setTimeout(()=>{
messages.innerHTML += "<div class='message bot'>AI: "+reply+"</div>";
messages.scrollTop=messages.scrollHeight;
},500);

input.value="";
}
</script>

</body>
</html>
