# ArtCraft の調査

AI 画像・動画制作のオープンソース デスクトップアプリ ArtCraft と、同名で語られるシリーズの整理

> 📅 作成: 2026-10-25 / 更新: 2026-10-25

[README へ戻る](../../README.md)

1. [ArtCraft とは](#1-artcraft-とは)
2. [機能とモデル](#2-機能とモデル)
3. [評価と注意点](#3-評価と注意点)
4. [同名のシリーズ (Crafting Apps)](#4-同名のシリーズ-crafting-apps)
5. [出典](#5-出典)

## 1. ArtCraft とは

ArtCraft は、アーティスト・デザイナー・映像制作者向けの「制作エンジン」を名乗るオープンソースのデスクトップアプリ。キャッチコピーは "The IDE for artists." で、2D の構図づくりと 3D のシーン設計を行ってから、用途に合うモデルで画像・動画を生成する。

| 項目 | 内容 |
|---|---|
| リポジトリ | [storytold/artcraft](https://github.com/storytold/artcraft) (Star 約 36.3k ・ Fork 約 5.7k。取得時点) |
| 公式サイト | [getartcraft.com](https://getartcraft.com/) (Windows ・ macOS の安定版) |
| 主な言語 | Rust (リポジトリの構成から推測。GitHub の言語欄は空)。`frontend` ディレクトリあり |
| ライセンス | MIT または Apache-2.0 のデュアル (リポジトリの記載)。サードパーティ素材は NOTICE を参照 |
| 版 | 0.41.0 (2026-09-26 リリース、紹介サイトの記載)。Linux はソースからビルド |
| 作者 | ソフトウェア技術者の Brandon Thomas (報道による。AI 支援で Rust 実装したと述べている) |

> [!NOTE]
> **情報の食い違い。** 紹介サイトは版番号に 0.41.0 と 0.42.0 の両方を載せ、ライセンスも Apache-2.0 と MIT OR Apache-2.0 が混在している。リポジトリの LICENSE と Releases を一次情報として確かめる必要がある。

## 2. 機能とモデル

### Advanced Crafting

2D/3D の合成、画像から 3D メッシュへの変換、キャラクターのポーズ付け、シーンのブロッキング、キャラクターの同一性の転写、背景除去。

### Quick Prompting

テキストからの画像生成、プロンプトによる画像編集、キャンバス編集、画像から動画への変換。

### 対応プロバイダ

ArtCraft 自身のほか Grok ・ Midjourney ・ Sora ・ World Labs。ArtCraft 経由では画像 16 ・ 動画 25 ・ 音楽と音声 5 ・ 3D メッシュ 11 ・ ワールド (スプラット) 5 の計 62 モデルが挙げられている。紹介サイトは Nano Banana ・ FLUX ・ Kling ・ Veo にも触れている。

## 3. 評価と注意点

| 観点 | 内容 (紹介サイトの 0.42.0 / Ubuntu 24.04 での試用記による) |
|---|---|
| 費用 | アプリは無料。ホスト型モデルは有料クレジットか購読が必要。外部プロバイダの自前アカウントも使える |
| アカウント | 起動時にサインアップ画面が出て、アカウントなしでは使えない。閉じるボタンなし |
| 通信 | サインイン前にモデル一覧のためサーバへ接続する。オフライン用途には向かない |
| Discord | 約 60 秒ごとに Discord のステータスを更新。アプリ内に無効化の設定が見つからなかったとの報告 |
| ビルド | 約 13 分 (4 コア)。.deb は 47.6 MB。ディスクは約 5 GB 必要 |
| 資源 | サインイン画面で約 850 MB の RAM (GPU なし機の値)。ウィンドウ既定が 2400×1300 |

これらは第三者の記述で、未検証。自分の環境での実測は今後の課題。

## 4. 同名のシリーズ (Crafting Apps)

報道では、ArtCraft は 2 つの意味で使われる。(1) 上記の AI 画像・動画スタジオ。(2) Adobe 製品の代替を狙う無料のオープンソース アプリ群 (Crafting Apps)。後者は PhotoCraft (Photoshop 相当) ・ FilmCraft (Premiere 相当) ・ LightCraft (Lightroom 相当) などで、Rust 製、Windows ・ macOS ・ Linux 対応、オフラインでアカウント不要とされる。いずれも初期のアルファ段階。

> [!NOTE]
> **未解決。** アプリ数は報道で 7 本と 13 本に割れている。シリーズの一覧と各アプリの状態は、次の調査で一次情報から確かめる。

## 5. 出典

- [GitHub - storytold/artcraft](https://github.com/storytold/artcraft)
- [craftsuite.net - ArtCraft](https://craftsuite.net/artcraft)
- [getartcraft.com](https://getartcraft.com/)
- [ArtCraft Wiki](https://www.artcraft.wiki/)
- [ProPakistani (2026-10-09)](https://propakistani.pk/2026/10/09/free-open-source-copies-of-photoshop-premiere-and-lightroom-are-here/)
- [Windows Mode](https://www.windowsmode.com/?p=47621)
- [Showmetech](https://www.showmetech.com.br/artcraft-alternativas-gratuitas-photoshop-premiere-lightroom/)

[README へ戻る](../../README.md)
