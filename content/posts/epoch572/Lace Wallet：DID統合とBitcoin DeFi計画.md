---
title: Lace Wallet：DID統合とBitcoin DeFi計画
date: 2025-07-28
tags:
  - Lace
  - Cardano
  - DID
  - BitcoinDeFi
  - IOG
  - Midnight
categories:
  - カルダノ
  - ウォレット
  - 分散型ID
  - マルチチェーン
draft: false
description: Lace WalletにおけるDID統合『Lace ID』と、Bitcoin DeFi機能追加計画（2025年7月26日発表）の詳細解説とCGTAによるシナリオ分析
aliases:
  - lace-id-bitcoindefi
epoch: 572
---

# 🧠 Lace Wallet の進化：DID統合「Lace ID」とBitcoin DeFi計画

## ✅ 概要

2025年7月26日、IOGはLace Walletに以下の機能統合を発表：

| 項目               | 内容                                                                 |
|--------------------|----------------------------------------------------------------------|
| **Lace ID**        | 分散型ID（DID）を統合し、自己主権型デジタル認証が可能に                     |
| **Bitcoin DeFi**   | ビットコインのDeFi機能をLaceから利用可能に                              |

---

## 🧬 Lace ID：分散型IDの統合計画

| 項目 | 内容 |
|------|------|
| **名称** | Lace ID |
| **目的** | DIDをLaceに統合し、ユーザーが自らの認証情報を安全・私的に管理可能にする |
| **基盤技術** | ゼロ知識証明（ZK）によるプライバシー保護 |
| **活用場面** | dApps認証、DeFi、DAOガバナンス、Web3投票等 |

### 🎯 期待される効果

- 自己主権型IDにより、中央管理なしに「誰が誰か」を証明
- KYC不要のdApp・投票などへの応用が可能
- Web3エコシステム全体への拡張性

---

## 🧾 DIDとは？

| 項目 | 内容 |
|------|------|
| **定義** | Decentralized Identifier：自己主権型デジタルID |
| **例** | 年齢、住所、資格などを必要なときだけ証明可能 |
| **他との違い** | GoogleやFacebookのIDとは異なり、中央機関に依存しない |

---

## 🪙 Bitcoin DeFi：新たな統合機能

### 概要

- **Lace Wallet上で、BitcoinネットワークのDeFi機能**が利用可能に
- クロスチェーンなDeFi接続の第一歩

### 位置づけと背景

- **BitVMX構想**により、Bitcoinを改変せずにスマートコントラクト実行を可能に
- Laceはその利用インターフェースを提供

---

## 🔮 今後の展望（CGTAシナリオ分析）

| シナリオ | 内容 | 出現確率（推定） |
|----------|------|----------------|
| S5: LaceがWeb3認証標準に | DID統合が業界で広く採用される | 20% |
| S4: Cardano内で標準化 | CatalystやDAOで必須ツールに | 35% |
| S3: 限定的採用 | 一部のdAppにのみ限定導入 | 25% |
| S2: 技術停滞 | ZK負荷や規制が障害に | 15% |
| S1: 構想の撤退 | 他プロジェクトとの競争で敗退 | 5% |

---

## 📚 出典・参考

- [Lace Wallet 公式サイト](https://www.lace.io)
- [Midnight Tokenomics and Incentives Whitepaper, 2025年6月版] [oai_citation:0‡⭕️Midnight-Tokenomics-And-Incentives-Whitepaper.pdf](file-service://file-AoSHhiwa8EcVW9V98k2GZb)
- BitVMX構想（IOG発表、2025年7月）
- Cardano・Bitcoin・Midnightクロスチェーン関連資料

---

# 🆚 Lace ID vs Âtrium Profile 比較レポート（2025年7月）

## ✅ 概要比較

| 項目 | Lace ID | Âtrium Profile |
|------|---------|----------------|
| **運営主体** | IOG（Input Output） | Âtrium Labs（Cardano系dApp） |
| **ローンチ状況** | 2025年7月発表、年内実装予定 | 2025年7月22日メインネットローンチ済 |
| **IDの形式** | DID（Decentralized Identifier） | プロファイル名（例：@bwtake） |
| **技術基盤** | ZK（ゼロ知識証明）＋DID標準 | StoaスマートコントラクトでMint |
| **プライバシー設計** | 高い（本人の意思でのみ開示） | 公開前提（ソーシャルID） |
| **主要用途** | DeFi、投票、認証、DAO | コミュニティ可視化、Web3 SNS、DRep連携 |
| **チェーン連携** | マルチチェーン（Lace経由） | Cardano中心 |
| **IDの所有形態** | DID文書として自己管理 | NFTとして自己所有 |

---

## 🧠 技術と思想の違い

### Lace ID の特徴

- **目的**：自己主権型ID（SSI）を実現し、Web3空間での「証明可能なプライバシー」を実装
- **技術的基盤**：ZK（ゼロ知識証明）により「知っていることだけを証明」
- **用途**：
  - dAppログイン（Web3対応）
  - KYC不要のDeFi接続
  - DAO・Catalyst投票
  - 公的サービス認証の可能性も

### Âtrium Profile の特徴

- **目的**：Web3ソーシャルインフラを構築し、アイデンティティの可視化と交流を促進
- **技術的基盤**：StoaスマートコントラクトによりNFT形式でプロフィールをMint
- **用途**：
  - Stake PoolやDRepの顔として表示
  - Atrium内でのユーザー同士の相互接続
  - Web3名刺、活動履歴の蓄積

---

## 🔍 利用シーン別評価

| ユースケース | Lace ID | Âtrium Profile |
|--------------|---------|----------------|
| **KYC不要のDeFi** | ◎（ZK活用で証明可能） | ×（認証機能はない） |
| **DAOやCatalystでの投票** | ◎（匿名証明が可能） | △（公開プロフィールに向く） |
| **DRep・SPOの可視化** | △（非公開が基本） | ◎（視認性が高い） |
| **Web3ソーシャル連携** | △（現在の設計は非公開前提） | ◎（コミュニケーション重視） |
| **ユーザーの身元証明** | ◎（DID標準に準拠） | △（任意の名前、証明性は弱い） |

---

## 🔮 CGTAによるシナリオ予測

| シナリオ | Lace ID | Âtrium Profile |
|----------|---------|----------------|
| **S5：業界標準化** | DID標準の採用によりDeFi接続や国家eID連携も | Cardano外部にも広がるWeb3名刺文化 |
| **S3：限定普及** | 法制度やZKコストで遅れる可能性 | Cardano内部では標準だが、外には出づらい |

---

## 📌 出典・参考

- [Lace公式サイト](https://www.lace.io)
- [Midnight Tokenomics Whitepaper v1.0, June 2025]
- [Âtrium Labs公式ブログ・Discord投稿]
- Cardanoコミュニティ内での検証と利用実態（2025年7月時点）

---

作成日時：2025-07-28