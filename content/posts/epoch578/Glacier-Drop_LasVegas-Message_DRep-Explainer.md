---
title: ラスベガスからのメッセージ──Glacier Dropが開くカルダノの新章（DRep要点解説）
date: 2025-08-23
epoch: 578
tags:
  - Cardano
  - Midnight
  - GlacierDrop
  - Hydra
  - Governance
  - DRep
draft: false
---

# 概要（TL;DR）
- 「Glacier Drop」は *8エコシステム / 7ブロックチェーン* に跨る前例のない配布。2025-08-05に請求ポータル公開、**初週で1B（10億）NIGHT超**が請求済み。請求期間は**60日**で先着差なし。Hydraが実戦投入された。  
- Midnightの核は **NIGHT → DUST**。NIGHTは**24B**供給で“燃やす”のではなく**DUSTを継続生成**。DUSTは手数料支払いに使われ、**動的価格制御**で混雑に適応。  
- 配布は**三相**：①Glacier（60日）→②Scavenger Mine（30日）→③Lost & Found（4年）。**解凍360日＋グレース90日**で償還。  

> 出典：Midnight公式ブログ・白書・CHのX投稿（末尾「参考資料」参照）

---

## 重要ポイント（表）

| 項目 | 内容 |
|---|---|
| 公開メッセージ | Charles Hoskinson「Hello from Las Vegas」（Rare Evo期間中の配信） |
| クレーム開始 | 2025-08-05（Glacier Drop Claim Portal） |
| 初動実績 | 初週で **>1B NIGHT** 請求、2週で **1.5B NIGHT** 超 |
| 60日ルール | 期間内は**先着差なし**（急がなくてOK） |
| 技術基盤 | **Hydra**で大量請求を吸収（Head→最終確定） |
| スナップショット | 2025-06-11（直前時点）、8エコシステム対象 |
| トークン設計 | **NIGHT(24B)** が **DUST** を継続生成（NIGHT自体は消費されない） |
| 手数料モデル | 最低手数料＋混雑率×重量の**動的価格**（目標充足 ~50%） |
| 配布フェーズ | Glacier(60d) → Scavenger(30d) → Lost&Found(4y) |
| 解凍・償還 | **解凍360d** → **グレース90d**（合計450dの償還フェーズ） |

---

## 何が「新章」か（DRep視点）
1. **実需ベースの二重構造**：NIGHTは“発電機”、DUSTは“使用電力”。DUSTは**非譲渡・消耗・減衰**の性質で、手数料の**安定性**と**耐スパム**を両立。DAppの**スポンサー払い**（手数料肩代わり）も可能。  
2. **協調トークノミクス**：他チェーン/法定通貨に対して**価値を囲い込まない**設計。クロスチェーン到達性と実用性を最優先。  
3. **公正配布**：無料・広範・オープン。未請求分は**Scavenger**で再配分、**Lost & Found**で再チャンス。  
4. **Hydraの本番投入**：大量の請求を**Hydra Head**に流し、Cardanoのスケール設計を**現実の高負荷業務**で証明。  

---

## 技術の要点
- **供給と存在形態**：NIGHT総供給は**24B**。CardanoとMidnightの両レジャーでネイティブに存在し、**二重解放を防ぐ不変条件**の下で同期。  
- **ブリッジ**：初期は **Cardano→Midnight の片道**を優先、双方向は後続フェーズで段階的に。  
- **報酬設計**：ブロック報酬は**リザーブ**からの**予見可能な分配式**。満杯ブロック誘導でネットワーク効率を最適化。  
- **手数料**：最低手数料＋混雑率（直近ブロック参照）×重量。**目標ブロック充足 ~50%** を軸に価格を自動調整。  
- **配布タイムライン**：Glacier(60d)→Scavenger(30d)→Lost&Found(4y)。**解凍360d**→**償還グレース90d**→**計450d**で完結。  

---

## 実務メモ（請求・ウォレット）
- **ハードウェア差**（Ledger/Trezor/世代差）に伴う初期の不整合は想定内。ウォレット/取引所側の対応は**段階的拡充**。  
- **先着差なし**：60日ウィンドウ内の請求量・条件は同一。対応が整ってからでも不利にはならない。  

---

## リスクと論点
- **UX/互換性摩擦**：ハードウェア実装差・取引所対応の遅れは短期的な摩擦要因。  
- **規制接合**：DUSTの“合理的プライバシー”は規制整合を志向するが、国別の運用差は残る。  
- **ブリッジ方向**：片道設計の期間中は流動性設計に留意。  
- **需給ショック**：解凍期（360d）における流動化でボラが高まる可能性。  

---

## 5段階シナリオ分析（S5=最良→S1=最悪、確率はCGTA推定）

| シナリオ | 叙述 | 主要ドライバー | 確率 |
|---|---|---|---:|
| **S5 大成功** | Hydra活用が定着。DAppの**スポンサー払い**普及、RWA/RegTechがMidnight採用。“業界標準”へ。 | 初週>1B勢い、協調トークノミクスの実装速度、規制とのソフトランディング | **25%** |
| **S4 堅調拡大** | 60日請求→解凍→Scavengerで裾野拡大。手数料の安定が評価、RWAは試験導入。 | ウォレット/取引所整備、解凍期の需給吸収 | **35%** |
| **S3 ベースライン** | 技術は順調だがUX摩擦（HW/取引所）と片道ブリッジがネック。採用は緩やか。 | 実装差対応の遅延、双方向ブリッジ待ち | **25%** |
| **S2 失速** | 配布後のDApp不足・RWA停滞。市場ボラで外野が萎む。 | “殺しアプリ”不足、規制不確実性 | **10%** |
| **S1 つまずき** | 重大なセキュリティ/ブリッジ事故や規制ショックで停止・再設計。 | 仕様外ブリッジ事故、規制差し止め | **5%** |

---

## DRepとしての当面アクション
- **情報整備**：コミュニティ向け「請求手順・対応ウォレット・詰まりやすい点」テンプレを更新（**60日/先着差なし**を強調）。  
- **KPI観測**：①請求件数・額、②ウォレット/取引所対応数、③**スポンサー払い採用DApp数**、④解凍期のオンチェーン活動量（手数料安定性）。  
- **提言準備**：Hydra商用活用と **RWA/RegTech** の進捗をCatalystや予算ガバナンスの議題に接続する説明資料を作成。  

---

## 参考資料（一次情報中心）
- Midnight公式：**The tokenomics powering Midnight network**（白書紹介, 2025-06-25）  
  https://midnight.network/blog/the-tokenomics-powering-midnight-network
- 白書PDF：**Midnight Tokenomics and Incentives Whitepaper**（v1.02, 2025-06）  
  https://45047878.fs1.hubspotusercontent-na1.net/hubfs/45047878/Midnight-Tokenomics-And-Incentives-Whitepaper.pdf
- Glacier Drop：**Claim Portal Open**（2025-08-05）  
  https://midnight.network/blog/glacier-drop-claim-portal-now-open
- Glacier Drop：**One billion NIGHT tokens claimed after first week**（2025-08-12）  
  https://midnight.network/blog/one-billion-night-tokens-claimed
- State of the Network - August 2025（2週で**1.5B**請求言及）  
  https://midnight.network/blog/state-of-the-network-august-2025
- CH（X）：**Hello from Las Vegas**（2025-08-06）  
  https://x.com/IOHK_Charles/status/1953138760281145678
- CH（X）：**Hydraで動いている**言及（2025-08-07）  
  https://x.com/IOHK_Charles/status/1952815671034954064
- スナップショット詳細（例・XRPパラメータ掲載ページの一例）  
  https://www.midnight.gd/news/getting-ready-for-glacier-drop

---

**作成者**：BWtake & CGTA（DRep解説版）  
**作成日時**：2025-08-23 22:54 UTC+09:00
