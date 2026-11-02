# How to install an app from Spartan Speaks

These apps aren't on the Play Store, so you install them directly from an **APK file**. It's safe and takes about a minute.

## On your Android phone

1. **Download the APK.** Tap the **⬇ Download APK** button on the [main page](../README.md), or open the [Releases page](https://github.com/Mathi-Spartan/Spartan-Speaks---Android-Studio/releases) and tap the `.apk` file under **Assets**.
2. **Open it.** When the download finishes, tap the notification, or open your **Files** / **Downloads** app and tap the file.
3. **Allow installs from this source (first time only).** Android will say something like *"For your security, your phone is not allowed to install unknown apps from this source."*
   - Tap **Settings**
   - Turn on **Allow from this source**
   - Go back
4. **Tap Install.** Then tap **Open**. Done 🎉

## "Blocked by Play Protect"?

Google Play Protect sometimes warns about apps that aren't from the Play Store, just because it hasn't seen them before.

- Tap **More details**, then **Install anyway**.
- If it offers to **send the app for a security scan**, you can say yes or no. Either is fine.

## Updating to a new version

Download the newer APK and install it the same way. It installs **over** the old version and **keeps your data**.

> If Android says the app *"conflicts with an existing package"*, the new file was signed differently. Back up your data inside the app first, uninstall the old version, then install the new one.

## Check your download (optional)

Each app page lists a **SHA-256** checksum. To confirm your file wasn't changed:

- **Windows (PowerShell):** `Get-FileHash .\Uyir-1.0.49.apk -Algorithm SHA256`
- **Mac / Linux:** `shasum -a 256 Uyir-1.0.49.apk`

The result should match the one on the app's page.

---

<sub>[← Back to all apps](../README.md) · [FAQ](FAQ.md)</sub>
