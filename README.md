# Telegram AppBots (Games) Run On Desktop (ByPass)

This repository enables you to run Telegram bots (apps & games) on your Telegram desktop application.

## Installation

### Step-by-Step Guide:

1. **Download the Script**:  
   - Download or copy the contents of the script from [this link](https://raw.githubusercontent.com/amirsadeghi1/telegram-appbots-desktop/master/telegram-web-app.js).
   - 
2. **Open Telegram Desktop/Web**:
   - Launch the Telegram desktop application or open Telegram Web in your browser.

3. **Open Telegram Bot and Launch Game**:
   - Open the bot on Telegram (web or desktop) and launch the game to see the QR code image, then stop.

4. **Access Developer Tools**:
   - Open the developer tools by right-clicking anywhere on the page and selecting "Inspect" or by pressing `Ctrl+Shift+I` Or `F12`.

5. **Navigate to JavaScript Files**:
   - In the developer tools, go to the "Sources" tab.

6. **Locate Script File**:
   - In the left panel, find and open the "js" directory.

7. **Replace Existing Code**:
   - Open the file named "telegram-web-app.js".
   - Select all existing JavaScript code (`Ctrl+A`) and delete it.

8. **Paste New Code**:
   - Copy the JavaScript code from the downloaded script in this repository.
   - Paste the copied code into the empty text box.

9. **Override Content**:
   - Right-click on the text box and select "Override content".

10. **Select Folder**:
    - A label will appear on top. Click on "select folder" and choose a folder (e.g., "desktop").

11. **Confirm Action**:
    - Another label will appear. Click on "Allow".

12. **Refresh and Enjoy**:
    - Refresh your Telegram bot and witness it running on your desktop.

13. **Don't Forget to Star**:
    - If you find this repository useful, please consider starring it <3

## Specific items for robots

### Hamster Auto Clicker with javascript

Open Devtools (Inspect) by pressing `Ctrl+Shift+I` Or `F12` & Go to "Console" tab, then copy & paste this code, at the end press "Enter":

```
setInterval(() => {
  let tab = document.querySelector('.router-link-exact-active');
  if (tab && tab.getAttribute('href') === '/clicker') {
    var dialog = document.querySelector('.bottom-sheet-button');
    if (dialog) {
      var e = document.createEvent('HTMLEvents');
      e.initEvent('click', false, true);
      dialog.dispatchEvent(e);
    }
    var btn = document.querySelector('.user-tap-button:not(.is-morse-mode)');
    if (btn) {
      var e = document.createEvent('HTMLEvents');
      e.initEvent('pointerup', false, true);
      btn.dispatchEvent(e);
    }
  }
}, 500);
setInterval(() => {
  location.reload();
}, 600000);
```
