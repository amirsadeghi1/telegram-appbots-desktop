# 🚀 Run Telegram AppBots (Games) on Desktop – *Bypass Method*

> 💡 Unlock **Telegram Games & Apps** on Telegram Desktop using a smart browser-side script injection hack.  
> 🧠 No extension, no modding – just pure DevTools magic.

![badge](https://img.shields.io/badge/Status-Stable-green)  
![badge](https://img.shields.io/github/stars/amirsadeghi1/telegram-appbots-desktop?style=social)  

---

## ⚙️ What This Does

This tool lets you bypass mobile-only restrictions on Telegram web apps (bots/games) and run them smoothly inside **Telegram Desktop/Web**.

---

## 🛠️ Installation

### 🔟 Step-by-Step Guide

1. **Download the Script**  
   Grab the script from [this link](https://raw.githubusercontent.com/amirsadeghi1/telegram-appbots-desktop/master/telegram-web-app.js)  
   Or just `Ctrl+A` + `Ctrl+C` the raw code.

2. **Launch Telegram Desktop or Telegram Web**  
   Open your bot/game in Telegram Desktop **or** in your browser via [Telegram Web](https://web.telegram.org/).

3. **Start the Game**  
   Click “Play” on the bot. Once the QR code shows up, **pause here** – do *not* scan or continue.

4. **Open DevTools**  
   Press `Ctrl+Shift+I` or `F12` to open **Developer Tools**.

5. **Navigate to Sources**  
   In DevTools, go to the `Sources` tab.

6. **Find `telegram-web-app.js`**  
   Look in the left pane → expand the `js` folder → open `telegram-web-app.js`.

7. **Replace the Existing Code**  
   Inside `telegram-web-app.js`:  
   - Select all (`Ctrl+A`)  
   - Delete  
   - Paste your new script

8. **Override Content (Very Important)**  
   - Right-click inside the code editor → choose **“Override content”**  
   - Click **“Select folder”** on the top bar  
   - Choose any local folder (you can create one called `telegram-injector`)

9. **Grant Access**  
   Click **“Allow”** when prompted.

10. **Refresh the Page**  
    Hit `Ctrl+R` or the refresh button.  
    🕹️ Your bot/app should now **run flawlessly** on desktop.

11. **Star the Repo 💖**  
    If this saved you hours of reverse engineering, leave a ⭐ [right here](https://github.com/amirsadeghi1/telegram-appbots-desktop)!

---

## 🤖 Bot-Specific Hacks

### 🐹 Hamster Kombat – Auto Clicker in JS

Use this simple **JavaScript auto-clicker** for Hamster-style games:

1. Open DevTools → go to the **Console** tab.
2. Paste the following code block and press **Enter**:

```js
setInterval(() => {
  let tab = document.querySelector('.router-link-exact-active');
  if (tab && tab.getAttribute('href') === '/clicker') {
    let dialog = document.querySelector('.bottom-sheet-button');
    if (dialog) {
      let e = document.createEvent('HTMLEvents');
      e.initEvent('click', false, true);
      dialog.dispatchEvent(e);
    }
    let btn = document.querySelector('.user-tap-button:not(.is-morse-mode)');
    if (btn) {
      let e = document.createEvent('HTMLEvents');
      e.initEvent('pointerup', false, true);
      btn.dispatchEvent(e);
    }
  }
}, 500);

// Optional: Reload every 10 mins to avoid crashes
setInterval(() => {
  location.reload();
}, 600000);
