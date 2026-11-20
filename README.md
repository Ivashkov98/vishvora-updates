# Vishvora updates

Where the Vishvora Android app looks for new versions. It reads
`https://raw.githubusercontent.com/Ivashkov98/vishvora-updates/main/latest.json`, and when that names a newer
version than the one installed, downloads the APK named beside it, checks it (the fingerprint in latest.json, the
same app, a higher version, the same signing key) and installs it.

Only the newest APK is kept here. Each update is one commit that adds the new APK, removes the old one and replaces
latest.json. The steps are in the app's project, docs/HANDOFF-ANDROID.md, section 4.7 ("Publishing an update").

To install Vishvora by hand on a new device, open the APK file named in latest.json here and tap "Download raw file".
