# BearableWindows
A collection of tips and tricks to make windows (10) more useable
## No Microsoft Account
### During installation / first setup
1. Network
  - When on **Wi-Fi**: Do not connect to a network during setup (can still be done later)
  - On a **wired connection**: Don't plug the ethernet cable in (or unplug before proceeding)
2. ==TODO== or read the instructions on screen an follow those that do **not** lead to a microsoft/online account or _make your experience better_
### When adding an additional account
1. Add someone else to this PC
2. **How will this person sign in?** 
  - click `I don't have this person's sign-in information`
3. **Create account**
  - click `Add a user without a Microsoft account`
4. continue with account creation
## Disable "Finish Setting Up Windows"
1. Press >>win<< + >>i<< or open settings
2. Go to **System**
3. Go to **Notifications and Actions**
4. uncheck "suggest ways I can finish setting up my device to get the most out of Windows"

[Tumblr Source Post](https://www.tumblr.com/fluffmugger/727713701203984384)
## Disable Online Search
1. Open **regedit**
2.
  - For whole machine go to `HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\Windows`
  - For current user go to `HKEY_CURRENT_USER\Software\Policies\Microsoft\Windows`
3. Create new **Key** (Folder) called `Explorer`
4. Navigate there and add new **DWORD (32-bit)** called `DisableSearchBoxSuggestions`
5. Edit and set **value** to `1`
6. close regedit and **reboot**
