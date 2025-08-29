---
title: BitcoinOS_Cardano_Bridgeless_Transfer_Report
date: 2025-05-06
epoch: 556
tags:
  - 観測記録
  - カルダノ
  - FBL
  - ADA
  - BTC
  - ETH
  - SOL
  - 比較
draft: false
---
# ブリッジレスBTC転送（Bitcoin → Cardano）実現報告：BitcoinOSによる実証実験

**出典：[BitcoinOS公式ポスト (2025年5月4日)](https://twitter.com/BTC_OS)**

---

## 概要：何が起きたか？

2025年5月4日、**BitcoinOS（@BTC_OS）**は、BitcoinとCardano間における初の**ブリッジレス（bridge-less）なBTC転送の成功**を報告しました。この技術は、従来の中央集権的ブリッジやラップトークンを使わずに、**ZK（ゼロ知識）証明**を用いたトラストレスな転送を可能にします。

---

## 技術構成とフロー図の解説

### 関係するプレイヤー

| 名前 | 説明 |
|------|------|
| **BitcoinOS** | BTCロックとZK証明（BitSNARK）を提供する中核プロトコル |
| **Sundial Protocol** | Cardanoチェーン上でxBTCを受け取る処理を担当 |
| **ADAHandle (@adahandle)** | ユーザーのCardanoアドレス名（例：@fujimoto）管理 |
| **BitSNARK** | BTCがロックされたことをZKで証明する仕組み |

---

### 処理フロー

```mermaid
graph TD
  A[1 BTC (Bitcoin)] --> B(BitcoinOS)
  B --> C[ZK証明(BitSNARK)]
  C --> D[1 xBTC 発行 (Cardano)]
  D --> E[Sundial受領]
  E --> F[@Handleへ送金]
```

または画像の図を参考：

![ブリッジレス転送図](EBF1AC41-CD30-4737-B16E-2A2CB9D44EF0.png)

---

## 特徴と意義

| 特徴 | 内容 |
|------|------|
| **完全ブリッジレス** | 信頼できる第三者不要、ZKによる自己証明 |
| **Unchained Token Standard** | クロスチェーンで使える新しいxBTC規格 |
| **アドレスではなくハンドルへ送金** | ユーザー名（@name）へ直接転送可能 |
| **セキュアな相互運用性** | CardanoとBitcoinの安全な接続手段 |

---

## 情報源とリンク

- BitcoinOS公式ポスト: [@BTC_OS](https://twitter.com/BTC_OS)
- Sundial Protocol: [@SundialProtocol](https://twitter.com/SundialProtocol)
- ADA Handle: [adahandle.com](https://adahandle.com)

---

作成日時: 2025-05-05 15:08:15

[[cardano_bitcoin_defi_projects]]