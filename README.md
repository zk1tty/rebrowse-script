# Hosting Bash Scripts on Custom Domain - Solutions Guide

## Overview
You want to host your `install-chromium.sh` script on your custom domain so users can install your tool with:
```bash
curl -LsSf https://script.rebrowse.me/install.sh | sh
```

### local test

```bash
sh public/install-chromium.sh
``` 

### expacted result

```bash


-e ██████╗ ███████╗██████╗ ██████╗  ██████╗ ██╗    ██╗███████╗███████╗
-e ██╔══██╗██╔════╝██╔══██╗██╔══██╗██╔═══██╗██║    ██║██╔════╝██╔════╝
-e ██████╔╝█████╗  ██████╔╝██████╔╝██║   ██║██║ █╗ ██║███████╗█████╗  
-e ██╔══██╗██╔══╝  ██╔══██╗██╔══██╗██║   ██║██║███╗██║╚════██║██╔══╝  
-e ██║  ██║███████╗██████╔╝██║  ██║╚██████╔╝╚███╔███╔╝███████║███████╗
-e ╚═╝  ╚═╝╚══════╝╚═════╝ ╚═╝  ╚═╝ ╚═════╝  ╚══╝╚══╝ ╚══════╝╚══════╝


🚀 Chromium Setup
========================================

-e ℹ️  Detected OS: macos
-e ℹ️  Installing macOS dependencies...
-e ℹ️  Installing Python 3.11 (current version 3.9.6 is too old)...
==> Downloading https://formulae.brew.sh/api/formula.jws.json
==> Downloading https://formulae.brew.sh/api/cask.jws.json
Warning: python@3.11 3.11.13 is already installed and up-to-date.
To reinstall 3.11.13, run:
  brew reinstall python@3.11
-e ℹ️  Using Python 3.11 from Homebrew: /opt/homebrew/bin/python3.11
-e ℹ️  Chromium already installed
-e ✅ macOS dependencies installed
-e ℹ️  Checking Python version using: /opt/homebrew/bin/python3.11
-e ℹ️  Python version: 3.11.13
-e ✅ Python version 3.11.13 meets requirements (>=3.11)
-e ℹ️  Installing Python dependencies...
-e ℹ️  Using Python: /opt/homebrew/bin/python3.11 (version: 3.11.13)
Requirement already satisfied: pip in /opt/homebrew/lib/python3.11/site-packages (25.1.1)
-e ℹ️  Installing browser-use and dependencies...
-e ✅ Python dependencies installed
-e ℹ️  Installing Playwright Chromium browser...
-e ✅ Playwright Chromium browser installed
-e ℹ️  Verifying installation...
INFO     [browser_use.telemetry.service] Anonymized telemetry enabled. See https://docs.browser-use.com/development/telemetry for more information.
INFO     [browser_use.BrowserSession🆂 c2c5.76] 🌎 Launching new local browser playwright:chromium keep_alive=False user_data_dir= ~/.config/browseruse/profiles/default
INFO     [browser_use.BrowserSession🆂 c2c5.76]  ↳ Spawned browser_pid=56404 ~/Library/Caches/ms-playwright/chromium-1169/chrome-mac/Chromium.app/Contents/MacOS/Chromium
INFO     [browser_use.BrowserSession🆂 c2c5.76] 🛑 Closing browser_pid=56404 browser context <BrowserContext browser=None>
✅ Browser test successful! Page title: ''
-e ✅ Installation verification passed!
-e ℹ️  Creating usage example...
-e ✅ Usage example created at ~/rebrowse_example.py
-e ℹ️  Run it with: /opt/homebrew/bin/python3.11 ~/rebrowse_example.py

-e ✅ 🎉 Installation completed successfully!

-e ℹ️  🚀 Running example demonstration...
This will show browser automation in action!

👀 Watch for:
  - 🌸 Pink bouncing REBROWSE screensaver with sparkles
  - Browser window opening
  - Navigation to rebrowse.me and httpbin.org
  - Page titles being extracted

💡 To skip this demo next time, use: SKIP_DEMO=1 curl ... | bash

INFO     [browser_use.telemetry.service] Anonymized telemetry enabled. See https://docs.browser-use.com/development/telemetry for more information.
=== Browser-Use Example Script ===
This script demonstrates browser automation with browser-use library

🚀 Starting browser automation example...
ℹ️ rebrowse.png not found, using text logo
🌸 Custom Rebrowse screensaver enabled! Logo: REBROWSE
INFO     [browser_use.BrowserSession🆂 9eca.40] 🌎 Launching new local browser playwright:chromium keep_alive=False user_data_dir= ~/.config/browseruse/profiles/default
INFO     [browser_use.BrowserSession🆂 9eca.40]  ↳ Spawned browser_pid=56427 ~/Library/Caches/ms-playwright/chromium-1169/chrome-mac/Chromium.app/Contents/MacOS/Chromium
📍 Navigating to rebrowse.me...
📄 Page title: Rebrowse - Loom for workflow automation
🔗 Current URL: https://www.rebrowse.me/
📍 Navigating to httpbin.org...
📄 New page title: httpbin.org
🔄 Closing browser...
INFO     [browser_use.BrowserSession🆂 9eca.40] 🛑 Closing browser_pid=56427 browser context <BrowserContext browser=None>
✅ Browser automation completed!

-e ✅ ✨ Example demonstration completed successfully!
🎯 Everything is working perfectly!

🎉 Installation & Demo Complete!
=================================

What just happened:
✅ Python 3.11+ installed and configured
✅ browser-use package installed
✅ Playwright Chromium browser installed
✅ Example script created and tested

Next steps:
1. 🎯 You're all set!
2. 🤖 For headless mode, set headless=True in the BrowserProfile
3. 🗣️ Get support on Telegram: https://t.me/n0rixpunks

Files created:
- ~/rebrowse_example.py (your starting template)
- ~/.rebrowse_install.log (installation log)

Troubleshooting:
- Re-run example: /opt/homebrew/bin/python3.11 ~/rebrowse_example.py
- For headless issues: uncomment --disable-gpu in the script
- Python path: /opt/homebrew/bin/python3.11
```