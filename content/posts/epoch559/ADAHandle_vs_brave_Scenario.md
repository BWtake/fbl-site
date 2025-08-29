---
title: ADAHandle_vs_brave_Scenario
date: 2025-05-24
epoch: 559
tags:
  - 観測記録
  - カルダノ
  - FBL
  - ADA
  - 比較
  - ADAHandle
  - Brave
  - シナリオ分析
draft: false
---
# ADA Handle vs .braveドメイン 徹底比較とシナリオ分析

📅 最終更新日：2025年5月24日

---

## 🧩 機能・構造・思想の比較表

| 比較項目        | ADA Handle                  | Unstoppable Domains（.brave）                         |
| ----------- | --------------------------- | --------------------------------------------------- |
| 対応チェーン      | **Cardano（UTxO/EUTxO）**     | **Polygon/Ethereum/Solana/Bitcoin/Base**（EVM/UTXO系） |
| 名前形式        | `@takeshi`                  | `takeshi.brave`                                     |
| 所有形式        | Cardano NFT（CIP-68）         | ERC-721 NFT（Polygon）                                |
| 所有媒体        | Cardanoウォレット（Lace, Eternl等） | Brave Wallet（ネイティブ）または他EVMウォレット                     |
| 紐づけられるアドレス  | ADAアドレス1つ（将来複数化も可）          | 310種類以上の暗号資産アドレス                                    |
| 対応機能        | ADA送金短縮、NFT表示、プロフィール（開発中）   | 送金、分散型サイト、NFT証明、dAppログインなど                          |
| 分散型Web対応    | ❌（現時点では非対応）                 | ✅（IPFS連携可能）                                         |
| DID対応       | PRISMとの連携で分散IDへ拡張予定         | 分散IDとしての活用が進んでいる（Web3ログイン等）                         |
| サポートウォレット   | Lace, Eternl, Typhonなど      | Brave Wallet（標準）                                    |
| 更新料         | ❌ なし                        | ❌ なし（買い切りNFT型）                                      |
| 発行・管理主体     | ADA Handleチーム               | Unstoppable Domains社（米国）                            |
| 商標取得機能      | ❌ なし（実名でも自由に取得可）            | ✅ 商標権所有者が優先取得可能                                     |
| 登録情報の公開/非公開 | ❌ メタデータに準拠                  | ✅ デフォルト非公開（オプトイン型）                                  |

---

## 🧠 機能面での長所と短所

| 観点           | ADA Handleの強み                          | .braveの強み                                   |
|----------------|--------------------------------------------|------------------------------------------------|
| カルダノ連携   | Cardanoネイティブ、送金UXが革新的       | Brave Walletとの統合でマルチチェーン簡便       |
| 簡潔さ         | `@名前` という非常に簡易な構文           | `.brave` でWeb2ライクな覚えやすさ              |
| Web3応用       | ガバナンス、投票、NFT称号と統合しやすい  | IPFS対応、Web3プロフィール・分散サイトに強み   |
| 認知と市場     | Cardano限定コミュニティで高認知           | Braveユーザー（8500万人）＋多数チェーン対応    |

---

## 🔮 シナリオ分析（5段階）

### ✅ S5：完全共存・クロスチェーンDID実現（20%）
ADA Handleと.braveがそれぞれの強みを持ちながら、分散IDとして連携・互換性を持つ未来

### ✅ S4：機能別住み分け型共存（35%）
ADA HandleはCardanoガバナンス・NFTなどに特化、.braveはWeb3ログイン・Webサイト用途に強み

### ✅ S3：ユーザー主導で統合志向（25%）
Brave WalletのCardano完全対応が進み、.braveでADA送金やNFT閲覧も可能に

### ✅ S2：.brave主導で置換圧力（15%）
新規ユーザーが.braveドメインに集中、ADA Handleの存在感が相対的に低下

### ✅ S1：片方の淘汰（5%）
技術更新停止または方向性のズレにより、片方が淘汰される

---

## 📝 統合所見

| テーマ     | 見解                                      |
| ------- | --------------------------------------- |
| カルダノらしさ | ADA HandleはUTxO+DID+CIP準拠の「純正UX革新型」     |
| 世界標準    | .braveはクロスチェーン＋ID＋Webという「次世代DNS志向」      |
| 競合か共存か  | 現状は補完関係。技術的には統合の可能性あり                   |
| DRep視点  | CardanoのVoltaire UX強化においてはADA Handleが優位 |

