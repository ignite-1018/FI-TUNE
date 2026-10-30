# FI TUNE

![FI TUNE — Music, your way](assets/fi-tune-banner.png)

FI TUNE is a community-developed Android music player derived from [ArchiveTune](https://github.com/rukamori/ArchiveTune). It is an independent project and is not affiliated with or endorsed by the ArchiveTune maintainers.

## Highlights

- Browse and play music, manage queues and playlists, and search your library.
- Listen to downloaded and cached music, or play audio stored on your device.
- View synced lyrics and customize the player with themes, icon packs, and playback settings.
- Use playback features such as the equalizer, Android Auto, widgets, and media notifications.

## Get FI TUNE

The first FI TUNE release is being prepared. Once published, signed APKs will be available from [GitHub Releases](https://github.com/ignite-1018/FI-TUNE/releases). Until then, build the app from source using the instructions below.

The Android application ID is `com.fitune.app`. The initial release is version `1.0.0` with version code `1`.

## Build from source

Clone the repository and its submodules, open the project in Android Studio, or install the Android SDK and required toolchains and run:

```powershell
git clone --recurse-submodules https://github.com/ignite-1018/FI-TUNE.git
cd "FI-TUNE"
.\gradlew.bat assembleGmsMobileUniversalDebug
```

To enable update checks after publishing FI TUNE releases, use these values in an untracked `local.properties` file:

```properties
GITHUB_OWNER=ignite-1018
GITHUB_REPO=FI-TUNE
RELEASE_GITHUB_OWNER=ignite-1018
RELEASE_GITHUB_REPO=FI-TUNE
ENABLE_GITHUB_UPDATES=true
TOGETHER_SERVER_URL=https://your-server.example
```

Keep `ENABLE_GITHUB_UPDATES` disabled until releases are available. The Together server URL is optional and should point to a service you control. Never commit signing keys, passwords, API keys, or other credentials.

The release workflow builds and signs GMS and FOSS APK variants. It requires the persistent Android signing key in repository Actions secrets: `KEYSTORE` (base64-encoded keystore), `KEY_ALIAS`, `KEYSTORE_PASSWORD`, and `KEY_PASSWORD`. Keep secure backups of the keystore and its passwords; future updates for this application ID must use the same signing identity.

## License and attribution

FI TUNE is derived from ArchiveTune and is distributed under the GNU General Public License, version 3. The upstream `LICENSE` and source copyright notices are retained. Changes in this derivative must be marked, and any distributed derivative must also comply with GPL-3.0, including making its corresponding source available.
