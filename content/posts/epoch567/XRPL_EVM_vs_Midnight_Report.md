---
title: XRPL_EVM_vs_Midnight_Report
date: 2025-07-01
epoch: 567
tags:
  - 観測記録
  - カルダノ
  - FBL
  - ADA
  - 比較
  - XRPL
draft: false
---

# XRPLのEVM互換サイドチェーン正式稼働とMidnightとの比較分析

## 📰 ニュース概要

2025年6月30日、リップル社はXRP Ledger（XRPL）における**EVM互換サイドチェーン**のメインネット稼働を発表。  
これによりXRPL上でEthereum系DAppやSolidityが使えるようになり、ガス代は**XRP**で支払われる。

| 項目 | 内容 |
|------|------|
| 技術 | Ethereum仮想マシン（EVM）互換のサイドチェーン |
| 主導企業 | Ripple, Peersyst, Axelar |
| 使用言語 | Solidity |
| ウォレット互換 | MetaMask 対応 |
| ガス代通貨 | **XRP** |
| ユースケース | トークン化、レンディング、決済、機関向けDeFi |
| コメント | 「XRPがマルチチェーン世界を移動する時代の始まり」 - Peersyst CEO |

---

## 🧠 Midnightとの構造的比較

| 項目 | XRPLのEVMサイドチェーン | Midnight（Cardano Partner Chain） |
|------|--------------------------|------------------------------------|
| 立場 | サイドチェーン（補助） | Partner Chain（独立性高） |
| ガス代通貨 | XRP（価格変動あり） | DUST（NIGHTから生成、価格非連動） |
| トークン構造 | 単一トークン構造 | **二重構造（NIGHT → DUST）** |
| プライバシー保護 | なし | ZKベースでトランザクション秘匿 |
| 拡張性 | EVM互換に限定 | Babel Fees, Multichain Observability対応 |
| スパム耐性 | XRPコスト依存 | DUSTの減衰＋ZK証明により強固 |

---

## 📌 議論の要点と評価

### XRPL EVMサイドチェーンの強み
- XRPエコシステムにEVMの開発資産を取り込む戦略
- MetaMaskやSolidityなどの開発ツールを流用可能
- 規制下の資産・ウォレットと接続しやすい構造

### 限界と懸念
- XRPの価格変動によるガス代不安定性
- プライバシー保護の欠如
- プロトコル的に「ガスと価値の分離」が実現されていない

---

## 🧬 Midnightの二重構造的優位性

Midnightは、次世代Web3設計として以下の点で抜きん出ている：

- トークン（NIGHT）とリソース（DUST）の**分離設計**
- DUSTは非譲渡・価値非保持・プライバシー保護
- ガス費モデルと価格・スパム・プライバシー問題を切り離し

---

## 🔚 結論

XRPLのEVM互換サイドチェーンは、**既存のEVMエコシステムとの統合による即効性ある戦略**である一方で、  
Midnightのような**制度的かつ構造的設計の刷新（L1に近いL2＋二重構造）とは本質的に異なる方向性**である。

Midnightは今後のWeb3における**公共インフラ型の次世代L2モデル**として、模倣困難かつ先進的な基盤を提供する。

---

📘 出典：
- Ripple社発表（2025年6月30日）
- Midnight Tokenomics and Incentives Whitepaper（2025年6月）
- Wormhole, Axelarパートナーシップ情報（XRPL関連）

作成日時：2025年7月1日
