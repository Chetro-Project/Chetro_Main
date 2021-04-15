# 桜斗/Chetro 研究開発要領 基本計画書

## 基本計画書附属書類

- [付属書 研究開発母体資料](./Proi_Org.md#プロジェクト母体)
- [付属書 基本アーキテクチャ(構成システム)構想](./Arch_Org.md)
- [付属書 CPU 開発方針・仕様案](./hardware/HW_CPU_Base.md)
- [付属書 ブートローダ開発方針・仕様案](./FW_Bootloader.md)

## プロジェクト概要

プロジェクト名:

- 識別名：NOS-NT
- 正式名：桜斗 Project
- 代替名：Chetro Project

プロジェクト内容：TRON ベース Windows 的独自 OS の「桜斗(寧和)」の開発

プロジェクト母体：
[付属書 研究開発母体資料](./Proi_Org.md#プロジェクト母体)参照

## 基本的方向性

- マルチタスク＆リアルタイムオペレーティングシステム
- オープン標準/仕様＆オープンソースシステム/ソフトウェア
- プリエンプション型リアルタイム

### 参考元

- TRON ベース;TOPPERS 含む
- 下記 OS に寄せたデザイン
  - Windows 10
  - Windows 8
  - Windows Me
  - Windows xp
  - Windows Vista
  - React OS
- 下記 OS 的な仕様及び独自仕様を付加
  - Kubuntu
  - Android-x86
  - HAIKU

## ハードウェア条件

最低限次には対応する

- Intel x86-64 (Intel 64) 搭載 プロセッサ向け
- [TRON Chip Neo (TC-nx64)](./hardware/HW_CPU_Base.md) 搭載 プロセッサ向け

## 諸実装関連

- Rust/NASM で実装
- Rust VM/Julia VM/Dart VM/Java VM/Lua VM を標準実装
- Win-x86-64.exe 実行環境(デスクトップ版)/.apk(モバイル版)を標準装備(但し完全最適化はせず)
- 標準 C/Java/Rust/Julia/Dart ライブラリを提供
- 動的メモリ確保手法には TLSF アロケータを採用する

## 基本アーキテクチャ(構成システム)

[付属書 基本アーキテクチャ(構成システム)構想](./Arch_Org.md)参照

## エディション・バージョン・世代・リビジョン

- 寧和 Gen20 NT v2.0.3
- (OS 名) (世代) (エディション) (リビジョン)

### 各概説

- 世代：開発着手年又はリリース年(前者は西暦下 2 桁、後者は西暦下 2 桁＋月 2 桁)

  - Ex) Gen20 　　 2020 年開発着手
  - Ex) Gen2601 　　 2026 年 7 月リリース

- エディション：利用対象の別(次節記載の通り)

  - Ex) NT 　　通常版・一般向け

- リビジョン：修正等関係

## エディション

- 一般向け
  - Lite 　　軽量版・軽量(低性能)パソコン向け(RaspberryPi 他)
  - Smart 　　限定機能版・機能限定パソコン向け(ネットブックの類)
  - NT 　　通常版・一般向け
  - Premium 　　通常高機能版・クリエータ/ゲーマ向け
  - Professional 　　専門的高機能版・電気電子情報通信技術者向け
- 特殊用途向け
  - Super 　　スパコン向け
  - Server 　　サーバ向け
  - Distribute 　　分散処理向け
- 組み込み向け
  - μI-General 　　一般組み込み向け
  - μI-Professional 　　高度機能研究向け
  - μI-Lite 　　軽量組み込み向け
- 携帯端末向け
  - Phone 　　スマートフォン向け
  - Mobile 　　その他モバイル向け
  - Tab 　　　タブレット端末向け
  - Wears 　　ウェアラブル端末向け

### コードネーム

- Gen20： Jupiter
