---
title: transaction_success_rate_analysis
date: 2025-07-08
epoch: 568
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

# 🔎 オンチェーントランザクション成功率比較とCardanoの優位性

## 📅 データ概要

- **投稿者**：@algerstmehn（X / Twitter）
- **作成日**：2025年7月2日
- **情報源**：FlipsideCrypto（[flipsidecrypto.xyz](https://flipsidecrypto.xyz/)）および Dune Analytics（[dune.com](https://dune.com/)）
- **グラフ内容**：主要ブロックチェーンにおけるオンチェーントランザクションの成功率と失敗率の比較

---

## 📊 チェーン別 成功率ランキング（視覚解析）

![成功率ランキング][def]

| 順位  | ブロックチェーン              | 成功率（緑）  | 失敗率（赤） | 特記事項                                  |
| --- | --------------------- | ------- | ------ | ------------------------------------- |
| 1位  | Algorand              | ほぼ100%  | ごくわずか  | 無料トランザクションあり、UXに優れる                   |
| 2位  | **Cardano (ADA)**     | 約99.9%  | ほぼ0%   | 失敗Tx時も手数料ゼロ。Babel Feesによる署名支払い方式などの影響 |
| 3位  | Ethereum              | 約98〜99% | 少量     | ガス不足、フロントラン等で失敗あり                     |
| 中位  | Avalanche, Polygon など | 約90%前後  | 10%前後  | コンジェスションの影響あり                         |
| 最下位 | **Solana**            | 約65〜70% | 約30%超  | スパムTxによる失敗率上昇が顕著（特にBotやNFT関連）         |

---

## 📌 投稿のポイント翻訳と補足

- **「ユーザー体験（UX）は非常に重要」**  
  → 成功率が高く、失敗しても手数料が発生しない設計はUX向上に貢献

- **$ALGO と $ADA**：  
  → どちらも「失敗時のコストゼロ」を実現している希少なチェーン  
  → DApp開発者や一般ユーザーにとって魅力的な設計

- **Cardanoの特徴**：  
  → Babel Fees（署名者と支払者を分離）やSmart Contractベースの手数料スポンサー機能が整備されつつある

---

## 🧠 なぜCardanoとAlgorandが強いのか？

| 特徴                     | Cardano                        | Algorand                       |
|--------------------------|--------------------------------|--------------------------------|
| 失敗時の手数料           | **ゼロ**（Tx前検証）           | **ゼロまたは極小**            |
| UX最適化構造             | Babel Fees, SmartSig構造       | 無料Txフレームワーク           |
| コンセンサス設計         | PoS（Ouroboros, EUTXO）        | Pure PoS（即時確定）           |
| 開発ツール               | Plutus, Aiken, Marlowe         | TEALベース（やや限定）         |
| 開発者支持               | 中〜高                         | やや低                         |

---

## 📚 出典検証と信頼性（要点）

- **FlipsideCrypto** の複数ダッシュボードで、NEAR・Sei・Ethereumなどの成功率が公開（例：Sei 約99.3%、NEAR 約86.7%）  
  出典：[Flipside SEI分析](https://flipsidecrypto.xyz/hess/sei-performance-vs.-other-chains-ieB_uz)、[NEAR分析](https://flipsidecrypto.xyz/zakkisyed/near-protocol-network-performance-analysis-qC8_86)

- **Solanaの失敗率**について、ZK論文等でもスパムTxによる影響が指摘されている  
  出典：[arxiv.org 論文](https://arxiv.org/abs/2504.18055)

- **Cardanoの失敗時手数料ゼロ設計**は仕様として明確に存在し、公式ドキュメントでも確認可能  
  出典：[Cardano Docs: Fees](https://docs.cardano.org/about-cardano/explore-more/fee-structure)

---

## ✅ 結論とDRep的示唆

- CardanoはUX・失敗時設計・開発者支援の3点で極めて高水準
- Midnightの**DUST生成モデル**（失敗してもNight保持でDUST再生）も、この潮流に沿った設計
- **高成功率 × 低コスト失敗**は、ガバナンス提案やL2展開においても極めて重要なインフラ要件
- 今後、Babel FeesやCharmsの発展により、Cardanoは**トランザクションUXの最適化をリード**する立場にある

---

⏱ 作成日時：2025年7月8日


[def]: /images/transaction_success_rate.png