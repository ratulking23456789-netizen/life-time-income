<!DOCTYPE html>
<html>

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Online BD</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Segoe UI;
        }

        body {
            background: linear-gradient(-45deg, #000428, #004e92, #0f2027, #2c5364);
            background-size: 400% 400%;
            animation: bg 12s infinite alternate;
            color: white;
            min-height: 100vh;
        }

        @keyframes bg {
            0% {
                background-position: 0% 50%;
            }

            100% {
                background-position: 100% 50%;
            }
        }

        nav {
            display: flex;
            justify-content: center;
            gap: 15px;
            padding: 20px;
            background: rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(15px);
        }

        nav button {
            padding: 10px 18px;
            border: none;
            border-radius: 25px;
            background: rgba(255, 255, 255, 0.1);
            color: white;
            cursor: pointer;
            transition: 0.4s;
        }

        nav button:hover {
            background: #00f2fe;
            transform: scale(1.1);
        }

        .section {
            display: none;
            padding: 40px;
            text-align: center;
            animation: fade 0.6s ease;
        }

        @keyframes fade {
            from {
                opacity: 0;
                transform: translateY(20px);
            }

            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .active {
            display: block;
        }

        .card {
            background: rgba(255, 255, 255, 0.08);
            padding: 30px;
            border-radius: 20px;
            max-width: 900px;
            margin: auto;
            backdrop-filter: blur(20px);
        }

        input {
            padding: 10px;
            margin: 10px;
            border-radius: 10px;
            border: none;
        }

        .btn {
            padding: 8px 18px;
            border: none;
            border-radius: 20px;
            cursor: pointer;
            background: #00f2fe;
            color: black;
            margin: 5px;
        }

        .hidden {
            display: none;
        }
    </style>
</head>

<body>

    <nav>
        <button onclick="show('home')">হোম</button>
        <button onclick="show('work')">কাজ</button>
        <button onclick="show('admin')">এডমিন কনটাক্ট</button>
        <button onclick="showPayment()">পেমেন্ট</button>
        <button onclick="show('login')">Login</button>
    </nav>

    <!-- HOME -->
    <div id="home" class="section active">
        <div class="card">
            <h2>Online BD</h2>
            <p>
                Online BD একটি বিশ্বস্ত অনলাইন আয়ের প্ল্যাটফর্ম, যেখানে আপনি ঘরে বসে বিভিন্ন সহজ কাজ করে উপার্জন করতে
                পারবেন।
            </p>
        </div>
    </div>

    <!-- WORK -->
    <div id="work" class="section">
        <div class="card">
            <h2>কাজসমূহ</h2>
            <p>🎥 ভিডিও দেখে আয়</p>
            <p>✉️ জিমেইল মার্কেটিং</p>
            <p>💬 Telegram কাজ</p>
            <p>📱 WhatsApp কাজ</p>
        </div>
    </div>

    <!-- ADMIN -->
    <div id="admin" class="section">
        <div class="card">
            <h2>এডমিন কন্টাক্ট</h2>
            <p>
                একাউন্ট সংক্রান্ত যেকোনো বিষয়ে যোগাযোগ করুন:
            </p>
            <p>Telegram: <b>@mhlahab11</b></p>
        </div>
    </div>

    <!-- LOGIN -->
    <div id="login" class="section">
        <div class="card">
            <h2>Login</h2>
            <input type="text" id="user" placeholder="Username"><br>
            <input type="password" id="pass" placeholder="Password"><br>
            <input type="text" id="code" placeholder="Security Code"><br>
            <button class="btn" onclick="login()">Login</button>
            <p id="msg"></p>
        </div>
    </div>

    <!-- DASHBOARD -->
    <div id="dashboard" class="section">
        <div class="card">
            <h2>👤 Profile Dashboard</h2>
            <p>Welcome lahab49</p>

            <button class="btn" onclick="showGmail()">Gmail</button>
            <button class="btn" onclick="showTelegram()">Telegram</button>
            <button class="btn" onclick="showWhatsApp()">WhatsApp</button>

            <div id="demoArea"></div>

            <button class="btn" onclick="logout()">Logout</button>
        </div>
    </div>

    <!-- PAYMENT -->
    <div id="payment" class="section">
        <div class="card">
            <h2>Payment Section</h2>
            <p>Login করার পর পেমেন্ট তথ্য দেখা যাবে।</p>
        </div>
    </div>

    <script>
        let logged=false;

function show(id){
document.querySelectorAll(".section").forEach(sec=>sec.classList.remove("active"));
document.getElementById(id).classList.add("active");
}

function login(){
let u=user.value;
let p=pass.value;
let c=code.value;

if(u==="lahab49" && p==="lahab11" && c==="52152311"){
logged=true;
show("dashboard");
}else{
msg.innerText="ভুল তথ্য দিয়েছেন";
}
}

function logout(){
logged=false;
show("home");
}

function showPayment(){
if(logged){
show("payment");
}else{
alert("Login করতে হবে");
}
}

function randomNumber(){
return Math.floor(1000000000 + Math.random()*9000000000);
}

function showGmail(){
demoArea.innerHTML=
<h3>Gmail Demo</h3>
<p>Random Number: ${randomNumber()}</p>
<button class='btn' onclick='showGmail()'>Refresh</button>
;
}function showTelegram(){
demoArea.innerHTML=
<h3>Telegram Demo</h3>
<p>Random Number: ${randomNumber()}</p>
<button class='btn' onclick='showTelegram()'>Refresh</button>
;
}

function showWhatsApp(){
demoArea.innerHTML=
<h3>WhatsApp Demo</h3>
<p>Random Number: ${randomNumber()}</p>
<button class='btn' onclick='showWhatsApp()'>Refresh</button>
;
}

</script>

</body>

</html>
