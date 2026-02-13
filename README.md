<!DOCTYPE html>
<html lang="bn">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Online BD Premium</title>

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Segoe UI',sans-serif;
}

body{
background:linear-gradient(135deg,#141e30,#243b55,#0f2027);
background-size:400% 400%;
animation:bg 12s ease infinite;
color:white;
min-height:100vh;
}

@keyframes bg{
0%{background-position:0% 50%;}
50%{background-position:100% 50%;}
100%{background-position:0% 50%;}
}

nav{
display:flex;
justify-content:center;
gap:15px;
padding:20px;
background:rgba(255,255,255,0.05);
backdrop-filter:blur(10px);
box-shadow:0 0 20px rgba(0,255,255,0.3);
flex-wrap:wrap;
}

nav button{
padding:10px 22px;
border:none;
border-radius:25px;
background:linear-gradient(45deg,#00f5ff,#ff00c8);
color:white;
cursor:pointer;
font-weight:bold;
transition:0.3s;
}

nav button:hover{
transform:scale(1.1);
box-shadow:0 0 15px cyan;
}

.section{
display:none;
padding:60px 10%;
animation:fade 0.5s ease;
min-height:80vh;
}

@keyframes fade{
from{opacity:0;}
to{opacity:1;}
}

.active{
display:block;
}

.box{
background:rgba(255,255,255,0.08);
padding:40px;
border-radius:20px;
box-shadow:0 0 25px rgba(0,255,255,0.3);
max-width:1000px;
margin:auto;
}

h1{
font-size:40px;
margin-bottom:20px;
background:linear-gradient(45deg,#00f5ff,#ff00c8);
-webkit-background-clip:text;
color:transparent;
}

h2{
margin-bottom:20px;
}

input{
padding:12px;
margin:8px;
width:260px;
border:none;
border-radius:10px;
font-size:15px;
}

button.action{
padding:10px 25px;
border:none;
border-radius:25px;
background:linear-gradient(45deg,#ff512f,#dd2476);
color:white;
cursor:pointer;
font-weight:bold;
margin-top:10px;
}

.balance{
font-size:22px;
color:#00ffcc;
margin:15px 0;
}

.hidden{
display:none;
}

@media(max-width:768px){
.section{padding:40px 5%;}
}
</style>
</head>

<body>

<nav>
<button onclick="showSection('home')">হোম</button>
<button onclick="showSection('work')">কাজ</button>
<button onclick="showSection('admin')">এডমিন কন্টাক্ট</button>
<button onclick="showSection('payment')" id="paymentBtn" class="hidden">পেমেন্ট</button>
<button onclick="showSection('login')" id="loginBtn">Login</button>
<button onclick="logout()" id="logoutBtn" class="hidden">Logout</button>
</nav>

<!-- HOME -->
<div id="home" class="section active">
<div class="box">
<h1>Online BD</h1>
<p>
Online BD একটি বিশ্বস্ত অনলাইন আয়ের প্ল্যাটফর্ম, যেখানে আপনি ঘরে বসে বিভিন্ন সহজ কাজ করে উপার্জন করতে পারবেন।
আমাদের মূল লক্ষ্য হলো তরুণ প্রজন্মকে অনলাইন জগতে দক্ষ করে তোলা এবং তাদের আর্থিকভাবে স্বাবলম্বী করে তোলা।
</p>

<br>
<p>💰 রেফার ইনকাম</p>
<p>🎥 ভিডিও দেখে আয়</p>
<p>✉️ জিমেল মার্কেটিং</p>
<p>💬 Telegram অ্যাকাউন্ট তৈরি</p>
<p>📱 WhatsApp অ্যাকাউন্ট তৈরি</p>
<p>⌨️ Typing Job</p>
</div>
</div>

<!-- WORK -->
<div id="work" class="section">
<div class="box">
<h2>কাজ</h2>
<p>🎥 ভিডিও দেখে আয়</p>
<p>✉️ জিমেইল মার্কেটিং</p>
<p>💬 টেলিগ্রাম কাজ</p>
<p>📱 হোয়াটসঅ্যাপ অ্যাকাউন্ট কাজ</p>
</div>
</div>

<!-- ADMIN -->
<div id="admin" class="section">
<div class="box">
<h2>এডমিন কন্টাক্ট</h2>
<p><b>Telegram:</b> @mhlahab11</p>
<p>একাউন্ট করার জন্য সরাসরি এডমিনের সাথে যোগাযোগ করুন।</p>
</div>
</div>

<!-- PAYMENT -->
<div id="payment" class="section">
<div class="box">
<h2>পেমেন্ট</h2>
<div class="balance">Balance: <span id="balance">0</span> ৳</div>
<button class="action" onclick="addBalance()">ডেমো ইনকাম +100৳</button>
</div>
</div>

<!-- LOGIN -->
<div id="login" class="section">
<div class="box">
<h2>Secure Login</h2>
<input type="text" id="username" placeholder="Username"><br>
<input type="password" id="password" placeholder="Password"><br>
<input type="text" id="securityCode" placeholder="Security Code"><br>
<button type="button" class="action" onclick="login()">Login</button>
<p id="loginMsg"></p>
</div>
</div>

<script>

let balance = 0;
let isLoggedIn = false;

function showSection(id){
document.querySelectorAll('.section').forEach(sec=>{
sec.classList.remove('active');
});
document.getElementById(id).classList.add('active');
} function login(){
let user = document.getElementById("username").value;
let pass = document.getElementById("password").value;
let code = document.getElementById("securityCode").value;

if(user==="lahab49" && pass==="lahab11" && code==="52152311"){
isLoggedIn = true;
document.getElementById("loginMsg").innerHTML="✅ Login Successful!";
document.getElementById("paymentBtn").classList.remove("hidden");
document.getElementById("logoutBtn").classList.remove("hidden");
document.getElementById("loginBtn").classList.add("hidden");
showSection("home");
}else{
document.getElementById("loginMsg").innerHTML="❌ ভুল তথ্য দিয়েছেন!";
}
}

function logout(){
location.reload();
}

function addBalance(){
if(isLoggedIn){
balance += 100;
document.getElementById("balance").innerText = balance;
}else{
alert("Login না করলে ব্যালেন্স বাড়বে না!");
}
}

</script>

</body>
</html>
