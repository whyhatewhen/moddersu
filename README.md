## FAQ: Play Protect & Mod APK Installation

### Why does Google Play Protect block modded APKs?
Modded APKs are modified versions of original apps, which means their signing certificate no longer matches the official developer's signature. Play Protect flags any unrecognized signature or altered code as a potential risk and blocks the install by default.

### How do I turn off Google Play Protect?
1. Open the **Google Play Store**.
2. Tap your **profile icon** in the top-right corner and select **Play Protect**.
3. Tap the **Settings (gear) icon** in the top-right corner.
4. Toggle off **Scan apps with Play Protect** and tap **Turn off** to confirm.

*(Optional: You can also disable **Improve harmful app detection** on the same screen if you don't want unknown APKs uploaded to Google for analysis.)*

### Why is the Play Protect toggle grayed out?
If you can't turn it off, one of these restrictions is usually active on your device or account:
- **Google Advanced Protection:** Accounts enrolled in Google's Advanced Protection Program block sideloading entirely, and the setting can't be overridden locally.
- **Work or School Profile (MDM):** Device management policies from an employer or school often lock down security settings.
- **Parental Controls:** Google Family Link restricts changes to app verification settings on supervised accounts.

### Should I re-enable Play Protect after installing?
Yes, it's a good idea to turn it back on once you're done so your other apps stay protected. Just keep in mind that Play Protect may occasionally warn you about the modded app or automatically disable it if Google flags the signature later on.

---

### How do I allow "Install Unknown Apps" on Android?
Before sideloading, you need to give your browser or file manager permission to install APKs:
1. Open **Settings** > **Apps** > **Special app access** > **Install unknown apps** *(or just search "Install unknown apps" in your Settings search bar)*.
2. Pick the app you'll use to open the APK (e.g., Chrome, Files, or ZArchiver).
3. Enable **Allow from this source**.

### How do I install the Mod APK?
1. **Remove the original app first:** If you already have the Play Store version installed, uninstall it. Android will throw an *"App not installed as package conflicts with an existing package"* error if the signatures don't match.
2. **Find the downloaded file:** Open your file manager and head to your **Downloads** folder.
3. **Install:** Tap the `.apk` file and hit **Install**. If a Play Protect prompt still pops up, tap **More details** > **Install anyway**.

### How do I install `.apks`, `.xapk`, or `.apkm` files?
Many modern apps use Android App Bundles (split APKs), which the built-in Android installer can't handle on its own.
- Grab a split-APK installer like **SAI (Split APKs Installer)**, **ZArchiver**, or **AntiSplit-M** (which can merge bundles into a regular `.apk`).
- Open the tool, grant it storage and unknown-app permissions, select your bundle file, and install from there.

### Why won't Google Sign-In work inside a Mod APK?
Google Play Services checks an app's cryptographic signature before allowing OAuth/Google Sign-In. Since a modded APK is signed with a custom test key, Google login will almost always fail.
- **Workaround:** Log in with an email and password instead, or use Facebook login (just uninstall or temporarily disable the official Facebook app first so it signs in through your browser).

### How can I check if a Mod APK is safe before installing?
- **Run it through VirusTotal:** Upload the file (or check its SHA-256 hash) on [VirusTotal](https://www.virustotal.com/). Seeing 1–3 generic flags (like `Android.PUA` or `DebugKey`) is normal because of the re-signing tools modders use, but widespread trojan/spyware warnings mean you should delete it.
- **Check requested permissions:** Pay attention to what the app asks for on first launch. An offline game or simple utility has no business asking for Contacts, SMS, Call Logs, or Accessibility Services.
- **Compare the file size:** Check the size against the official Play Store listing. If an app is normally 100 MB and the APK you downloaded is 3 MB, it's likely an adware dropper.
