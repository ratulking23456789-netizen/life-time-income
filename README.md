<!DOCTYPE html>
<html lang="bn">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Online BD Pro</title>

<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:Segoe UI;}
body{
background:linear-gradient(-45deg,#141e30,#243b55,#000428,#004e92);
background-size:400% 400%;
animation:bg 12s ease infinite;
color:#fff;
}

@keyframes bg{
0%{background-position:0% 50%;}
50%{background-position:100% 50%;}
100%{background-position:0% 50%;}
}

nav{
display:flex;
flex-wrap:wrap;
justify-content:center;
gap:10px;
padding:15px;
background:rgba(255,255,255,0.05);
backdrop-filter:blur(10px);
}

nav button{
padding:8px 18px;
border:none;
border-radius:25px;
background:linear-gradient(45deg,#00f5ff,#ff00c8);
color:#fff;
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
padding:30px;
text-align:center;
animation:fade 0.6s ease;
}

@keyframes fade{
from{opacity:0;}to{opacity:1;}
}

.active{display:block;}

.box{
background:rgba(255,255,255,0.08);
padding:25px;
border-radius:20px;
box-shadow:0 0 25px rgba(0,255,255,0.3);
max-width:800px;
margin:auto;
}

input{
padding:10px;
margin:6px;
width:250px;
border:none;
border-radius:10px;
}

.login-btn{
padding:10px 25px;
border:none;
border-radius:20px;
background:linear-gradient(45deg,#ff512f,#dd2476);
color:white;
cursor:pointer;
}

.balance{
font-size:22px;
margin:15px 0;
color:#00ffcc;
}

@media(max-width:600px){
nav{flex-direction:column;}
input{width:90%;}
}
</style>
</head>

<body>

<nav>
<button onclick="show('home')">হোম</button>
<button onclick="show('work')">কাজ</button>
<button onclick="show('admin')">এডমিন</button>
<button onclick="show('payment')">পেমেন্ট</button>
<button onclick="show('login')">Login</button>
<button onclick="logout()">Logout</button>
</nav>

<!-- HOME -->
<div id="home" class="section active">
<div class="box">
<h1>🌐 Online BD Pro</h1>
<p>Online BD একটি বিশ্বস্ত অনলাইন আয়ের প্ল্যাটফর্ম...</p>
</div>
</div>

<!-- WORK -->
<div id="work" class="section">
<div class="box">
<h2>📌 কাজের তালিকা</h2>
<p>🎥 ভিডিও দেখে আয়</p>
<p>✉️ জিমেইল মার্কেটিং</p>
<p>💬 টেলিগ্রাম কাজ</p>
<p>📱 হোয়াটসঅ্যাপ কাজ</p>
<button onclick="earn()">কাজ সম্পন্ন করুন (+100৳)</button>
</div>
</div>

<!-- ADMIN -->
<div id="admin" class="section">
<div class="box">
<h2>👤 এডমিন কন্টাক্ট</h2>
<p>Telegram: <b>@mhlahab11</b></p>
<p>একাউন্ট করতে সরাসরি এডমিনের সাথে যোগাযোগ করুন।</p>
</div>
</div>

<!-- PAYMENT -->
<div id="payment" class="section">
<div class="box">
<h2>💳 পেমেন্ট</h2>
<div class="balance">আপনার ব্যালেন্স: <span id="balance">0</span> ৳</div>
<p>৫০০৳ হলে পেমেন্ট রিকোয়েস্ট করতে পারবেন।</p>
<button onclick="requestPayment()">পেমেন্ট রিকোয়েস্ট</button>
<p id="paymsg"></p>
</div>
</div>

<!-- LOGIN -->
<div id="login" class="section">
<div class="box">
<h2>🔐 Login</h2>
<input type="text" id="username" placeholder="Username"><br>
<input type="password" id="password" placeholder="Password"><br>
<input type="text" id="code" placeholder="Security Code"><br>
<button class="login-btn" onclick="login()">Login</button>
<p id="msg"></p>
</div>
</div>

<script>

let userBalance = 0;

function show(id){
document.querySelectorAll('.section').forEach(sec=>{
sec.classList.remove('active');
});
document.getElementById(id).classList.add('active');
}

function login(){
let user=document.getElementById("username").value;
let pass=document.getElementById("password").value;
let code=document.getElementById("code").value;

if(user==="lahab49" && pass==="lahab11" && code==="52152311"){
localStorage.setItem("loginTime",Date.now());
document.getElementById("msg").innerHTML="✅ Login Successful!";
show("home");
}
else{
document.getElementById("msg").innerHTML="❌ ভুল তথ্য!";
}
}

function logout(){
localStorage.removeItem("loginTime");
location.reload();
}window.onload=function(){
let loginTime=localStorage.getItem("loginTime");
if(loginTime){
let diff=Date.now()-loginTime;
if(diff>3600000){
localStorage.removeItem("loginTime");
alert("Session Expired! আবার Login করুন");
}
}
}

function earn(){
userBalance+=100;
document.getElementById("balance").innerText=userBalance;
}

function requestPayment(){
if(userBalance>=500){
document.getElementById("paymsg").innerHTML="✅ পেমেন্ট রিকোয়েস্ট পাঠানো হয়েছে!";
userBalance=0;
document.getElementById("balance").innerText=userBalance;
}
else{
document.getElementById("paymsg").innerHTML="❌ ৫০০৳ না হলে রিকোয়েস্ট করা যাবে না!";
}
}

</script>

</body>
</html>
