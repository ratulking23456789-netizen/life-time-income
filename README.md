<!DOCTYPE html>
<html lang="bn">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wellcome Online BD - ইন্টারফেস</title>
    <style>
        /* বেসিক CSS স্টাইলিং - সহজে মোবাইলে দেখার জন্য */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f9;
            color: #333;
        }
        .container {
            max-width: 600px;
            margin: 20px auto;
            background-color: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        .menu-item {
            background-color: #007bff;
            color: white;
            padding: 15px;
            margin-bottom: 10px;
            border-radius: 5px;
            cursor: pointer;
            font-size: 1.1em;
            font-weight: bold;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .menu-content {
            padding: 15px;
            border: 1px solid #ddd;
            border-radius: 5px;
            margin-bottom: 15px;
            background-color: #f9f9f9;
            display: none; /* ডিফল্টভাবে লুকিয়ে থাকবে */
        }
        .menu-content.active {
            display: block; /* ক্লিক করলে দেখাবে */
        }
        h2, h3 {
            color: #0056b3;
            border-bottom: 2px solid #eee;
            padding-bottom: 5px;
            margin-top: 0;
        }
        /* লগইন স্টাইল */
        .login-form input[type="text"],
        .login-form input[type="password"] {
            width: 95%;
            padding: 10px;
            margin-bottom: 10px;
            border: 1px solid #ccc;
            border-radius: 4px;
        }
        .login-form button {
            background-color: #28a745;
            color: white;
            padding: 10px 15px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            width: 100%;
            font-size: 1.1em;
        }
        .login-form button:hover {
            background-color: #218838;
        }
        /* পেমেন্ট ও অন্যান্য তথ্য স্টাইল */
        .payment-info strong {
            display: block;
            margin-top: 10px;
            font-size: 1.1em;
            color: #d9534f;
        }
        .contact {
            display: inline-block;
            margin-top: 15px;
            padding: 10px 15px;
            background-color: #f0ad4e;
            color: white;
            text-decoration: none;
            border-radius: 4px;
        }
        .footer {
            text-align: center;
            font-size: 0.8em;
            color: #666;
            margin-top: 20px;
        }
    </style>
</head>
<body>

<div class="container">
    <h1>Wellcome Online BD</h1>

    <div class="menu-item" data-target="loginContent">
        🔑 লগইন (Login)
    </div>
    <div class="menu-content login-form" id="loginContent">
        <h2>🔑 লগইন</h2>
        <p>Account:</p>
        <input type="text" placeholder="ইউজারনেম বা ফোন নম্বর">
        <p>Password:</p>
        <input type="password" placeholder="পাসওয়ার্ড">
        <button>Login</button>
    </div>

    <div class="menu-item" data-target="aboutContent">
        💡 About
    </div>
    <div class="menu-content" id="aboutContent">
        <h2>💡 About</h2>
        <p>
            ✅ 'Wellcome Online BD' প্ল্যাটফর্মের সুবিধা ও লাভজনক দিক
            আপনার দেওয়া ছবিটি থেকে বোঝা যাচ্ছে যে, এই প্ল্যাটফর্মটি মূলত ক্ষুদ্র বিনিয়োগে অনলাইনে আয় করার সুযোগ তৈরি করেছে। এর মূল সুবিধা ও লাভজনক দিকগুলো নিম্নরূপ:
            <br><br>
            ১. 💰 স্বল্প বিনিয়োগে আয়ের সুযোগ (Low Investment, High Potential)
            <br>
            • মাত্র ২০০ টাকায় শুরু: এটিই এই কোম্পানির সবচেয়ে বড় আকর্ষণ। মাত্র ২০০ টাকায় একটি অ্যাকাউন্ট খুলে আয়ের যাত্রা শুরু করা যায়, যা অন্য কোনো গতানুগতিক ব্যবসার ক্ষেত্রে প্রায় অসম্ভব।
            <br>
