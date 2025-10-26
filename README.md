<!DOCTYPE html>
<html lang="bn">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Lifetime Income | সাগতম</title>
  <style>
    :root {
      --primary: #ff4757;
      --secondary: #3742fa;
      --bg: #0f172a;
      --card: #1e293b;
      --text: #e2e8f0;
      --muted: #94a3b8;
      font-family: "Noto Sans Bengali", system-ui, sans-serif;
    }
    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: linear-gradient(180deg, #0f172a, #1e293b);
      color: var(--text);
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 30px 10px;
    }

    header {
      text-align: center;
      margin-bottom: 25px;
    }

    header h1 {
      font-size: 32px;
      color: var(--primary);
      letter-spacing: 1px;
      margin-bottom: 8px;
    }

    header h2 {
      font-size: 20px;
      color: var(--secondary);
      font-weight: 600;
    }

    .login-box {
      background: var(--card);
      padding: 20px;
      border-radius: 14px;
      width: 100%;
      max-width: 400px;
      box-shadow: 0 8px 25px rgba(0,0,0,0.5);
      margin-bottom: 30px;
    }

    .login-box label {
      display: block;
      margin-bottom: 6px;
      font-weight: 600;
    }

    .login-box input {
      width: 100%;
      padding: 10px 12px;
      margin-bottom: 14px;
      border-radius: 8px;
      border: none;
      background: #334155;
      color: var(--text);
      font-size: 15px;
      outline: none;
    }

    .login-box button {
      width: 100%;
      padding: 12px;
      background: linear-gradient(90deg, var(--primary), var(--secondary));
      border: none;
      border-radius: 10px;
      color: white;
      font-size: 16px;
      font-weight: 600;
      cursor: pointer;
      transition: 0.3s;
    }

    .login-box button:hover {
      transform: scale(1.03);
    }

    .section {
      width: 100%;
      max-width: 600px;
      background: var(--card);
      padding: 25px;
      border-radius: 14px;
      margin-bottom: 25px;
      box-shadow: 0 4px 20px rgba(0,0,0,0.4);
    }

    .section h3 {
      color: var(--primary);
      margin-bottom: 12px;
      text-align: center;
      font-size: 20px;
    }

    ul {
      list-style: none;
      padding-left: 0;
    }

    ul li {
      background: rgba(255,255,255,0.05);
      padding: 10px 12px;
      border-radius: 8px;
      margin-bottom: 8px;
      font-size: 15px;
      color: var(--text);
      transition: 0.3s;
    }

    ul li:hover {
      background: rgba(255,255,255,0.1);
      transform: translateX(4px);
    }

    footer {
      text-align: center;
      color: var(--muted);
      font-size: 13px;
      margin-top: 20px;
      line-height: 1.5;
    }

    @media (max-width: 480px) {
      header h1 { font-size: 26px; }
      .section { padding: 18px; }
    }
  </style>
</head>
<body>

  <header>
    <h1>🌟 Lifetime Income</h1>
    <h2>সাগতম জানাই আপনাকে</h2>
  </header>

  <div class="login-box">
    <label for="account">Account</label>
    <input type="text" id="account" placeholder="আপনার একাউন্ট নাম দিন">

    <label for="password">Password</label>
    <input type="password" id="password" placeholder="আপনার পাসওয়ার্ড দিন">

    <button type="button">Login</button>
  </div>

  <div class="section">
    <h3>💼 আমাদের কাজসমূহ</h3>
    <ul>
      <li>Telegram Account Creating</li>
      <li>WhatsApp Account Creating</li>
      <li>Gmail Account Creating</li>
      <li>Refer System</li>
      <li>Daily Task (Like, Follow, Subscribe)</li>
    </ul>
  </div>

  <div class="section">
    <h3>💰 পেমেন্ট সিস্টেম</h3>
    <ul>
      <li>বিকাশ</li>
      <li>নগদ</li>
      <li>রকেট</li>
      <li>৬৭০ টাকা হলে Withdraw করতে পারবেন</li>
    </ul>
  </div>

  <div class="section">
    <h3>ℹ️ About</h3>
    <p style="text-align:center; line-height:1.6; color:var(--muted);">
      দেশের যেকোনো জায়গা থেকে কাজ করতে পারবেন।<br>
      একাউন্ট তৈরি করার জন্য এডমিনের সাথে যোগাযোগ করুন।
    </p>
  </div>

  <footer>
