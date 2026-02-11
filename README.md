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
        <h1>Online BD একটি বিশ্বস্ত অনলাইন আয়ের প্ল্যাটফর্ম, যেখানে আপনি ঘরে বসে বিভিন্ন সহজ কাজ করে উপার্জন করতে
            পারবেন।
            ।</h1>
    </div>

    <div id="work" class="section">
        <div class="card">
            <h2>💼 আমাদের কাজসমূহ</h2><br>
        💰<!DOCTYPE html>
        <html lang="en">
        
        <head>
            <meta charset="UTF-8">
            <meta name="viewport" content="width=device-width, initial-scale=1.0">
            <title>Full HD Demo Verification</title>
            <style>
                /* Full HD Gradient Background */
                body {
                    margin: 0;
                    font-family: 'Segoe UI', sans-serif;
                    background: linear-gradient(135deg, #ff9a9e, #fad0c4, #a1c4fd, #c2e9fb);
                    background-size: 400% 400%;
                    animation: gradientBG 15s ease infinite;
                    display: flex;
                    justify-content: center;
                    align-items: center;
                    height: 100vh;
                }
        
                @keyframes gradientBG {
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
        
                /* Container */
                .container {
                    width: 400px;
                    padding: 30px;
                    border-radius: 20px;
                    background: rgba(255, 255, 255, 0.2);
                    backdrop-filter: blur(15px);
                    box-shadow: 0 20px 50px rgba(0, 0, 0, 0.3);
                    text-align: center;
                    color: white;
                    animation: fadeIn 1s ease;
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
        
                /* Tabs */
                .tabs {
                    display: flex;
                    justify-content: space-between;
                    margin-bottom: 20px;
                }
        
                .tab {
                    flex: 1;
                    margin: 0 5px;
                    padding: 12px 0;
                    border-radius: 15px;
                    cursor: pointer;
                    font-weight: bold;
                    color: white;
                    transition: 0.3s;
                    text-shadow: 0 0 5px rgba(0, 0, 0, 0.5);
                    box-shadow: 0 0 10px rgba(255, 255, 255, 0.3);
                }
        
                .tab:hover {
                    transform: scale(1.05);
                    box-shadow: 0 0 20px rgba(255, 255, 255, 0.7);
                }
        
                .tab.active {
                    background: linear-gradient(90deg, #ff6ec4, #7873f5);
                    box-shadow: 0 0 25px #fff;
                }
        
                /* Input */
                input {
                    width: 90%;
                    padding: 12px;
                    margin: 15px 0;
                    border-radius: 12px;
                    border: 2px solid rgba(255, 255, 255, 0.5);
                    text-align: center;
                    font-size: 16px;
                    outline: none;
                    background: rgba(255, 255, 255, 0.1);
                    color: white;
                    transition: 0.3s;
                }
        
                input:focus {
                    border: 2px solid #ff6ec4;
                    box-shadow: 0 0 10px #ff6ec4;
                }
        
                /* Buttons */
                button {
                    padding: 12px 25px;
                    border: none;
                    border-radius: 12px;
                    cursor: pointer;
                    font-weight: bold;
                    margin: 5px;
                    transition: 0.3s;
                    text-shadow: 0 0 5px rgba(0, 0, 0, 0.5);
                }
        
                .verify {
                    background: #ff6ec4;
                    color: white;
                    box-shadow: 0 0 15px #ff6ec4;
                }
        
                .refresh {
                    background: #4ADEDE;
                    color: white;
                    box-shadow: 0 0 15px #4ADEDE;
                }
        
                button:hover {
                    transform: scale(1.05);
                }
        
                /* Number Box */
                #numberBox {
                    font-weight: bold;
                    font-size: 20px;
                    margin-top: 15px;
                    color: #f9d423;
                    text-shadow: 0 0 10px #fff;
                }
        
                /* OTP Box */
                #otpBox {
                    margin-top: 20px;
                    font-weight: bold;
                    font-size: 20px;
                    display: none;
                    color: #4ADEDE;
                    text-shadow: 0 0 10px #fff;
                }
        
                /* Loader Animation */
                .loader {
                    display: none;
                    margin-top: 15px;
                }
        
                .loader span {
                    display: inline-block;
                    width: 10px;
                    height: 10px;
                    background: white;
                    border-radius: 50%;
                    margin: 0 3px;
                    animation: bounce 1s infinite alternate;
                }
        
                .loader span:nth-child(2) {
                    animation-delay: 0.2s;
                }
        
                .loader span:nth-child(3) {
                    animation-delay: 0.4s;
                }
        
                @keyframes bounce {
                    from {
                        transform: translateY(0);
                    }
        
                    to {
                        transform: translateY(-15px);
                    }
                }
            </style>
        </head>
        
        <body>
        
            <div class="container">
                <h2>💎 Full HD Verification</h2>
        
                <div class="tabs">
                    <div class="tab active" onclick="switchApp('gmail')">Gmail</div>
                    <div class="tab" onclick="switchApp('telegram')">Telegram</div>
                    <div class="tab" onclick="switchApp('whatsapp')">WhatsApp</div>
                </div>
        
                <input type="password" id="code" placeholder="Enter Security Code">
                <br>
                <button class="verify" onclick="verifyCode()">Verify</button>
                <button class="refresh" onclick="generateNumber()">Refresh</button>
        
                <div id="numberBox"></div>
        
                <div class="loader" id="loader">
                    <span></span><span></span><span></span>
                    <div>Sending OTP...</div>
                </div>
        
                <div id="otpBox"></div>
            </div>
        
            <script>
                let currentApp = "gmail";
        
        const codes = {
          gmail: "38383",
          telegram: "394932",
          whatsapp: "33883"
        };
        
        function switchApp(app){
          currentApp = app;
        document.querySelectorAll('.tab').forEach(el=>el.classList.remove('active'));
        if(app==="gmail") document.querySelector(".tab:nth-child(1)").classList.add('active');
        if(app==="telegram") document.querySelector(".tab:nth-child(2)").classList.add('active');
        if(app==="whatsapp") document.querySelector(".tab:nth-child(3)").classList.add('active');
        
        document.getElementById("numberBox").innerText = "";
        document.getElementById("otpBox").style.display="none";
        document.getElementById("loader").style.display="none";
        document.getElementById("code").value="";
        }
        
        function generateNumber(){
        let number = "01" + Math.floor(100000000 + Math.random()*900000000);
        document.getElementById("numberBox").innerText = "📱 Number: " + number;
        document.getElementById("otpBox").style.display="none";
        }
        
        function verifyCode(){
        let inputCode = document.getElementById("code").value;
        if(inputCode === codes[currentApp]){
        document.getElementById("loader").style.display="block";
        document.getElementById("otpBox").style.display="none";
        
        setTimeout(()=>{
        document.getElementById("loader").style.display="none";
        document.getElementById("otpBox").style.display="block";
        let otp = Math.floor(1000 + Math.random()*9000);
        document.getElementById("otpBox").innerText = "🎉 Demo OTP: " + otp;
        generateNumber(); // Show number after correct code
        },1500);
        }else{
        alert("❌ Wrong Security Code");
        document.getElementById("numberBox").innerText = "";
        document.getElementById("otpBox").style.display="none";
        }
        }
        
        // Initialize
        generateNumber();
            </script>
        
        </body>
        
        </html> <br><br>
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
            <h2>💳 account</h2><br>
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
