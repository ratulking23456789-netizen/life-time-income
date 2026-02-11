<!DOCTYPE html>
<html lang="bn">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Online BD - Official</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', sans-serif;
        }

        body {
            min-height: 100vh;
            background: linear-gradient(-45deg, #1e3c72, #2a5298, #ff512f, #dd2476);
            background-size: 400% 400%;
            animation: gradient 10s ease infinite;
            color: white;
        }

        @keyframes gradient {
            0% {
                background-position: 0% 50%;
            }

            50% {
                background-position: 100% 50%;
            }

            100% {
                background-position: 0% 50%;
            }
        }

        nav {
            text-align: center;
            padding: 20px;
        }

        nav button {
            padding: 10px 20px;
            margin: 5px;
            border: none;
            border-radius: 25px;
            cursor: pointer;
            font-weight: bold;
        }

        .section {
            display: none;
            padding: 40px 20px;
            text-align: center;
        }

        .active {
            display: block;
        }

        .card {
            max-width: 500px;
            margin: auto;
            background: rgba(0, 0, 0, 0.65);
            padding: 30px;
            border-radius: 20px;
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.5);
        }

        input {
            width: 100%;
            padding: 12px;
            margin: 10px 0;
            border: none;
            border-radius: 8px;
        }

        .btn {
            width: 100%;
            padding: 12px;
            border: none;
            border-radius: 8px;
            background: #00e6ac;
            font-weight: bold;
            cursor: pointer;
        }

        .btn:hover {
            background: #00b386;
        }

        #error {
            color: #ff4d4d;
        }
    </style>
</head>

<body>

    <nav>
        <button onclick="showSection('home')">হোম</button>
        <button onclick="showSection('work')">কাজ</button>
        <button onclick="showSection('register')">একাউন্ট খুলুন</button>
        <button onclick="showSection('payment')">পেমেন্ট</button>
        <button onclick="showSection('login')">লগিন</button>
    </nav>

    <div id="home" class="section active">
        <h1>Online BD একটি বিশ্বস্ত অনলাইন আয়ের প্ল্যাটফর্ম, যেখানে আপনি ঘরে বসে বিভিন্ন সহজ কাজ করে উপার্জন করতে পারবেন।
        আমাদের মূল লক্ষ্য হলো তরুণ প্রজন্মকে অনলাইন জগতে দক্ষ করে তোলা এবং তাদের আর্থিকভাবে স্বাবলম্বী করে তোলা।
        
        💼 আমাদের কাজসমূহ:
        
        💰 রেফার ইনকাম: আপনার লিংক শেয়ার করে অন্যকে রেফার করুন, আর প্রতিটি রেফারে আয় করুন।
        
        🎥 ভিডিও দেখে আয়: সহজভাবে ভিডিও দেখে পয়েন্ট বা টাকা উপার্জন করুন।
        
        ✉️ জিমেল মার্কেটিং: ইমেইল মার্কেটিংয়ের মাধ্যমে ইনকামের সুযোগ নিন।
        
        💬 Telegram অ্যাকাউন্ট তৈরি: নির্দিষ্ট কাজ অনুযায়ী টেলিগ্রাম অ্যাকাউন্ট খুলে আয় করুন।
        
        📱 WhatsApp অ্যাকাউন্ট তৈরি: হোয়াটসঅ্যাপ অ্যাকাউন্ট তৈরি করেও আয় করা সম্ভব।
        
        ⌨️ Typing Job: টাইপিংয়ের মাধ্যমে সহজে ইনকাম করুন – এটি নতুনদের জন্য একদম পারফেক্ট কাজ।
        
        
        🌟 আমাদের লক্ষ্য:
        
        প্রত্যেক ব্যবহারকারীকে অনলাইন ইনকামের মাধ্যমে দক্ষ, আত্মনির্ভরশীল ও সফল করে তোলা।</h1>
    </div>

    <div id="work" class="section">
        <div class="card">
            <h2>💼 আমাদের কাজসমূহ</h2><br>
        💰 রেফার ইনকাম <br><br>
        🎥 ভিডিও দেখে আয় <br><br>
        ✉️ জিমেল মার্কেটিং <br><br>
        💬 Telegram কাজ <br><br>
        📱 WhatsApp কাজ <br><br>
        ⌨️ Typing Job
        </div>
    </div>

    <div id="register" class="section">
        <div class="card">
            <h2>📌 একাউন্ট খোলার নিয়ম</h2><br>
        এডমিন কন্টাক আইডি: <b>@mhlahab11</b><br><br>
        একাউন্ট খোলার ফি: <b>২০০ টাকা</b><br><br>
        কোম্পানি ১০০ টাকা সার্ভিস চার্জ কেটে নিবে এবং ১০০ টাকা আপনার একাউন্টে যোগ করবে।
        </div>
    </div>

    <div id="payment" class="section">
        <div class="card">
            <h2>💳 পেমেন্ট সিস্টেম</h2><br>
        💰 একাউন্ট খোলার ফি: <b>২০০ টাকা</b><br><br>

        📱 <b>বিকাশ (Send Money)</b><br>
        নম্বর: <b>01XXXXXXXXX</b><br><br>

        📱 <b>নগদ (Send Money)</b><br>
        নম্বর: <b>01XXXXXXXXX</b><br><br>

        🔔 পেমেন্ট করার পর ট্রানজেকশন আইডি বা স্ক্রিনশট এডমিন
            <b>@mhlahab11</b> এ পাঠাতে হবে।
        </div>
    </div>

    <div id="login" class="section">
        <div class="card">
            <h2>🔐 লগিন করুন</h2>
            <input type="text" id="username" placeholder="ইউজার নেম">
            <input type="password" id="password" placeholder="পাসওয়ার্ড">
            <input type="text" id="code" placeholder="সিকিউরিটি কোড">
            <button class="btn" onclick="login()">লগিন</button>
            <p id="error"></p>
        </div>
    </div>

    <div id="dashboard" class="section">
        <div class="card">
            <h2>Welcome to Online BD</h2><br>
        🎉 সফলভাবে লগিন হয়েছে!
        </div>
    </div>

    <script>
        function showSection(id){
    document.querySelectorAll('.section').forEach(sec=>{
        sec.classList.remove('active');
    });
    document.getElementById(id).classList.add('active');
}

function login(){
    var user=document.getElementById("username").value;
    var pass=document.getElementById("password").value;
    var code=document.getElementById("code").value;

    if(user==="admin111" && pass==="12345111" && code==="1234111"){
        showSection("dashboard");
        document.getElementById("error").innerText="";
    }else{
        document.getElementById("error").innerText="❌ ভুল তথ্য! লগিন হবে না।";
    }
}
    </script>

</body>

</html>
