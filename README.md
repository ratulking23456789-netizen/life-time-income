<!DOCTYPE html>
<html lang="bn">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Online BD Extreme 8K</title>

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Segoe UI',sans-serif;
}

body{
background:linear-gradient(-45deg,#000000,#0f2027,#1a2a6c,#b21f1f,#fdbb2d,#141e30);
background-size:800% 800%;
animation:bgMove 20s ease infinite;
color:white;
overflow-x:hidden;
}

@keyframes bgMove{
0%{background-position:0% 50%;}
50%{background-position:100% 50%;}
100%{background-position:0% 50%;}
}

/* Floating Glow Effect */
body::before{
content:"";
position:fixed;
width:600px;
height:600px;
background:radial-gradient(circle,rgba(0,255,255,0.4),transparent 70%);
top:-200px;
left:-200px;
animation:float 10s infinite alternate;
}

@keyframes float{
0%{transform:translate(0,0);}
100%{transform:translate(300px,300px);}
}

nav{
width:100%;
display:flex;
justify-content:center;
flex-wrap:wrap;
gap:15px;
padding:25px;
background:rgba(255,255,255,0.05);
backdrop-filter:blur(15px);
box-shadow:0 0 40px rgba(0,255,255,0.5);
position:sticky;
top:0;
z-index:1000;
}

nav button{
padding:14px 30px;
border:none;
border-radius:40px;
background:linear-gradient(45deg,#00f5ff,#ff00c8);
color:white;
font-size:16px;
font-weight:bold;
cursor:pointer;
transition:0.4s;
}

nav button:hover{
transform:scale(1.15);
box-shadow:0 0 25px cyan;
}

.section{
display:none;
padding:80px 10%;
min-height:80vh;
animation:fade 0.7s ease;
}

@keyframes fade{
from{opacity:0;}
to{opacity:1;}
}

.active{display:block;}

.box{
background:rgba(255,255,255,0.08);
padding:50px;
border-radius:30px;
box-shadow:0 0 50px rgba(0,255,255,0.4);
width:100%;
max-width:1200px;
margin:auto;
font-size:18px;
line-height:1.8;
}

h1{
font-size:48px;
margin-bottom:20px;
background:linear-gradient(45deg,#00f5ff,#ff00c8);
-webkit-background-clip:text;
color:transparent;
}

h2{
font-size:36px;
margin-bottom:20px;
}

input{
padding:15px;
margin:10px;
width:320px;
border:none;
border-radius:15px;
font-size:16px;
}

button.action{
padding:14px 35px;
border:none;
border-radius:30px;
background:linear-gradient(45deg,#ff512f,#dd2476);
color:white;
font-size:16px;
cursor:pointer;
margin:10px;
transition:0.4s;
}

button.action:hover{
transform:scale(1.1);
box-shadow:0 0 20px #ff00c8;
}

.balance{
font-size:26px;
color:#00ffcc;
margin:20px;
}

.hidden{display:none;}

@media(max-width:768px){
.section{padding:40px 5%;}
h1{font-size:32px;}
}
</style>
</head>

<body>

<nav>
<button onclick="show('home')">হোম</button>
<button onclick="show('work')">কাজ</button>
<button onclick="show('admin')">এডমিন কন্টাক্ট</button>
<button onclick="show('payment')" id="payBtn" class="hidden">পেমেন্ট</button>
<button onclick="show('login')" id="loginBtn">Login</button>
<button onclick="logout()" id="logoutBtn" class="hidden">Logout</button>
</nav>

<!-- HOME -->
<div id="home" class="section active">
<div class="box">
<h1>Online BD</h1>
<p>
Online BD একটি বিশ্বস্ত অনলাইন আয়ের প্ল্যাটফর্ম...
</p>
<br>
<p>💰 রেফার ইনকাম</p>
<p>🎥 ভিডিও দেখে আয়</p>
<p>✉️ জিমেল মার্কেটিং</p>
<p>💬 Telegram অ্যাকাউন্ট</p>
<p>📱 WhatsApp অ্যাকাউন্ট</p>
<p>⌨️ Typing Job</p>
</div>
</div>

<!-- WORK -->
<div id="work" class="section">
<div class="box">
<h2>কাজ নির্বাচন করুন</h2>
<button class="action" onclick="openTask('gmail')">Gmail</button>
<button class="action" onclick="openTask('telegram')">Telegram</button>
<button class="action" onclick="openTask('whatsapp')">WhatsApp</button>
<div id="taskArea"></div>
</div>
</div>

<!-- ADMIN -->
<div id="admin" class="section">
<div class="box">
<h2>এডমিন কন্টাক্ট</h2>
<p>Telegram ID: @mhlahab11</p>
<p>একাউন্ট করার জন্য সরাসরি এডমিনের সাথে যোগাযোগ করুন।</p>
</div>
</div>

<!-- PAYMENT -->
<div id="payment" class="section">
<div class="box">
<h2>পেমেন্ট সিস্টেম</h2>
<div class="balance">Balance: <span id="balance">0</span> ৳</div>
<button class="action" onclick="requestPayment()">পেমেন্ট রিকোয়েস্ট</button>
<p id="paymsg"></p>
</div>
</div><!-- LOGIN -->
<div id="login" class="section">
<div class="box">
<h2>Secure Login</h2>
<input type="text" id="username" placeholder="Username"><br>
<input type="password" id="password" placeholder="Password"><br>
<input type="text" id="code" placeholder="Security Code"><br>
<button class="action" onclick="login()">Login</button>
<p id="msg"></p>
</div>
</div>

<script>
let balance=0;

function show(id){
document.querySelectorAll('.section').forEach(s=>s.classList.remove('active'));
document.getElementById(id).classList.add('active');
}

function login(){
let u=username.value;
let p=password.value;
let c=code.value;

if(u==="lahab49" && p==="lahab11" && c==="52152311"){
msg.innerHTML="✅ Login Successful!";
payBtn.classList.remove("hidden");
logoutBtn.classList.remove("hidden");
loginBtn.classList.add("hidden");
show("home");
}else{
msg.innerHTML="❌ ভুল তথ্য!";
}
}

function logout(){
location.reload();
}

function openTask(type){
let codes={
gmail:"385729",
telegram:"38382",
whatsapp:"521523"
};

taskArea.innerHTML=
<br>
<input type="text" id="taskCode" placeholder="Enter Security Code">
<button class="action" onclick="verify('${codes[type]}')">Verify</button>
<div id="taskResult"></div>
;
}

function verify(correct){
if(document.getElementById("taskCode").value===correct){
generate();
}else{
taskResult.innerHTML="❌ ভুল কোড!";
}
}

function generate(){
let num=Math.floor(1000000000+Math.random()*9000000000);
taskResult.innerHTML=
<p>Fake Number: ${num}</p>
<input type="text" placeholder="Enter OTP">
<br>
<button class="action" onclick="generate()">Refresh</button>
;
balance+=100;
document.getElementById("balance").innerText=balance;
}

function requestPayment(){
if(balance>=500){
paymsg.innerHTML="✅ Payment Requested!";
balance=0;
document.getElementById("balance").innerText=balance;
}else{
paymsg.innerHTML="❌ ৫০০৳ হয়নি!";
}
}
</script>

</body>
</html>
