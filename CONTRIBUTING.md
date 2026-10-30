# Contributing to FI TUNE

Thanks for helping improve FI TUNE. Issues and pull requests should focus on one change, include enough detail to review it, and preserve the upstream GPL-3.0 notices.

## Development setup

1. Install Android Studio, the Android SDK, Git, and a compatible JDK.
2. Clone this repository and initialize its submodules:

   ```powershell
   git clone --recurse-submodules https://github.com/ignite-1018/FI-TUNE.git
   cd FI-TUNE
   ```

3. Open the project in Android Studio or build a debug APK:

   ```powershell
   .\gradlew.bat assembleGmsMobileUniversalDebug
   ```

Keep local configuration in the untracked `local.properties` file. Never commit signing keys, passwords, API keys, or access tokens.

## Before opening a pull request

- Explain the user-visible behavior and how you tested it.
- Run the narrowest relevant Gradle test or build task.
- Keep changes focused and retain all GPL-3.0 notices.
- Mark modified files as changed where required by the license.

## License and attribution

FI TUNE is a GPL-3.0 derivative of [ArchiveTune](https://github.com/rukamori/ArchiveTune). Contributions to this repository are distributed under GPL-3.0 and must preserve the applicable source notices.
