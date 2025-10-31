<p style="color:var(--muted)">Login করে বাম পাশে থাকা অপশনগুলো ক্লিক করলে সংশ্লিষ্ট কন্টেন্ট এখানে দেখা যাবে।</p>
        </div>

        <div style="height:12px"></div>

        <div class="card payment-info" id="sideInfo">
          <strong>Account তৈরি ফি:</strong> ২০০ টাকা<br>
          💳 <b>Nagad Personal:</b> 01909850916<br>
          💳 <b>Bikash Personal:</b> 01630148084<br><br>
          Send Money করে Screenshot এডমিনের কাছে জমা দিন।
          <div style="margin-top:10px">
            <a class="contact" href="https://t.me/Online079" target="_blank">📞 Contact Admin @Online079</a>
          </div>
        </div>
      </main>
    </div>

    <footer>© 2025 Lifetime Income</footer>
  </div>

  <script>
    // Elements
    const loginToggle = document.getElementById('loginToggle');
    const loginForm = document.getElementById('loginForm');
    const options = document.getElementById('options');
    const doLogin = document.getElementById('doLogin');
    const contentArea = document.getElementById('contentArea');
    const sideInfo = document.getElementById('sideInfo');

    // Toggle login form visibility
    loginToggle.addEventListener('click', () => {
      const visible = loginForm.style.display === 'block';
      loginForm.style.display = visible ? 'none' : 'block';
      loginToggle.classList.toggle('active', !visible);
      // hide options when closing form
      if(visible) options.style.display = 'none';
    });

    // When user clicks Login button: show the 5 options area (simulating click-to-open)
    doLogin.addEventListener('click', () => {
      // (Here you could add real auth; for demo we just show the options)
      options.style.display = 'block';
      // show default (Payment) content
      showContent('payment');
    });

    // Clicking items in options list shows content
    document.querySelectorAll('#options li').forEach(li => {
      li.addEventListener('click', () => {
        // highlight clicked
        document.querySelectorAll('#options li').forEach(x => x.style.background = '');
        li.style.background = '#fbfbfb';
        showContent(li.dataset.target);
      });
    });

    // function to populate main content
    function showContent(key){
      let html = '';
      if(key === 'payment'){
        html = `
          <h3>Payment System</h3>
          <p>পেমেন্ট সিস্টেম সম্বন্ধে তথ্য এখানে দেখানো হবে — ব্যবহারকারী Nagad / Bikash করে টাকা পাঠানো ও Screenshot জমা দেবেন।</p>
          <div class="payment-info" style="margin-top:12px">
            <strong>Account তৈরি ফি:</strong> ২০০ টাকা<br>
            💳 <b>Nagad Personal:</b> 01909850916<br>
            💳 <b>Bikash Personal:</b> 01630148084<br><br>
            Send Money করে Screenshot এডমিনের কাছে জমা দিন।
          </div>
        `;
      } else if(key === 'accountInfo'){
        html = `
          <h3>আপনার Account তথ্য</h3>
          <p>এখানে ব্যবহারকারীর Account সম্পর্কিত তথ্য দেখানো হবে — নাম, অ্যাকাউন্ট স্ট্যাটাস, উত্পাদন, রেফারেল লিংক ইত্যাদি।</p>
          <ul>
            <li>Account: <em>(আপনার দেয়া নাম)</em></li>
            <li>Status: Active / Pending</li>
            <li>Referral Bonus: প্রতিটি সফল রেফারেলে ২৫ টাকা</li>
          </ul>
        `;
      } else if(key === 'about'){
        // Use the about content user provided (shortened / formatted)
        html = `
          <h3>About — Wellcome Online BD</h3>
          <p>✅ 'Wellcome Online BD' প্ল্যাটফর্মের সুবিধা ও লাভজনক দিক:</p>
          <ol>
            <li><strong>স্বল্প বিনিয়োগে আয়ের সুযোগ:</strong> মাত্র ২০০ টাকায় শুরু। ভিডিও দেখা ও বিজ্ঞাপন থেকে উপার্জনের সুযোগ।</li>
            <li><strong>কাজের স্বাধীনতা:</strong> যে কোন সময় ও যে কোন জায়গা থেকে কাজ করা যাবে।</li>
            <li><strong>ব্যবসায়িক মডেল:</strong> রেফারেল, বিজ্ঞাপন ও সাবস্ক্রিপশনের মাধ্যমে রাজস্ব।</li>
            <li><strong>আধুনিক প্রযুক্তি:</strong> WhatsApp/Telegram ব্যবহার করে কাজ করা যাবে।</li>
          </ol>
          <p style="font-weight:700">🔥 মূলকথা: একটি লাভজনক উদ্যোগ — স্বল্প মূলধনের, দ্রুত প্রসারের মডেল।</p>
          <p><a href="https://t.
