# FI TUNE

FI TUNE は Android 向けの音楽プレーヤーです。YouTube Music と端末内の音楽を再生でき、歌詞、再生履歴、テーマ設定などの機能を備えています。

このプロジェクトは [ArchiveTune](https://github.com/rukamori/ArchiveTune) を基にしたコミュニティ開発の派生版であり、ArchiveTune の開発者とは関係がなく、承認も受けていません。GPL-3.0 のライセンスと著作権表示を維持しています。

## ビルド

Android Studio でこのプロジェクトを開くか、Android SDK と必要なツールをインストールした後、Gradle Wrapper を実行してください。

```powershell
.\gradlew.bat assembleGmsMobileUniversalDebug
```

FI TUNE のリリースを公開した後で GitHub の更新チェックを有効にする場合は、追跡対象外の `local.properties` に設定を追加します。

```properties
GITHUB_OWNER=ignite-1018
GITHUB_REPO=FI-TUNE
RELEASE_GITHUB_OWNER=ignite-1018
RELEASE_GITHUB_REPO=FI-TUNE
ENABLE_GITHUB_UPDATES=true
```

Discord 連携や Together サーバーを使う場合は、自分で管理するサービスの設定を追加してください。

```properties
DISCORD_APPLICATION_ID=your-discord-application-id
TOGETHER_SERVER_URL=https://your-server.example
```

パスワード、署名鍵、API キーなどの秘密情報をコミットしないでください。

## ライセンスと帰属表示

FI TUNE は GNU General Public License version 3 (GPL-3.0) の下で配布される ArchiveTune の派生版です。配布する派生版も GPL-3.0 と対応するソースコード提供の条件に従う必要があります。
