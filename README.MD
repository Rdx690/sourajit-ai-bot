<div align="center">
  <img src="https://files.catbox.moe/y16skc.jpg" alt="SOURAJIT-AI Banner" width="720"/>

  <h1>🚀 SOURAJIT-AI Bot</h1>
  <p>A smart, modular Node.js bot powered by SOURAJIT-AI. Built for developers, VPS automation, and creative AI experiments.</p>

  <p>
    <a href="https://github.com/rdx690/sourajit-ai-bot">GitHub Repo</a> • 
    <a href="https://panel.sourajitai.com">Live Panel</a>
  </p>
</div>

---

## 📦 Features
- 🌐 Clean, minimal Node.js bot framework
- 📊 Winston-powered logging system
- 📜 Simple `.env` configuration support
- ⚙️ Extendable for APIs (Telegram, Discord, etc.)
- 📝 Easy process management via PM2 or Docker (optional)

---

## 📂 Project Structure

## 📱 WhatsApp Linked Device Support

SOURAJIT-AI bot can pair with WhatsApp by generating a secure 8-digit **Pair Code**.  
Once paired, the bot sends session confirmations and messages to your WhatsApp number.

---

## 📷 Device Pairing Process

<div align="center">
  <img src="https://files.catbox.moe/y16skc.jpg" alt="WhatsApp Pairing Process" width="720"/>
</div>

---

## 🔑 Pair Code Example

When you run the bot, it will generate a pair code like this:
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>SOURAJIT-AI Bot Pairing</title>
  <style>
    body { font-family: Arial, sans-serif; background: #111; color: #eee; text-align: center; padding: 50px; }
    h1 { font-size: 3em; color: #0f0; }
    .code { font-size: 4em; margin: 20px; color: #f90; }
    button { padding: 10px 20px; background: #0f0; border: none; color: #000; font-size: 1.2em; cursor: pointer; }
  </style>
</head>
<body>

  <h1>🔐 Pair with SOURAJIT-AI Bot</h1>
  <p>Your secure device pair code:</p>
  <div class="code" id="pairCode">87364522</div>
  <button onclick="generateCode()">🔄 Refresh Code</button>

  <script>
    function generateCode() {
      const code = Math.floor(10000000 + Math.random() * 90000000);
      document.getElementById('pairCode').innerText = code;
    }
  </script>

</body>
</html>
