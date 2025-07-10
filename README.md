# spyboyhub
<!DOCTYPE html>
<html lang="en" data-theme="dark">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>SpyBoy Hub</title>
  <style>
    :root {
      --bg-color: #0d0d0d;
      --text-color: #ffffff;
      --card-bg: #1f1f1f;
      --border-color: #444;
    }
    [data-theme="light"] {
      --bg-color: #ffffff;
      --text-color: #000000;
      --card-bg: #f0f0f0;
      --border-color: #ccc;
    }
    body {
      background-color: var(--bg-color);
      color: var(--text-color);
      font-family: 'Segoe UI', sans-serif;
      margin: 0;
      padding: 40px 20px;
      text-align: center;
      min-height: 100vh;
      position: relative;
      overflow-x: hidden;
    }
    .banner {
      font-size: 48px;
      font-weight: bold;
      color: #00ffff;
      text-shadow: 0 0 10px #00ffff, 0 0 20px #00ffff;
      margin-bottom: 10px;
    }
    .subtitle {
      font-size: 22px;
      margin-bottom: 30px;
      border-right: 2px solid;
      white-space: nowrap;
      overflow: hidden;
      width: 0;
      animation: typing 3s steps(30, end) forwards, blink 0.7s step-end infinite alternate;
    }
    @keyframes typing {
      from { width: 0 }
      to { width: 100% }
    }
    @keyframes blink {
      50% { border-color: transparent }
    }
    .search-box {
      display: flex;
      justify-content: center;
      margin-bottom: 25px;
    }
    input[type="text"] {
      padding: 12px;
      width: 250px;
      border: none;
      border-radius: 6px 0 0 6px;
      font-size: 16px;
      outline: none;
    }
    .search-btn {
      padding: 12px 20px;
      border: none;
      background-color: #00bfff;
      color: white;
      font-weight: bold;
      font-size: 16px;
      border-radius: 0 6px 6px 0;
      cursor: pointer;
    }
    .button {
      display: block;
      width: 280px;
      margin: 10px auto;
      padding: 12px;
      font-size: 16px;
      font-weight: bold;
      color: white;
      background-color: var(--card-bg);
      border: 2px solid var(--border-color);
      border-radius: 8px;
      text-decoration: none;
      transition: background-color 0.3s;
    }
    .button:hover {
      background-color: #333;
    }
    .toggle-theme {
      margin-top: 20px;
      cursor: pointer;
      font-size: 14px;
      padding: 6px 12px;
      background-color: #444;
      border: none;
      color: white;
      border-radius: 6px;
    }
    .particles {
      position: absolute;
      top: 0; left: 0;
      width: 100%;
      height: 100%;
      z-index: -1;
      background: radial-gradient(#00ffff33 1px, transparent 1px);
      background-size: 50px 50px;
      animation: move 10s linear infinite;
      opacity: 0.2;
    }
    @keyframes move {
      from { background-position: 0 0; }
      to { background-position: 50px 50px; }
    }
    .member-counter {
      font-size: 14px;
      color: #aaa;
      margin-top: 10px;
    }
    .floating-telegram {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background-color: #229ED9;
      color: white;
      padding: 12px 18px;
      border-radius: 50px;
      font-weight: bold;
      text-decoration: none;
      display: flex;
      align-items: center;
      gap: 10px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.4);
      transition: background-color 0.3s;
      z-index: 999;
    }
    .floating-telegram:hover {
      background-color: #1a8dbf;
    }
    .floating-telegram img {
      width: 20px;
      height: 20px;
    }
  </style>
</head>
<body>

  <div class="particles"></div>

  <div class="banner">SPYBOY</div>
  <div class="subtitle">Welcome to the ultimate hub 💻</div>

  <div class="search-box">
    <input type="text" placeholder="Search here..." />
    <button class="search-btn">🔍</button>
  </div>

  <a class="button" href="https://t.me/I0kspecial_opeing" target="_blank">📢 Join Channel</a>
  <a class="button" href="https://t.me/spyboy_pvts" target="_blank">📝 Contact Me</a>
  <a class="button" href="https://t.me/spyboy_pvts" target="_blank">📞 Support</a>
  <a class="button" href="https://YOUR-FOLDER-LINK.com" target="_blank">📂 Free Folder</a>

  <div class="member-counter">📈 @I0kspecial_opeing — 4.2K+ Members</div>

  <button class="toggle-theme" onclick="toggleTheme()">🌗 Toggle Light/Dark Mode</button>

  <a class="floating-telegram" href="https://t.me/I0kspecial_opeing" target="_blank">
    <img src="https://upload.wikimedia.org/wikipedia/commons/8/82/Telegram_logo.svg" alt="Telegram" />
    Join Channel
  </a>

  <script>
    function toggleTheme() {
      const current = document.documentElement.getAttribute("data-theme");
      document.documentElement.setAttribute("data-theme", current === "light" ? "dark" : "light");
    }
  </script>

</body>
</html>
