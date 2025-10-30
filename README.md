# 🚀 Run Telegram AppBots (Games) on Desktop – *Bypass Method*

> 💡 Unlock **Telegram Games & Apps** on Telegram Desktop using a smart browser-side script injection hack.  
> 🧠 No extension, no modding – just pure DevTools magic.

![badge](https://img.shields.io/badge/Status-Stable-green)  
![badge](https://img.shields.io/github/stars/amirsadeghi1/telegram-appbots-desktop?style=social)  

---

## 🛠️ Quick — Step-by-Step

> ⏱ Estimated time: 2–5 minutes

1. **Get the script**  
   Download or open the raw file:  
   [`telegram-web-app.js`](https://raw.githubusercontent.com/amirsadeghi1/telegram-appbots-desktop/master/telegram-web-app.js)  
   Or simply copy its contents (`Ctrl+A`, `Ctrl+C`).

2. **Open Telegram Desktop or Telegram Web**  
   Navigate to the bot/game you want to launch.

3. **Start the bot and stop at the QR**  
   Click **Play**. When the QR or login prompt appears, **don’t** scan it yet — leave it visible.

4. **Open Developer Tools**  
   Press `Ctrl+Shift+I` or `F12` to open DevTools.

5. **Go to the “Sources” tab**

6. **Locate `telegram-web-app.js`**  
   In the left sidebar, expand the `js` (or equivalent) folder → open `telegram-web-app.js`.

7. **Replace the file’s content**  
   - Select all (`Ctrl+A`)  
   - Delete  
   - Paste your copied script

8. **Enable Overrides (critical)**  
   - Right-click in the editor → **Override content**  
   - Click **Select folder** → choose or create one (e.g., `telegram-injector`)

9. **Grant permission**  
   When prompted, click **Allow**.

10. **Refresh the page**  
    Press `Ctrl+R`.  
    🕹️ The bot/game should now **run smoothly** on desktop.

11. **Star the repo 💖**  
    If this saved you some reverse-engineering time, star it here → [GitHub Repo](https://github.com/amirsadeghi1/telegram-appbots-desktop)

---

## ❗ Notes & Troubleshooting
- Works best with Chromium-based browsers and Telegram Desktop (Electron).  
- If the file resets after reloading, make sure **Overrides** are enabled and the folder is writable.  
- If it still fails, clear cache or restart DevTools after replacing the file.

---

## 🔒 Disclaimer
This technique temporarily modifies client-side files at runtime.  
Use responsibly — only on accounts or bots you own or have permission to test.
