<LIFE TIME>
<html lang="bn">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>LIFETIME | Home</title>
  <style>
    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background-color: #fff;
      color: #333;
    }
    header {
      background-color: #e60000;
      color: white;
      text-align: center;
      padding: 40px 10px;
      font-size: 28px;
      font-weight: bold;
      text-transform: uppercase;
      letter-spacing: 2px;
    }
    nav {
      background-color: #b30000;
      text-align: center;
      padding: 10px 0;
    }
    nav a {
      color: white;
      text-decoration: none;
      margin: 0 15px;
      font-weight: 500;
      transition: color 0.3s;
    }
    nav a:hover {
      color: #ffd700;
    }
    .hero {
      text-align: center;
      padding: 80px 20px;
      background: linear-gradient(to right, #ff4d4d, #e60000);
      color: white;
    }
    .hero h1 {
      font-size: 48px;
      margin-bottom: 10px;
    }
    .hero p {
      font-size: 20px;
    }
    .section {
      padding: 60px 20px;
      text-align: center;
    }
    .section h2 {
      color: #e60000;
      margin-bottom: 20px;
      font-size: 32px;
    }
    .section p {
      max-width: 700px;
      margin: auto;
      font-size: 18px;
      line-height: 1.6;
    }

    /* সুবিধাসমূহ Section */
    .benefits {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 25px;
      margin-top: 40px;
    }
    .benefit-box {
      background: #fff5f5;
      border: 2px solid #e60000;
      border-radius: 10px;
      width: 280px;
      padding: 25px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      transition: transform 0.3s;
    }
    .benefit-box:hover {
      transform: scale(1.05);
    }
    .benefit-box h3 {
      color: #b30000;
      margin-bottom: 10px;
      font-size: 20px;
    }
    .benefit-box p {
      font-size: 16px;
      line-height: 1.5;
      color: #333;
    }

    footer {
      background-color: #b30000;
      color: white;
      text-align: center;
      padding: 15px 0;
      font-size: 16px;
    }
  </style>
</head>
<body>

  <header>
    WELLCOME
  </header>

  <nav>
    <a href="#">হোম</a>
    <a href="#">আমাদের সম্পর্কে</a>
    <a href="#">কাজ শুরু করুন</a>
    <a href="#">যোগাযোগ</a>
  </nav>

  <div class="hero">
    <h1>অনলাইন ইনকাম শুরু করুন আজই!</h1>
    <p>বাসা থেকে কাজ করে প্রতিদিন ইনকাম করুন নিজের মতো করে 💻</p>
  </div>

  <div class="section">
    <h2>আমাদের সার্ভিস</h2>
    <p>
      আমরা আপনাকে শেখাবো কিভাবে অনলাইনে আয় করা যায় — ফ্রিল্যান্সিং, ইউটিউব, অ্যাফিলিয়েট মার্কেটিং, 
      ব্লগিং, ও আরও অনেক কিছু! প্রতিদিন নতুন নতুন টিপস ও সুযোগ সম্পর্কে জানতে আমাদের ওয়েবসাইট ভিজিট করুন।
    </p>
  </div>

  <div class="section">
    <h2>আমাদের সুবিধাসমূহ</h2>

    <div class="benefits">
      <div class="benefit-box">
        <h3>💰 Weekly Withdraw</h3>
        <p>প্রতি সপ্তাহে টাকা তুলুন বিকাশ বা নগদে!</p>
      </div>

      <div class="benefit-box">
        <h3>👥 Referral Bonus</h3>
        <p>বন্ধুকে ইনভাইট করলে বাড়তি ইনকাম পান!</p>
      </div>

      <div class="benefit-box">
        <h3>✅ Monthly Reward</h3>
        <p>মাসে চারবার বোনাস ইনকাম যোগ হবে!</p>
      </div>
    </div>
  </div>

  <div class="section">
    <h2>কেন আমাদের সাথে কাজ করবেন?</h2>
    <p>
      ✅ সহজ ট্রেনিং<br>
      ✅ রিয়েল পেমেন্ট সিস্টেম<br>
      ✅ ২৪/৭ সাপোর্ট<br>
      ✅ বাংলাদেশি ইউজারদের জন্য উপযোগী সিস্টেম

    
    </p>
  </div>

  <footer>
     LIFE TIME | Developed bY BK HUNTER
  </footer>

</body>
</html>
                       <label for="account">Account</label>
                           <input id="account" name="account" type="text" placeholder="আপনার অ্যাকাউন্ট নাম/ইমেইল" autocomplete="username">
        

                     <div class="field">
                     <label for="password">Password</label>
               <div class="pw-row">
                    <input id="password" name="password" type="password" placeholder="আপনার পাসওয়ার্ড" autocomplete="current-password" style="flex:1;">
                    <button type="button" class="pw-toggle" id="togglePw" aria-pressed="false">Show</button>

        <button id="submitBtn" class="btn" type="submit">Submit</button>

  <script>
    // small JS: basic validation + show/hide password
    const form = document.getElementById('loginForm');
    const account = document.getElementById('account');
    const password = document.getElementById('password');
    const errorBox = document.getElementById('error');
    const submitBtn = document.getElementById('submitBtn');
    const toggle = document.getElementById('togglePw');

    toggle.addEventListener('click', () => {
      const isHidden = password.type === 'password';
      password.type = isHidden ? 'text' : 'password';
      toggle.textContent = isHidden ? 'Hide' : 'Show';
      toggle.setAttribute('aria-pressed', isHidden ? 'true' : 'false');
    });

    submitBtn.addEventListener('click', () => {
      errorBox.style.display = 'none';
      const a = account.value.trim();
      const p = password.value;

      if (!a || !p) {
        errorBox.textContent = 'দয়া করে Account এবং Password দুটোই পূরণ করুন।';
        errorBox.style.display = 'block';
        return;
      }

      // ---- এখানে সার্ভারে পাঠানোর জায়গা ----
      // উদাহরণ: fetch('/login', {method:'POST', body: JSON.stringify({account:a,password:p})})
      // কিন্তু এখন শুধু ডেমো: সফল হলে নিচের মেসেজ দেখাবে

      submitBtn.disabled = true;
      submitBtn.textContent = 'Signing in...';

      // ডেমো সিমুলেশন (1 সেকেন্ড)
      setTimeout(() => {
        submitBtn.disabled = false;
        submitBtn.textContent = 'Submit';
        alert('Login successful (ডেমো)। সার্ভার সাইড যাচাই করার জন্য আপনার কোড/এন্ডপয়েন্ট সংযুক্ত করুন।');
        // form.reset(); // চাইলে আনকমেন্ট করে ফর্ম ক্লিয়ার করো
      }, 1000);
    });

    // Enter key submission
    
