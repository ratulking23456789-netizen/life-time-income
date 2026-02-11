
<!doctype html>
<html lang="bn">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Ariyan Income — Account Demo</title>
  <style>
    :root{
      --primary:#007bff;
      --accent:#28a745;
      --bg:#f3f6fb;
      --card:#fff;
      --muted:#666;
      font-family: "Noto Sans Bengali", Arial, sans-serif;
    }
    body{margin:0;background:var(--bg);display:flex;align-items:center;justify-content:center;min-height:100vh;padding:18px;color:#222;}
    .app{width:100%;max-width:480px;background:var(--card);border-radius:12px;box-shadow:0 8px 30px rgba(10,20,40,0.08);overflow:hidden;}
    header{padding:14px 18px;border-bottom:1px solid #eef2f7;display:flex;align-items:center;gap:12px;background:linear-gradient(90deg,var(--primary),#0062d8);color:#fff}
    header h1{font-size:18px;margin:0}
    .content{padding:18px}
    .row{display:flex;gap:12px;flex-wrap:wrap}
    label{display:block;font-size:13px;margin-bottom:6px;font-weight:600}
    input, select, button{box-sizing:border-box}
    input[type="text"], input[type="password"], input[type="number"], select{
      width:100%;padding:10px;border-radius:8px;border:1px solid #e3e7ee;font-size:14px;background:#fff;
    }
    .card{background:var(--bg);padding:14px;border-radius:10px;margin-bottom:12px;border:1px solid #e9eef6}
    .btn{display:inline-block;padding:10px 14px;border-radius:8px;border:none;cursor:pointer;font-weight:700}
    .btn-primary{background:var(--primary);color:#fff}
    .btn-ghost{background:#fff;border:1px solid #dfe8f8;color:var(--primary)}
    .muted{color:var(--muted);font-size:13px}
    .center{text-align:center}
    .small{font-size:13px;color:var(--muted)}
    .nav{display:flex;gap:8px;margin-bottom:12px}
    .nav button{flex:1}
    .notice{padding:10px;border-radius:8px;background:#fff6f6;color:#9b2b2b;border:1px solid #ffd6d6;margin-top:8px}
    .success{padding:10px;border-radius:8px;background:#f3fffa;color:#087f46;border:1px solid #c9f4de;margin-top:8px}
    .profile{display:flex;align-items:center;gap:12px}
    .avatar{width:56px;height:56px;border-radius:50%;background:#e9eef6;display:inline-block}
    .actions{display:flex;gap:8px;margin-top:10px;flex-wrap:wrap}
    .tiny{font-size:12px;color:var(--muted)}
    .danger{background:#ff4d4f;color:#fff}
    footer{padding:10px 18px;border-top:1px solid #eef2f7;font-size:13px;color:var(--muted);text-align:center}
  </style>
</head>
<body>
  <div class="app" role="application" aria-label="Earning App with Signup">
    <header>
      <img src="https://via.placeholder.com/44" alt="logo" style="width:44px;height:44px;border-radius:8px;object-fit:cover">
      <div>
        <h1 id="app-name">Ariyan Income BD</h1>
        <div style="font-size:12px;opacity:0.9">পেমোড সাম্পল অ্যাপ — লোকাল একাউন্ট সিস্টেম</div>
      </div>
    </header>

    <div class="content">
      <div class="nav">
        <button id="tab-login" class="btn btn-ghost">Login</button>
        <button id="tab-signup" class="btn btn-ghost">Sign Up</button>
        <button id="tab-dashboard" class="btn btn-ghost">Dashboard</button>
      </div>

      <!-- LOGIN -->
      <div id="panel-login" class="panel">
        <div class="card">
          <h3 style="margin:0 0 8px 0">লগইন</h3>
          <div class="small">তৈরি করা ইউজারনেম ও পাসওয়ার্ড দিয়ে লগইন করো</div>
          <div style="margin-top:12px">
            <label for="login-username">ইউজারনেম</label>
            <input id="login-username" type="text" placeholder="username" />
          </div>
          <div style="margin-top:8px">
            <label for="login-password">পাসওয়ার্ড</label>
            <input id="login-password" type="password" placeholder="password" />
          </div>
          <div class="actions">
            <button id="btn-login" class="btn btn-primary">লগইন</button>
            <button id="btn-clear-login" class="btn">মুছো</button>
          </div>
          <div id="login-msg" class="small" style="margin-top:8px"></div>
        </div>
      </div>

      <!-- SIGN UP -->
      <div id="panel-signup" class="panel" style="display:none">
        <div class="card">
          <h3 style="margin:0 0 8px 0">নতুন একাউন্ট তৈরি</h3>
          <div class="small">নিচে নাম, ইউজারনেম ও পাসওয়ার্ড পূরণ করে 'Create Account' চাপো</div>

          <div style="margin-top:12px">
            <label for="su-name">নাম</label>
            <input id="su-name" type="text" placeholder="আপনার নাম" />
          </div>
          <div style="margin-top:8px">
            <label for="su-username">ইউজারনেম</label>
            <input id="su-username" type="text" placeholder="username ( অনন্য )" />
          </div>
          <div style="margin-top:8px">
            <label for="su-password">পাসওয়ার্ড</label>
            <input id="su-password" type="password" placeholder="password" />
          </div>
          <div style="margin-top:8px">
            <label for="su-confirm">পাসওয়ার্ড নিশ্চিত করো</label>
            <input id="su-confirm" type="password" placeholder="confirm password" />
          </div>

          <div class="actions">
            <button id="btn-signup" class="btn btn-primary">Create Account</button>
            <button id="btn-clear-signup" class="btn">Clear</button>
          </div>
          <div id="signup-msg" class="small" style="margin-top:8px"></div>
        </div>
      </div>

      <!-- DASHBOARD (shows when logged in) -->
      <div id="panel-dashboard" class="panel" style="display:none">
        <div class="card">
          <div style="display:flex;justify-content:space-between;align-items:center">
            <div class="profile">
              <div class="avatar" id="dash-avatar"></div>
              <div>
                <div id="dash-name" style="font-weight:700">User</div>
                <div id="dash-username" class="tiny">@username</div>
              </div>
            </div>
            <div style="text-align:right">
              <div class="small">Current Balance</div>
              <div id="dash-balance" style="font-weight:800;color:var(--accent)">BDT 0.00</div>
            </div>
          </div>

          <div class="actions" style="margin-top:12px">
            <button id="btn-logout" class="btn">Logout</button>
            <button id="btn-delete-account" class="btn danger">Delete Account</button>
          </div>

          <div style="margin-top:12px" class="small">নোট: এই ডেমো-অ্যাপে একাউন্ট ডাটা লোকালি ব্রাউজারের localStorage-এ থাকে। সার্ভার লাগবে বাস্তব ব্যবহারের জন্য।</div>
          <div id="dash-msg" style="margin-top:8px"></div>
        </div>
      </div>

    </div>

    <footer>
      পেমেন্ট রিকুয়েস্ট করতে অ্যাকাউন্টে অন্তত: <strong>৳670</strong> থাকতে হবে — (ডেমো নির্দেশিকা)
    </footer>
  </div>

  <script>
    // Simple local account system (DEMO)
    // Data structure in localStorage: "ai_users" -> JSON array of users
    // each user: { name, username, passwordB64, balance }
    // current logged in: "ai_current_user" -> username

    function $(id){ return document.getElementById(id); }

    // init
    if (!localStorage.getItem('ai_users')) {
      localStorage.setItem('ai_users', JSON.stringify([]));
    }

    // tabs
    const tabLogin = $('tab-login'), tabSignup = $('tab-signup'), tabDashboard = $('tab-dashboard');
    const panelLogin = $('panel-login'), panelSignup = $('panel-signup'), panelDashboard = $('panel-dashboard');

    function showPanel(panel){
      panelLogin.style.display = 'none';
      panelSignup.style.display = 'none';
      panelDashboard.style.display = 'none';
      panel.style.display = 'block';
    }

    tabLogin.addEventListener('click', ()=> showPanel(panelLogin));
    tabSignup.addEventListener('click', ()=> showPanel(panelSignup));
    tabDashboard.addEventListener('click', ()=> {
      const current = localStorage.getItem('ai_current_user');
      if (current) { loadDashboard(current); showPanel(panelDashboard); }
      else { showPanel(panelLogin); alert('প্রথমে লগইন করুন।'); }
    });

    // Signup
    $('btn-signup').addEventListener('click', ()=> {
      const name = $('su-name').value.trim();
      const username = $('su-username').value.trim();
      const pw = $('su-password').value;
      const pwc = $('su-confirm').value;
      const msg = $('signup-msg');

      msg.textContent = '';
      if(!name || !username || !pw || !pwc){ msg.textContent = 'সব ফিল্ড পূরণ করো।'; return; }
      if(pw !== pwc){ msg.textContent = 'পাসওয়ার্ড মিলছে না।'; return; }
      if(username.length < 3){ msg.textContent = 'ইউজারনেম কমপক্ষে 3 অক্ষর হওয়া উচিত।'; return; }

      let users = JSON.parse(localStorage.getItem('ai_users'));
      if (users.find(u => u.username.toLowerCase() === username.toLowerCase())) {
        msg.textContent = 'এই ইউজারনেম ইতিমধ্যে নেওয়া আছে।';
        return;
      }

      const pwB64 = btoa(pw); // simple encoding for demo (NOT secure for production)
      const newUser = { name, username, passwordB64: pwB64, balance: 0.00, created: new Date().toISOString() };
      users.push(newUser);
      localStorage.setItem('ai_users', JSON.stringify(users));

      msg.innerHTML = '<span style="color:green">একাউন্ট সফলভাবে তৈরি হয়েছে! এখন লগইন করো।</span>';
      // auto-clear fields
      $('su-name').value=''; $('su-username').value=''; $('su-password').value=''; $('su-confirm').value='';
      // switch to login
      showPanel(panelLogin);
    });

    $('btn-clear-signup').addEventListener('click', ()=> {
      $('su-name').value=''; $('su-username').value=''; $('su-password').value=''; $('su-confirm').value='';
      $('signup-msg').textContent = '';
    });

    // Login
    $('btn-login').addEventListener('click', ()=> {
      const username = $('login-username').value.trim();
      const pw = $('login-password').value;
      const msg = $('login-msg');
      msg.textContent = '';

      if(!username || !pw){ msg.textContent = 'ইউজারনেম ও পাসওয়ার্ড দিন।'; return; }

      const users = JSON.parse(localStorage.getItem('ai_users'));
      const user = users.find(u => u.username.toLowerCase() === username.toLowerCase());
      if (!user) { msg.textContent = 'ইউজারনেম পাওয়া যায়নি।'; return; }

      if (user.passwordB64 !== btoa(pw)) { msg.textContent = 'পাসওয়ার্ড ভুল।'; return; }

      // success
      localStorage.setItem('ai_current_user', user.username);
      msg.innerHTML = '<span style="color:green">সফলভাবে লগইন করা হয়েছে।</span>';
      loadDashboard(user.username);
      showPanel(panelDashboard);
      // clear login fields
      $('login-username').value=''; $('login-password').value='';
    });

    $('btn-clear-login').addEventListener('click', ()=> {
      $('login-username').value=''; $('login-password').value=''; $('login-msg').textContent='';
    });

    // Dashboard load
    function loadDashboard(username){
      const users = JSON.parse(localStorage.getItem('ai_users'));
      const user = users.find(u => u.username === username);
      if (!user) { alert('ইউজার পাওয়া যায়নি।'); return; }

      $('dash-name').textContent = user.name;
      $('dash-username').textContent = '@' + user.username;
      $('dash-balance').textContent = 'BDT ' + Number(user.balance).toFixed(2);
      // avatar can be initial letter
      const avatar = $('dash-avatar');
      avatar.textContent = user.name ? user.name.trim()[0].toUpperCase() : user.username[0].toUpperCase();
      avatar.style.display = 'flex';
      avatar.style.alignItems = 'center';
      avatar.style.justifyContent = 'center';
      avatar.style.fontWeight = '700';
      avatar.style.color = '#134a8a';
      avatar.style.background = '#e6f0ff';
      $('dash-msg').textContent = '';
    }

    // Logout
    $('btn-logout').addEventListener('click', ()=> {
      localStorage.removeItem('ai_current_user');
      $('dash-msg').textContent = 'আপনি লগআউট হয়েছে।';
      showPanel(panelLogin);
    });

    // Delete account
    $('btn-delete-account').addEventListener('click', ()=> {
      const current = localStorage.getItem('ai_current_user');
      if(!current){ alert('প্রথমে লগইন করুন।'); return; }
      if(!confirm('আপনি কি একাউন্ট মুছে ফেলতে চাচ্ছেন? এই অপারেশন ফিরিয়ে আনা যাবে না।')) return;

      let users = JSON.parse(localStorage.getItem('ai_users'));
      users = users.filter(u => u.username !== current);
      localStorage.setItem('ai_users', JSON.stringify(users));
      localStorage.removeItem('ai_current_user');

      alert('একাউন্ট মুছে দেয়া হয়েছে।');
      showPanel(panelSignup);
    });

    // On load: if already logged in, go to dashboard
    document.addEventListener('DOMContentLoaded', ()=> {
      const cur = localStorage.getItem('ai_current_user');
      if(cur){ loadDashboard(cur); showPanel(panelDashboard); }
      else showPanel(panelLogin);
    });

    // Extra: allow changing app name easily (if user wants another name)
    // Use console command: setAppName("Your App Name");
    function setAppName(name){
      if(name && name.trim()) document.getElementById('app-name').textContent = name.trim();
    }
    window.setAppName = setAppName;
  </script>
</body>
</html>

