
<html lang="bn">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Online BD - Trusted Earning Platform</title>
    <style>
        /* Premium Background & Animations */
        body {
            margin: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: radial-gradient(circle at center, #1a1a2e 0%, #0f0f1a 100%);
            color: white;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
            overflow-x: hidden;
        }

        /* 4K Lighting Animation */
        body::before {
            content: "";
            position: fixed;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: conic-gradient(from 0deg, transparent, #00d4ff, transparent 30%);
            animation: rotate 10s linear infinite;
            z-index: -1;
            opacity: 0.1;
        }

        @keyframes rotate {
            100% {
                transform: rotate(360deg);
            }
        }

        /* Navbar Design */
        nav {
            width: 100%;
            background: rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(15px);
            padding: 20px 0;
            position: sticky;
            top: 0;
            z-index: 100;
            display: flex;
            justify-content: center;
            gap: 15px;
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
        }

        nav button {
            background: rgba(255, 255, 255, 0.1);
            border: 1px solid rgba(0, 212, 255, 0.5);
            color: white;
            padding: 10px 20px;
            cursor: pointer;
            border-radius: 8px;
            transition: 0.3s;
            font-weight: bold;
            text-transform: uppercase;
        }

        nav button:hover {
            background: #00d4ff;
            box-shadow: 0 0 20px #00d4ff;
            color: #000;
        }

        /* Content Area */
        .container {
            max-width: 800px;
            margin: 40px auto;
            padding: 30px;
            background: rgba(255, 255, 255, 0.03);
            border-radius: 20px;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            text-align: center;
            display: none;
            /* Hidden by default */
            animation: fadeIn 0.8s ease-out;
        }

        .active {
            display: block;
        }

        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(20px);
            }

            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        h1 {
            color: #00d4ff;
            text-shadow: 0 0 10px #00d4ff;
        }

        .list-item {
            background: rgba(255, 255, 255, 0.05);
            margin: 10px 0;
            padding: 15px;
            border-radius: 10px;
            border-left: 5px solid #00d4ff;
            text-align: left;
        }

        /* Login Form */
        input {
            width: 80%;
            padding: 12px;
            margin: 10px 0;
            border-radius: 5px;
            border: none;
            background: rgba(255, 255, 255, 0.1);
            color: white;
            outline: none;
        }

        .login-btn {
            background: linear-gradient(45deg, #00d4ff, #0056b3);
            width: 85%;
            border: none;
            padding: 12px;
            color: white;
            font-weight: bold;
            border-radius: 5px;
            cursor: pointer;
        }
    </style>
</head>

<body>

    <nav>
        <button onclick="showPage('home')">হোম</button>
        <button onclick="showPage('work')">কাজ</button>
        <button onclick="showPage('admin')">এডমিন</button>
        <button onclick="showPage('payment')">পেমেন্ট</button>
        <button onclick="showPage('login')">Login</button>
    </nav> 
    <div id="home" class="container active">
        <h1>Online BD</h1>
        <p>Online BD একটি বিশ্বস্ত অনলাইন আয়ের প্ল্যাটফর্ম, যেখানে আপনি ঘরে বসে বিভিন্ন সহজ কাজ করে উপার্জন করতে পারবেন।
        </p>
        <p>আমাদের মূল লক্ষ্য হলো তরুণ প্রজন্মকে অনলাইন জগতে দক্ষ করে তোলা এবং তাদের আর্থিকভাবে স্বাবলম্বী করে তোলা।</p>
        <div class="list-item">💰 <b>রেফার ইনকাম:</b> লিংক শেয়ার করে প্রতিটি রেফারে আয় করুন।</div>
        <div class="list-item">🎥 <b>ভিডিও দেখে আয়:</b> ভিডিও দেখে পয়েন্ট বা টাকা উপার্জন করুন।</div>
        <div class="list-item">✉️ <b>জিমেল মার্কেটিং:</b> ইমেইল মার্কেটিংয়ের মাধ্যমে ইনকামের সুযোগ।</div>
        <div class="list-item">💬 <b>Telegram কাজ:</b> টেলিগ্রাম অ্যাকাউন্ট খুলে আয় করুন।</div>
        <div class="list-item">📱 <b>WhatsApp কাজ:</b> হোয়াটসঅ্যাপ অ্যাকাউন্ট তৈরি করে আয়।</div>
        <div class="list-item">⌨️ <b>Typing Job:</b> নতুনদের জন্য একদম পারফেক্ট কাজ।</div>
    </div>
    
    <div id="work" class="container">
        <h1>আমাদের কাজসমূহ</h1>
    
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lite Verification</title>
    <style>
        body {
            margin: 0;
            font-family: 'Segoe UI', sans-serif;
            background: linear-gradient(-45deg, #ff9a9e, #fad0c4, #a1c4fd, #c2e9fb);
            background-size: 400% 400%;
            animation: grad 10s infinite;
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        @keyframes grad {
            0% {
                background-position: 0% 50%
            }

            50% {
                background-position: 100% 50%
            }

            100% {
                background-position: 0% 50%
            }
        }

        .container {
            width: 350px;
            padding: 25px;
            border-radius: 20px;
            background: rgba(255, 255, 255, 0.2);
            backdrop-filter: blur(15px);
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.2);
            text-align: center;
            color: white;
        }

        .tabs {
            display: flex;
            gap: 5px;
            margin-bottom: 15px;
        }

        .tab {
            flex: 1;
            padding: 10px;
            border-radius: 10px;
            cursor: pointer;
            font-weight: bold;
            background: rgba(255, 255, 255, 0.1);
            transition: 0.3s;
        }

        .tab.active {
            background: linear-gradient(90deg, #ff6ec4, #7873f5);
            box-shadow: 0 0 15px #fff;
        }

        input {
            width: 90%;
            padding: 10px;
            margin: 10px 0;
            border-radius: 10px;
            border: none;
            outline: none;
            text-align: center;
            background: rgba(255, 255, 255, 0.2);
            color: white;
        }

        button {
            padding: 10px 20px;
            border: none;
            border-radius: 10px;
            cursor: pointer;
            font-weight: bold;
            margin: 5px;
            transition: 0.3s;
            color: white;
        }

        .verify {
            background: #ff6ec4;
            box-shadow: 0 5px 15px #ff6ec466;
        }

        .refresh {
            background: #4ADEDE;
            box-shadow: 0 5px 15px #4adedeb3;
        }

        #numberBox,
        #otpBox {
            font-weight: bold;
            margin-top: 15px;
            font-size: 18px;
        }

        #numberBox {
            color: #f9d423;
        }

        #otpBox {
            color: #4ADEDE;
            display: none;
        }

        .loader {
            display: none;
            margin-top: 10px;
        }

        .loader span {
            display: inline-block;
            width: 8px;
            height: 8px;
            background: white;
            border-radius: 50%;
            margin: 0 2px;
            animation: b 0.6s infinite alternate;
        }

        @keyframes b {
            to {
                transform: translateY(-10px);
            }
        }
    </style>
</head>

<body>
    <div class="container">
        <h3>💎 Verification Demo</h3>
        <div class="tabs">
            <div class="tab active" onclick="switchApp('gmail', this)">Gmail</div>
            <div class="tab" onclick="switchApp('telegram', this)">Telegram</div>
            <div class="tab" onclick="switchApp('whatsapp', this)">WhatsApp</div>
        </div>
        <input type="password" id="code" placeholder="Enter Security Code">
        <button class="verify" onclick="verifyCode()">Verify</button>
        <button class="refresh" onclick="genNum()">Refresh</button>
        <div id="numberBox"></div>
        <div class="loader" id="ldr"><span></span><span></span><span></span>
            <div>Sending OTP...</div>
        </div>
        <div id="otpBox"></div>
    </div>

    <script>
        let app = "gmail";
        const codes = { gmail: "38383", telegram: "394932", whatsapp: "33883" };
        const d = (id) => document.getElementById(id);

        function switchApp(a, el) {
            app = a;
            document.querySelectorAll('.tab').forEach(t => t.classList.remove('active'));
            el.classList.add('active');
            d("numberBox").innerText = d("otpBox").style.display = d("ldr").style.display = "";
            d("code").value = "";
        }

        function genNum() {
            d("numberBox").innerText = "📱 Number: 01" + Math.floor(100000000 + Math.random()*900000000);
            d("otpBox").style.display = "none";
        }

        function verifyCode() {
            if(d("code").value === codes[app]) {
                d("ldr").style.display = "block";
                d("otpBox").style.display = "none";
                setTimeout(() => {
                    d("ldr").style.display = "none";
                    d("otpBox").style.display = "block";
                    d("otpBox").innerText = "🎉 OTP: " + Math.floor(1000 + Math.random()*9000);
                    genNum();
                    }, 1200);
                    } else alert("❌ Wrong Code");
                    }
                    genNum();
                    </script>
                   
    <div id="admin" class="container">
        <h1>এডমিন কন্টাক্ট</h1>
        <div class="list-item" style="text-align: center;">
            <p>টেলিগ্রাম আইডি: <b>@mhlahab11</b></p>
            <p>একাউন্ট করার জন্য আপনাকে সরাসরি এডমিনের সাথে কন্টাক করতে হবে।</p>
            <a href="https://t.me/mhlahab11" style="color: #00d4ff; text-decoration: none;">[ মেসেজ দিন ]</a>
        </div>
    </div>
    
    <div id="payment" class="container">
        <h1>পেমেন্ট মেথড</h1>
        <p>বিকাশ, নগদ এবং রকেটের মাধ্যমে দ্রুত পেমেন্ট দেওয়া হয়।</p>
    </div>
    
    <div id="login" class="container">
        <h1>Login Area</h1>
        <input type="text" id="username" placeholder="ইউজার নেম">
        <input type="password" id="password" placeholder="পাসওয়ার্ড">
        <input type="text" id="security" placeholder="সিকিউরিটি কোড">
        <br>
        <button class="login-btn" onclick="checkLogin()">LOGIN</button>
        <p id="msg" style="color: red; margin-top: 10px;"></p>
    </div>
    
    <script>
        // Page Navigation
        function showPage(pageId) {
            let sections = document.querySelectorAll('.container');
            sections.forEach(section => section.classList.remove('active'));
            document.getElementById(pageId).classList.add('active');
        }
    
        // Login Logic
        function checkLogin() {
            const user = document.getElementById('username').value;
            const pass = document.getElementById('password').value;
            const sec = document.getElementById('security').value;
            const msg = document.getElementById('msg');
    
            if(user === "lahab49" && pass === "lahab11" && sec === "52152311") {
                alert("লগইন সফল হয়েছে!");
                msg.style.color = "lime";
                msg.innerText = "স্বাগতম, lahab49!";
            } else {
                msg.style.color = "red";
                msg.innerText = "ভুল ইউজারনেম, পাসওয়ার্ড বা কোড দিয়েছেন!";
            }
        }
    </script>
    
    </body>
    
    </html>
