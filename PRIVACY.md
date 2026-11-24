# Privacy

Trinity-NEXT does not include advertising, analytics, purchases or an account system.

- Your games (the one you left open in each mode, your lists of best games) and your
  options are stored on your device.
- Android backup and device transfer may also copy them, depending on your system
  settings. Trinity-NEXT does not operate a server of its own.
- The game reads the phone's tilt from its motion sensor while a game is open, to decide
  which way the stones slide. These readings are used at once and are neither stored nor
  sent anywhere.
- The updater contacts GitHub for release information and for downloads you request.
  GitHub receives ordinary connection information, including your IP address.
  See [GitHub's privacy statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement).
- Automatic update checks happen at most once a day while the app is open, and at
  once after an update. Downloads and installations require your action; nothing
  runs in the background.
- Downloaded APKs stay in the app's private cache, are excluded from Android
  backup and are temporarily shared with Android's installer. No GitHub token is
  required or stored.
- The app requests three Android permissions: internet access (for the update check),
  the permission to ask Android to install its own update, and vibration. A fourth entry
  in the app's manifest, `de.shakie.trinitynext.DYNAMIC_RECEIVER_NOT_EXPORTED_PERMISSION`,
  is added by the AndroidX library; it only shields the app's own internal messages
  and gives access to nothing.

Android, your browser and Google Play Protect have their own data handling and
security checks. This document describes Trinity-NEXT, not those external services.
