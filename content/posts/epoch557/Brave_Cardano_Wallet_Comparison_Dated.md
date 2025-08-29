---
title: Brave_Cardano_Wallet_Comparison_Dated
date: 2025-05-13
epoch: 557
tags:
  - 観測記録
  - カルダノ
  - FBL
  - ADA
  - ETH
  - SOL
  - 比較
  - Wallet
  - Brave
  - Lace
draft: false
---
以下に、**Brave + Cardano / Chrome + Lace / Brave + Ethereum / Brave + Solana** の使い勝手を比較した表と、それぞれの採用・拡張性に関する**5段階シナリオ分析**を行います。

📅 *最終更新日：2025年5月13日*

---

## 🧩 使い勝手の比較表（2025年5月時点）

| 項目           | Brave + Cardano       | Chrome + Lace      | Brave + Ethereum  | Brave + Solana         |
| ------------ | --------------------- | ------------------ | ----------------- | ---------------------- |
| 対応形式         | 内蔵ウォレット               | 拡張機能（Lace）         | 内蔵ウォレット           | 内蔵ウォレット                |
| 導入手順         | 不要（標準搭載）              | Chrome拡張機能インストール   | 不要（標準搭載）          | 不要（標準搭載）               |
| アセット管理       | $ADA, $NIGHTなどネイティブ | $ADA, NFT, 投票機能など | ETH, ERC-20, NFT  | SOL, SPLトークン, NFT      |
| スマートコントラクト署名 | 対応予定（Plutus、Hydra含）   | 完全対応（Lace Signing） | 完全対応（EIP-712）     | 完全対応（Solana RPC経由）     |
| スワップ機能       | 対応（DEX経由で統合予定）        | 一部DEX接続（Flintなど連携） | Uniswap等と統合済      | Jupiter等と統合済           |
| ID・ガバナンス参加   | Voltaire・MID連携視野あり    | CIP-68対応、投票済アセット管理 | ENS利用可、DAO多数      | SNS（Solana Name）やDAOあり |
| UXの一貫性       | Brave UXに統合           | Chrome依存、別UI       | Brave内で完結         | Brave内で完結              |
| モバイル対応       | Brave Mobileに組込予定     | Laceは現時点でモバイル未対応   | Brave Mobileで完全対応 | Brave Mobileで完全対応      |

---

## 🔮 シナリオ分析（それぞれの将来展開）

### 🟧 Brave + Cardano

| シナリオ | 内容                                     | 出現確率 |
| ---- | -------------------------------------- | ---- |
| S5   | Braveから直接Voltaire参加やMidnight連携（完全集約UX） | 35%  |
| S4   | Cardanoの送受信・スワップが一般化、Braveユーザーの一部が定着   | 40%  |
| S3   | 一部マニア向けで止まり、EthereumやSolanaに押される       | 15%  |
| S2   | Brave開発が優先度低下し統合停滞                     | 8%   |
| S1   | サポート停止・開発中止                            | 2%   |

---

### 🟦 Chrome + Lace（Cardano）

| シナリオ | 内容                                    | 出現確率 |
| ---- | ------------------------------------- | ---- |
| S5   | ChromeでもBraveでも使える最強のCardano拡張として普及   | 30%  |
| S4   | 投票と署名に特化したユーザー向けに定着                   | 35%  |
| S3   | 他の拡張ウォレット（Flint、Eternl）にシェアを奪われやや後退   | 20%  |
| S2   | モバイル非対応の影響で利用者伸び悩む                    | 12%  |
| S1   | Cardanoのブラウザ対応がBrave中心になりLaceの優位性が薄れる | 3%   |

---

### 🟪 Brave + Ethereum

| シナリオ | 内容                                      | 出現確率 |
| ---- | --------------------------------------- | ---- |
| S5   | Brave Wallet上でETH L2（Optimism等）と統合し普及加速 | 30%  |
| S4   | Uniswap・OpenSeaなどの統合でETH主要層が定着          | 40%  |
| S3   | MetaMaskに慣れた層が主に使用、Braveは補完的            | 20%  |
| S2   | ZK化やEIP進化の波にBraveが追従しきれず一部機能遅れる         | 8%   |
| S1   | ZKウォレット主流化でBrave Walletの役割が縮小           | 2%   |

---

### 🟩 Brave + Solana

| シナリオ | 内容                                   | 出現確率 |
| ---- | ------------------------------------ | ---- |
| S5   | Jupiter統合やNFTミント・ゲーム連携が爆発的普及         | 25%  |
| S4   | 開発者フレンドリーなSolana UXがBrave Wallet内で好評 | 35%  |
| S3   | Phantomウォレット等との競合でシェアが限定的に           | 25%  |
| S2   | SolanaのL2移行や過密化で一部Brave連携が滞る         | 10%  |
| S1   | Solanaがトラブルで一時的に除外される                | 5%   |

---

## 🧭 統合的な所感

* **Cardano × Brave**は**UX統合とWeb3思想の親和性**という面で突出。
* **Ethereum × Brave**は**実利重視（DeFi, NFT）層**に最適。
* **Solana × Brave**は**スピードとエンタメ領域（ゲーム/NFT）**で強み。
* **Lace**はガバナンスと投票参加者には不可欠だが、**UXでは統合度が劣る**面も。
