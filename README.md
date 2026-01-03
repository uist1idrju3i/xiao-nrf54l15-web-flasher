# study-DAP.js

[![Ask DeepWiki](https://deepwiki.com/badge.svg)](https://deepwiki.com/uist1idrju3i/study-dapjs)

Seeed XIAO nRF54L15向けのブラウザベースのファクトリーリセット・リカバリーツールです。WebUSBとCMSIS-DAPを使用して、インストール不要でブラウザから直接デバイスの復旧やファームウェア書き込みを行えます。

## 機能

- **Recover Only**: CTRL-AP経由でデバイスのマスイレースを実行し、保護されたデバイスをアンロックします
- **Factory Reset**: マスイレース後にファクトリーファームウェア（firmware.hex）を書き込み、デバイスを出荷時状態に復元します
- **OpenBlink XIAO nRF54L15 Firmware Flash**: マスイレース後に[OpenBlinkファームウェア](https://github.com/uist1idrju3i/openblink_XIAO_nRF54L15_Sense)を書き込みます

## 動作確認環境

- MacBook Pro (Apple M3)
- macOS 26.2
- Google Chrome 143.0.7499.170（公式ビルド）（arm64）

## 使い方

1. `index.html`をChromeまたはEdgeブラウザで開きます
2. 免責事項に同意します
3. 実行したい操作のボタンをクリックします
4. WebUSBデバイスピッカーからSeeed XIAO nRF54L15を選択します
5. 操作が完了するまで待ちます

## How to Get

リポジトリをクローンしてサブモジュールを初期化するには、以下のコマンドを実行してください：

```console
$ git clone https://github.com/uist1idrju3i/study-dapjs.git
$ git submodule init
$ git submodule update
```

## ライセンス

このプロジェクトはBSD 3-Clause Licenseの下で公開されています。

使用しているライブラリ：
- [DAP.js](https://github.com/ARMmbed/dapjs) - MIT License
- [platform-seeedboards](https://github.com/Seeed-Studio/platform-seeedboards/) - Apache License 2.0（設定リファレンス）

## Recommended VS Code Extensions

- [Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
