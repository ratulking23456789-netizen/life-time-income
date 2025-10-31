me/Online079" target="_blank" class="contact">📞 Contact Admin @Online079</a></p>
        `;
      } else if(key === 'accountFee'){
        html = `
          <h3>Account তৈরি ফি</h3>
          <p><strong>ফি:</strong> ২০০ টাকা</p>
          <p>পেমেন্ট নাম্বার:</p>
          <ul>
            <li>Nagad: 01909850916 (Personal)</li>
            <li>Bikash: 01630148084 (Personal)</li>
          </ul>
          <p>Send Money করে Screenshot এডমিনকে দেখিয়ে আপনার Account অ্যাক্টিভ করবেন।</p>
        `;
      } else if(key === 'contact'){
        html = `
          <h3>Contact Admin</h3>
          <p>Admin টিকটক / Telegram মাধ্যমে যোগাযোগ করুন:</p>
          <p><a href="https://t.me/Online079" target="_blank" class="contact">📞 @Online079</a></p>
          <p style="color:var(--muted)">নোট: কোনো আর্থিক লেনদেন করার আগে সাবধানে যাচাই করে নিন।</p>
        `;
      } else {
        html = <h3>Welcome</h3><p>নির্দিষ্ট অপশন নির্বাচন করুন।</p>;
      }

      contentArea.innerHTML = html;
      // scroll main to top in case
      contentArea.scrollTop = 0;
    }

    // Optional: allow Enter key in password to trigger login
    document.getElementById('password').addEventListener('keyup', function(e){
      if(e.key === 'Enter') doLogin.click();
    });
  </script>
</body>
</html>
