---
title: 🚀atala_prism_hyperledger_review
date: 2025-04-26
epoch: 554
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

# 🔍 Atala PRISMとHyperledgerの関係性：検証と現状

## 1. **Atala PRISMのHyperledgerへの貢献**

2023年12月、IOGはAtala PRISMの一部である「Open Enterprise Agent（OEA）」をHyperledger Labsに貢献しました。  
このOEAは、Scalaで構築された自己主権型アイデンティティ（SSI）エージェントであり、W3CのDID仕様やHyperledger AriesのRFCに準拠しています。  
その後、OEAは「Hyperledger Identus」として正式なHyperledgerプロジェクトに昇格しました。  

🔗 [IOG公式ブログ](https://iohk.io/en/blog/posts/2023/12/04/iog-contributes-atala-prism-to-hyperledger-foundation/?utm_source=chatgpt.com)  
🔗 [Project Catalyst（関連提案）](https://projectcatalyst.io/funds/9/cross-chain-collaboration/atala-prism-zkp-hyperledger-aries?utm_source=chatgpt.com)  
🔗 [Hyperledger Identus開発支援提案](https://projectcatalyst.io/funds/12/cardano-open-developers/hyperledger-identus-feature-development?utm_source=chatgpt.com)

---

## 2. **Hyperledger Identusの特徴とカルダノとの連携**

- **ブロックチェーン統合**：Identusは、カルダノブロックチェーンを検証可能なデータレジストリ（VDR）として使用し、DIDの作成、更新、解決を行います。  
- **DIDComm v2のサポート**：DIDComm v2プロトコルにより、エージェント間の安全な通信を実現。  
🔗 [Identus GitHub](https://github.com/hyperledger-identus/identus?utm_source=chatgpt.com)  
- **クラウドエージェント設計**：Dockerなどのコンテナ環境でのデプロイが可能。  
🔗 [OEA紹介記事](https://www.lfdecentralizedtrust.org/blog/introducing-open-enterprise-agent-a-new-hyperledger-lab-for-self-sovereign-digital-identity-dapps?utm_source=chatgpt.com)

---

## 3. **Atala PRISMとHyperledger Ariesの相互運用性**

Catalyst Fund7にて「Hyperledger-Prism Interoperability」が採択され、以下の2つのレイヤーを実現：

- **DIDComm v1通信レイヤー**：標準化されたエージェント通信。
- **検証可能なクレデンシャルのマッピング機構**：Hyperledger Aries ↔ Atala PRISM間でのVC変換。

🔗 [提案ページ](https://projectcatalyst.io/funds/7/accelerate-decentralized-identity/hyperledger-prism-interoperability?utm_source=chatgpt.com)

---

## 4. **コードリポジトリと開発状況**

- **Atala PRISM Node**：カルダノ上でのDID操作を行うノード実装。  
- **Identus Cloud Agent**：DID作成やクレデンシャル発行などを担う。  
🔗 [Identus紹介記事](https://iohk.io/blog/posts/2025/01/27/hyperledger-identus-then-now-and-tomorrow/?utm_source=chatgpt.com)  
- **Identus SDKs**：TypeScript / Kotlin Multiplatform対応の開発ツール群。  
🔗 [SDK GitHub](https://github.com/hyperledger-identus/sdk-kmp?utm_source=chatgpt.com)

---

# ✅ 結論：統合の現状と今後の展望

- **統合の現状**：Atala PRISMの技術はHyperledger Identusとして正式採用され、カルダノと連携。
- **今後の展望**：自己主権型IDの標準化と相互運用性を推進し、CardanoのID基盤として拡大予定。
