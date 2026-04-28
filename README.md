# Pokemon Champions Battle Logger

<p align="center">
  <img src="https://img.shields.io/github/v/release/fufufukakaka/pokemon_champions_battle_logger?style=flat-square&color=FF3B30" alt="Release">
  <img src="https://img.shields.io/github/downloads/fufufukakaka/pokemon_champions_battle_logger/total?style=flat-square&color=00B4DC" alt="Downloads">
  <img src="https://img.shields.io/badge/platforms-Windows%20%7C%20macOS%20%7C%20Linux-32D74B?style=flat-square" alt="Platforms">
  <img src="https://img.shields.io/badge/license-MIT-555?style=flat-square" alt="License">
</p>

<p align="center">
  <strong>Dominate Your Battle Data</strong><br>
  ポケモンの対戦動画から自動で記録・解析を行うツールです。
</p>

---

## 機能

- **自動バトル検出** — YouTube URL またはローカル動画ファイルを入力すれば、AI が自動的にバトルを検出し、ポケモン認識・技解析・勝敗判定を行います
- **詳細な分析** — 勝率推移、選出統計、KO 統計などをリアルタイム ダッシュボードで可視化
- **8 言語対応** — 日本語、英語、繁体中文、簡体中文、韓国語、フランス語、スペイン語、イタリア語、ドイツ語
- **100% ローカル** — データは全てお手元のマシンに保存されます。クラウド連携、アカウント登録、トラッキングは一切ありません
- **無料 & オープンソース**

## ダウンロード

> **最新リリース**: [こちらからダウンロード](https://github.com/fufufukakaka/pokemon_champions_battle_logger/releases/latest)

| プラットフォーム | ファイル |
|----------|------|
| Windows (x64) | `poke-champions-logger-windows-x64-setup.exe` |
| macOS (Apple Silicon) | `poke-champions-logger-macos-arm64.dmg` |
| Linux (x64) | `poke-champions-logger-linux-x64.deb` |

### クイックスタート

1. ご利用のプラットフォームのインストーラを [Releases](https://github.com/fufufukakaka/pokemon_champions_battle_logger/releases/latest) からダウンロード
2. インストール / アプリを起動 (プラットフォーム別の注意事項は下記参照)
3. ブラウザで `http://127.0.0.1:8000` が自動的に開きます
4. 初期設定ウィザードに従って設定 (言語選択、トレーナー名入力)

### Windows ユーザの方へ

初回起動時に Windows SmartScreen が **「Windows によって PC が保護されました」** という警告を表示する場合があります。これは実行ファイルがコード署名されていないためです (Windows のコード署名証明書はオープンソースプロジェクトにとって高額すぎるため見送っています)。

アプリを起動するには:

1. 警告ダイアログの **「詳細情報」** をクリック
2. **「実行」** をクリック

一部のアンチウイルスソフトが誤検出としてフラグを立てる場合もあります。その際は `poke_champions_logger.exe` を例外として追加してください。

### macOS ユーザの方へ

macOS 版は Developer ID 証明書でコード署名されていますが、**Apple によるノータライズは現状未実施**です (Apple のノータリーサービスがこのアプリのバンドル構造に対して断続的に処理失敗している既知の上流不具合のため — [tauri-apps/tauri#11992](https://github.com/tauri-apps/tauri/issues/11992) を参照)。そのため初回起動時に Gatekeeper の警告が表示されます。

> **⚠️ 重要 — macOS Sequoia / Tahoe をご利用の方へ**
>
> 初回起動時の警告ダイアログには **「ゴミ箱に入れる」** と **「完了」** の2つのボタンが表示されます。**「ゴミ箱に入れる」を絶対にクリックしないでください** — インストールしたばかりのアプリが削除されてしまいます。**「完了」** を押した上で、下記の手順に従ってシステム設定からアプリの実行を許可してください。

#### 初回起動の手順 (一度だけ)

##### macOS Sequoia 15 / Tahoe 26 以降

1. ダウンロードした `.dmg` を開き、**Pokemon Champions Battle Logger.app** を **アプリケーション** フォルダにドラッグ
2. アプリを起動すると警告ダイアログが表示されるので **「完了」** をクリック (※ **「ゴミ箱に入れる」は絶対にクリックしないこと**)
3. **システム設定 → プライバシーとセキュリティ** を開く
4. **セキュリティ** セクションまでスクロールすると、*「"Pokemon Champions Battle Logger" は…マルウェアが含まれていないことを検証できなかったため、使用がブロックされました」* と表示されています
5. **「このまま開く」** をクリックし、Touch ID またはパスワードで承認
6. もう一度アプリを起動すると、今度は **「開く」** ボタン付きのダイアログが表示されます — クリックして起動
7. アプリが起動します。次回以降は通常通り起動できます

##### macOS Sonoma 14 以前

1. ダウンロードした `.dmg` を開き、**Pokemon Champions Battle Logger.app** を **アプリケーション** フォルダにドラッグ
2. Finder で **アプリケーション** に移動
3. アプリを **右クリック** (または Control + クリック) し、コンテキストメニューから **「開く」** を選択
4. *「開発元を確認できないため…」* というダイアログが表示されたら **「開く」** をクリック
5. アプリが起動します。次回以降は通常通り起動できます

アプリの署名は `codesign --verify` で完全に検証可能で、登録済みの Apple Developer アカウント `Yusuke Fukasawa (D8NPWYTRLD)` まで遡ることができます。ノータライズは上流の問題が解決され次第、将来のリリースで再有効化する予定です。

## スクリーンショット

### ダッシュボード

<p align="center">
  <img src="docs/dashboard.png" alt="Dashboard" width="800">
</p>

### 動画処理

<p align="center">
  <img src="docs/upload_and_process_video.png" alt="Video Processing" width="800">
</p>

### 分析

<p align="center">
  <img src="docs/analysis.png" alt="Analysis" width="800">
</p>

### バトル詳細

<p align="center">
  <img src="docs/battle_detail.png" alt="Battle Detail" width="800">
</p>

## 動作環境

- **動画入力**: 1920x1080 (1080p) 30fps の動画
- **形式**: ポケモンチャンピオンズのシングルバトル
- **ストレージ**: アプリ本体と初回起動時にダウンロードされるモデルファイルで約 500MB

## コミュニティ

- [バグ報告](https://github.com/fufufukakaka/pokemon_champions_battle_logger/issues/new?template=bug_report.yml)
- [機能リクエスト](https://github.com/fufufukakaka/pokemon_champions_battle_logger/issues/new?template=feature_request.yml)
<!-- - [Discord](https://discord.gg/XXXXX) -->

---

> 🌐 **English version**: see [README.en.md](README.en.md)
