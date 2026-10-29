# FI TUNE

FI TUNE is a community-developed derivative of [ArchiveTune](https://github.com/rukamori/ArchiveTune), an Android music player. It is not affiliated with or endorsed by the ArchiveTune maintainers.

## What changed

- App display name: FI TUNE
- Android application ID: `com.fitune.app`
- GitHub release updates use the FI TUNE repository; they become useful once this project publishes releases.
- The upstream remote-service endpoint is not reused; remote gatekeeper functionality remains disabled until configured with an FI TUNE-controlled service.

The original Kotlin package namespace and copyright notices are retained to preserve upstream attribution.

## Build

Open the project in Android Studio or build it with the Gradle wrapper after installing the Android SDK and required toolchains:

```powershell
.\gradlew.bat assembleGmsMobileUniversalDebug
```

To use a different GitHub repository, set the following values in an untracked `local.properties` file:

```properties
GITHUB_OWNER=your-github-username
GITHUB_REPO=your-repository
RELEASE_GITHUB_OWNER=your-github-username
RELEASE_GITHUB_REPO=your-repository
```

Do not commit signing keys, passwords, API keys, or other credentials.

## License and attribution

FI TUNE is derived from ArchiveTune and is distributed under the GNU General Public License, version 3. The upstream `LICENSE` and source copyright notices are retained. Changes in this derivative must be marked, and any distributed derivative must also comply with GPL-3.0, including making its corresponding source available.
