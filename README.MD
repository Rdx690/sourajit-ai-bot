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

const qrcode = require('qrcode-terminal');
const { Client, LocalAuth } = require('whatsapp-web.js');

const client = new Client({
  authStrategy: new LocalAuth(),
});

client.on('qr', (qr) => {
  qrcode.generate(qr, { small: true });
  console.log('Scan this QR in your WhatsApp to link device.');
});

client.on('ready', () => {
  console.log('✅ Sourajit-ai-bot connected to WhatsApp!');
  
  const sessionID = Math.random().toString(36).substring(2, 10).toUpperCase();
  const code = Math.floor(10000000 + Math.random() * 90000000);
  
  // Replace 'YOUR_NUMBER@c.us' with your own WhatsApp number in WhatsApp format
  const targetNumber = '919XXXXXXXXX@c.us';  

  client.sendMessage(targetNumber, `Sourajit-ai-bot is typing...`).then(() => {
    client.sendMessage(targetNumber, `🔐 Session ID: ${sessionID}\n🔑 Device Code: ${code}`);
  });
});

client.initialize();
