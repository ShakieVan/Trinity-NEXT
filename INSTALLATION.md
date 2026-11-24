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

**Play Protect blocked the update to version 1.0.1 in a test on November 24, 2026.** On an
Android 16 emulator, during an update from 1.0.0 through the app, it reported "Schädliche
App blockiert" (harmful app blocked) with the text "Diese App könnte schädlich sein" (this
app may be harmful). It named no specific behaviour or file. The block was not overridden
and Play Protect was not switched off; 1.0.0 stayed installed in that test.

What led up to it, on the same emulator and the same day: when 1.0.0 was installed as an
update a few minutes earlier, Play Protect only recommended a scan because it did not know
the app ("App-Scan empfohlen"). The scan was not requested, and a second start of the
installation went through. No scan was requested for 1.0.1 either. The emulator had
Android's automatic sending of unknown apps to Google switched on, so Google may have
analysed 1.0.0 after it was installed there; that is an assumption, not something that
was observed.

On the owner's Galaxy S24 the update from 1.0.0 to 1.0.1 through the app was installed on
the same day (the owner's report; what Play Protect showed there was not recorded).

The classification is unexplained. It is neither confirmed as a false alarm nor withdrawn
by Google, and nothing here is a clearance.

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

- **November 24, 2026, to 1.0.0, Android 16 emulator: completed.** An older local test
  build (0.9.0) found 1.0.0, downloaded it and verified its size, checksum, package,
  version and signing certificate. Android's installer asked for confirmation. Play
  Protect then recommended a scan because it did not know the app ("App-Scan
  empfohlen"); the scan was not requested, and Android discarded this first attempt
  ("App wurde nicht installiert"). A second start of the installation from the app was
  completed by Android without a further Play Protect dialog. The installed file
  matched the public one byte for byte, and the app's reminder led to switching its
  installation permission off again. No scan was requested for this version.
- **November 24, 2026, from 1.0.0 to 1.0.1, Android 16 emulator: not completed.** The
  public 1.0.0 showed "Neue Version 1.0.1 verfügbar" on its title screen, downloaded
  1.0.1 and verified its size, checksum, package, version and signing certificate.
  After the confirmation in Android's installer, Google Play Protect blocked the
  installation ("Schädliche App blockiert", see above). The block was not overridden;
  1.0.0 stayed installed.
- **November 24, 2026, from 1.0.0 to 1.0.1, Galaxy S24: completed** according to the
  app's owner, who updated through the app on their own phone.
