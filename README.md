# Flashlight Alert

Flashlight Alertは、Androidスマートフォンのライトが点灯したまま端末が非操作になった場合に、設定時間の経過後に通知するアプリです。

## ダウンロード

最新の署名済みAPKは[Releases](https://github.com/nao-dev-space/flashlight-alert-releases/releases)からダウンロードしてください。

各リリースでは、次の2ファイルを配布します。

- `Flashlight-Alert-vX.Y.Z.apk`: インストール用APK
- `SHA256SUMS.txt`: APKが正規の配布物と一致することを確認するためのSHA-256

GitHubが自動表示する「Source code」は、この配布リポジトリのREADMEとプライバシーポリシーだけを含み、Androidアプリのソースコードは含みません。

## インストール

1. ReleasesからAPKをAndroid端末へダウンロードします。
2. Androidの案内に従い、ダウンロードに使用したブラウザーまたはファイル管理アプリについて「不明なアプリのインストール」を許可します。
3. APKを開いてインストールします。
4. インストール後、「不明なアプリのインストール」の許可を無効に戻すことを推奨します。
5. Flashlight Alertを開き、通知権限を許可します。アプリからライトを操作する場合は、カメラ権限も許可します。

Google Play外からの配布であるため、自動更新はありません。更新版が公開された場合は、新しいAPKをダウンロードして上書きインストールしてください。

## 正規性の確認

Windows PowerShellでは、APKと`SHA256SUMS.txt`を同じフォルダーへ保存し、次を実行します。

```powershell
Get-FileHash .\Flashlight-Alert-vX.Y.Z.apk -Algorithm SHA256
Get-Content .\SHA256SUMS.txt
```

表示された2つのSHA-256が一致しない場合は、APKをインストールしないでください。

正式なAPKの署名証明書SHA-256は次の値です。

```text
9b9e138855aae66c82ced3aec00914f090c5c361c5660861fe042dfb9cbc16dc
```

## プライバシー

本アプリは外部通信、広告、分析、クラウド保存を行いません。詳細は[プライバシーポリシー](PRIVACY.md)を参照してください。

## 問い合わせ

不具合は、このリポジトリの[Issues](https://github.com/nao-dev-space/flashlight-alert-releases/issues)で報告してください。報告にはパスワード、個人情報、その他の秘密情報を記載しないでください。

## ソースコードと再配布

Androidアプリのソースコードは公開していません。本リポジトリにオープンソースライセンスは付与していません。APK、文書、画像その他の内容について、明示的に許可していない複製、改変、再配布を許可しません。

Copyright (c) 2026 nao-dev-space. All rights reserved.
