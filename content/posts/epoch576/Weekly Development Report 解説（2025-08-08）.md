---
title: "Weekly Development Report 解説（2025-08-08）"
date: 2025-08-14
epoch: 576
tags: [Cardano, WeeklyDevReport, Midnight, DRep, Hydra, Lace, Voltaire]
---

## 概要
2025年8月8日時点のCardano開発週報を、DRep視点とMidnightトークノミクスの関連性も踏まえて整理。エコシステム成長指標、主要ニュース、技術進展、ガバナンス動向を俯瞰し、NIGHT配布進行（Glacier Drop → Scavenger Mine）やウォレット・スケーリング機能との接点を明確化。

---

## 1. エコシステム状況
| 指標 | 最新値 | 前回比 | 意味合い |
|------|--------|--------|----------|
| 構築中プロジェクト数 | 2,005件 | — | Cardano上のDApp/サービス開発規模 |
| 委任済みウォレット数 | 134万 | 増加 | ガバナンス参加基盤拡大 |
| ネイティブトークン総数 | 1,087万 | — | マルチアセット利用の広がり |
| トークンポリシー数 | 219,442 | +0.23% | 発行者や規格の増加 |
| トランザクション総数 | 1億1,238万件 | — | オンチェーン活動活発化 |
| アクティブDRep数 | 989人 | +14人 | ガバナンス参加増加 |
| GitHubコミット数 | 358 | +2 | 開発貢献継続 |

---

## 2. 主なニュース
- Midnight Network、**Blockchain.comと提携**
- **Zenkō Protocol**、メタバースPaviaを買収
- **Wanchain**、Cardano–SUIブリッジ構築
- **IOG**、Rare EvoでHydra搭載自販機展示
- **Finest**、NMKR経由で銀トークン（fSLVR）発行

---

## 3. コア技術進展
- **Leiosプロトタイプ**、**LSM-tree統合**、**Peras最適化**、**KESエージェント統合**進行
- **cardano-node v.10.5.1**メインネットリリース
- 新リポジトリ **cardano-parameters** 公開（Blockfrost APIで日次更新）

---

## 4. スマートコントラクト
- Plutusケース分析の型拡張（unit, pair, data types対応）
- **UPLCベンチマーク**（Fibonacci計算）導入
- **Plinthコンパイラ**最適化（Bool直接マッピング、スクリプト軽量化）

---

## 5. ウォレット・サービス
- **Lace v.1.26**
  - DApp署名前にTxメタデータ表示（Ledger利用時のGlacier Drop登録可）
  - **NFTPrintLab**：ウォレット内NFTを物理プリント可能
  - Lace v2開発継続（Midnight対応、モバイル対応）

---

## 6. スケーリング（Hydra）
- Glacier Drop支援でパッチ連続リリース（最新v0.22.4）
- API負荷軽減（重複署名無視）、Txスタック不具合修正
- 新HTTPエンドポイント追加、部分ADAコミット対応
- 今後：部分ファンアウト実装検討、デポジット回復、Rare EvoでHydra Doom発表

---

## 7. ガバナンス（Voltaire）
- **Intersect予算 1,575万ADA** 承認
- **IOR予算 2,684万ADA** 承認
- DRep投票 + 憲法委員会承認で国庫引き出し

---

## 8. 教育
- Rare Evoでワークショップ実施
- 『Mastering Cardano』執筆進行
- **Cardano Days（9月26–27日＠ワイオミング大学）** 告知

---

## Midnightトークノミクス接続ポイント
- Hydra更新 & Lace改良 → **Glacier Drop請求の円滑化**
- Lace v.1.26 → **Scavenger MineやLost-and-Found請求基盤**
- Hydra自販機デモ → **DUST決済型DAppのUX実証**
- Leios・Peras最適化 → **将来的なMidnightスループット強化**

---

## 行動指針（DRep視点）
1. **Lace v.1.26環境整備**（Midnight請求・DApp対応）
2. **Hydra v0.22.4テスト**（安定性・性能検証）
3. **Scavenger Mine参加準備**（計算タスク対応）
4. 関連ガバナンス提案のウォッチ（Midnight予算・技術導入）

---

作成日時: 2025-08-14

