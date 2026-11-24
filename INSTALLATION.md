# Installing and Updating Trinity-NEXT

Trinity-NEXT is distributed as an APK through this repository, outside Google Play.
Download only from [Trinity-NEXT Releases](https://github.com/ShakieVan/Trinity-NEXT/releases).
The universal APK works on all supported phones (Android 9 and later, with an accelerometer).

## First Installation

1. Download `TrinityNEXT-X.Y.Z-universal.apk` and open it from your browser or Downloads.
2. If Android requests permission for that source, open its **Settings** link.
   Enable **Allow from this source** only for the app that is opening the APK.
3. Return to the installer and read any security messages before continuing.
4. After installation, you can turn the source's installation permission off again.

Permission to install APKs and a Google Play Protect scan are separate checks.
Granting the first does not mean Google has approved the app.

## Google Play Protect

Play Protect does not know Trinity-NEXT: it is not distributed through Google Play and
is new. When you install it, Android may therefore recommend a scan ("App-Scan
empfohlen") or show a warning. **No scan has been requested for any version so far, so
Play Protect has not rated the app,** neither as harmless nor as harmful. Nothing here is
a clearance.

What the app asks of Android is listed in [PRIVACY.md](PRIVACY.md): internet access for the
update check, the permission to ask Android to install its own update, and vibration. Read
Play Protect's message on your device and decide for yourself.

## Updates Inside the App

1. Open **Updates** on the title screen. When a newer version is known, the title
   screen also shows a note "Neue Version … verfügbar".
2. Check the available version and its notes, then choose **Update herunterladen**
   (download update).
3. Choose **Update installieren** (install update). If needed,
   **Installationsfreigabe** (installation permission) opens Android's settings
   specifically for Trinity-NEXT.
4. Return to the app and start the installation. Android asks for confirmation.
5. On first opening after an update, the app offers a settings link if its
   installation permission is still active, so you can switch it off again.

For the first download, the permission belongs to your browser or file manager;
for an in-app update it belongs to Trinity-NEXT.

The app looks for updates at most once a day while it is open, and at once after
an update. It downloads and installs nothing on its own. Before installing it
checks the file's size and SHA-256 checksum against GitHub's release data, and the
package name, version and signing certificate against the installed app.

## Checking a Download Yourself

Every release lists the SHA-256 checksum of its APK in `SHA256SUMS.txt`. The app is
signed with one certificate, SHA-256
`8eae45ecfd7e5e1d09fd2334b599406dfe36d87845166e5f74dd1ad0241b0b92`.
Android refuses an update that is signed with another one.

## Update Results

Results of real updates through the app are recorded here as they are made.
