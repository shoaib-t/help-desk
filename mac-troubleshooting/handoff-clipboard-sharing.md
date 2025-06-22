# How to Fix Handoff Clipboard Sharing on macOS

**Context:**  
I have Handoff enabled on all my Apple devices (Mac, iPhone, iPad), but I could not copy/paste between my Mac and my iOS devices. However, clipboard sharing worked only between my iPad and iPhone.

---

## Steps to Fix Clipboard Sharing on Mac

1. **Open Spotlight Search**  
   Press `Command (⌘) + Space` to open Spotlight.

2. **Search for Handoff Settings**  
   Type **handoff** and select **General > AirDrop & Handoff** in System Settings.

3. **Toggle Handoff Off and On**  
   Turn **Handoff** off, then turn it back on again.

4. **Open Terminal**  
   Press `Command (⌘) + Space` again, type **Terminal**, and open the Terminal app.

5. **Enable Clipboard Sharing via Terminal**  
   Run this command to enable clipboard sharing for Handoff:

   ```bash
   defaults write com.apple.coreservices.useractivityd ClipboardSharingEnabled -bool true

6. Restart your Mac (Optional)
   If it doesn’t work immediately, try restarting your Mac
