---
title: AdaStat.net 使い方完全ガイド
date: 2025-08-22T13:00:00+09:00
epoch: 577
draft: false
tags:
  - Cardano
  - Explorer
  - AdaStat
  - SPO
  - DRep
  - FBL-Tools
categories:
  - Tools
  - Cardano
summary: 独立系Cardanoブロックチェーン・エクスプローラー AdaStat.net の特徴と実務フロー。トランザクション確認、ステーキング報酬追跡、プール比較、トークン調査、オンチェーン・ガバナンス監視、API活用まで。
---

## 0. 要約（3行）
- **AdaStat.net** は、ブロック／TX／アカウント（ステーク鍵）／プール／トークン／エポック／スロット／ガバナンスを横断して追跡できる独立系エクスプローラー。APIも公開。 :contentReference[oaicite:0]{index=0}  
- **強み**：履歴の深掘り（報酬・デリゲーション・作成ブロック等）、強力な**プール・フィルタ**、**カスタム・チャートメーカー**。 :contentReference[oaicite:1]{index=1}  
- **FBL実務**：①TX確認→②報酬追跡→③プール比較→④トークン調査→⑤ガバナンス監視→⑥API導入の順で定着させる。

---

## 1. AdaStat とは？（何ができるか）
- **総合エクスプローラー**：ブロック、トランザクション、プール、アドレス／アカウント（stake key）、エポック、スロット、トークン等を提供。トップの検索から横断検索が可能。 :contentReference[oaicite:2]{index=2}
- **差別化ポイント**  
  - アカウント／プールの**履歴**（アクティブ・エポック、作成ブロック、デリゲーション、**ステーキング報酬**など）を一望。 :contentReference[oaicite:3]{index=3}  
  - **プール絞り込み**（プレッジ、デリゲータ数、ステーク量 など）と**チャート作成**ツール。 :contentReference[oaicite:4]{index=4}  
  - **無料API**で主要データにアクセス（エポック／ブロック／TX／アカウント／プール／トークン等）。 :contentReference[oaicite:5]{index=5}  
  - **ガバナンスアクション**（提出・批准・施行・失効など）専用ページ。 :contentReference[oaicite:6]{index=6}

---

## 2. 画面ナビ（クイックリンク）
| セクション | URL | 主な用途 | 典型シーン |
|---|---|---|---|
| Blocks | /blocks | 最新・過去ブロックの確認 | TXがどのブロックに入ったか追う :contentReference[oaicite:7]{index=7} |
| Stake Pools | /pools | プール一覧と詳細、各種フィルタ | 委任先の選定、SPOの自己監視 :contentReference[oaicite:8]{index=8} |
| Accounts | /accounts | ステーキングアカウント（stake key）情報 | ライブステーク、報酬履歴の確認 :contentReference[oaicite:9]{index=9} |
| Tokens | /tokens | ネイティブトークンの一覧・詳細 | Policy確認・資産調査 :contentReference[oaicite:10]{index=10} |
| Governances | /governances | オンチェーン・ガバナンス一覧 | 提出→批准→施行のトラッキング :contentReference[oaicite:11]{index=11} |
| About | /about | 概要・特徴 | 機能把握、履歴閲覧の考え方 :contentReference[oaicite:12]{index=12} |

> 例：Accountsページのサンプルでは、Live stake/Tx回数/最終活動日時などが確認できる。 :contentReference[oaicite:13]{index=13}

---

## 3. 実務フロー（手順書）

### 3.1 トランザクション（TX）を確認する
1) 画面上部の検索に**TXハッシュ**を貼り付け → TX詳細へ遷移。  
2) **ブロック番号／エポック／入出力**を確認し、転送完了を検証。  
3) 必要に応じて関連アドレスやアカウントを辿る（階層ナビ）。  
*根拠：TX/ブロック横断閲覧の提供。* :contentReference[oaicite:14]{index=14}

### 3.2 ステーキング報酬／委任履歴を追う
1) **stake key**（`stake1...`）または**アドレス**を検索。  
2) Accounts詳細で**Live stake**、過去の**報酬／委任**などを確認。  
3) エポック推移で「委任切替」「報酬日の前後」を把握。  
*根拠：アカウント履歴（デリゲーション・報酬等）閲覧に対応。* :contentReference[oaicite:15]{index=15}

### 3.3 プールを比較し、最適な委任先を選ぶ
1) **Stake Pools**へ → 右側の**フィルタ**で「プレッジ」「デリゲータ数」「ステーク量」など条件を入力。  
2) プール詳細で**稼働履歴（作成ブロック等）**や手数料設定を確認。  
3) ウォッチ用途には**Telegram通知ボット**も利用可能（報酬・作成ブロック・パラメータ変更など）。  
*根拠：強力なプールフィルタ／通知ボットの存在。* :contentReference[oaicite:16]{index=16}

### 3.4 トークン（ネイティブ資産）を調査する
1) **Tokens**で銘柄名や**Policy ID**から検索。  
2) 作成日時、流通状況など**個別ページ**で把握。  
*根拠：トークン一覧・個別詳細提供。* :contentReference[oaicite:17]{index=17}

### 3.5 オンチェーン・ガバナンスを監視する（DRep向け）
1) **Governances**でアクション一覧（提出・批准・施行 ほか）を俯瞰。  
2) 重要案件は**Cardanoscanの GovActions**等と**相互参照**して投票状況を確認。  
*根拠：AdaStatのガバナンス一覧、CardanoscanのGovActions提供。* :contentReference[oaicite:18]{index=18}

### 3.6 APIで自動化（研究・分析向け）
- 入口：**https://api.adastat.net/**（ブロック／TX／アカウント／プール／トークン等）。自前のダッシュボードやFBLデータパイプラインに接続可能。 :contentReference[oaicite:19]{index=19}  
- テストネット対応やオープンソース化に関する提案・進捗は**Project Catalyst**の公開ページで確認。 :contentReference[oaicite:20]{index=20}

---

## 4. 使いどころ早見表（FBL視点）

| ユースケース | AdaStat が得意な理由 | 代替・補完 |
|---|---|---|
| **TX完了確認** | ブロックとTXの横断が早い | — |
| **委任・報酬の時系列チェック** | アカウント履歴の可視化（報酬・委任） | — :contentReference[oaicite:21]{index=21} |
| **委任先の選定（SPO比較）** | 強力なプール絞り込みと詳細ページ | Pool.pmの**ビジュアル把握**と併用すると直感的（リアルタイム可視化に強み） :contentReference[oaicite:22]{index=22} |
| **トークン調査** | トークン一覧・個別詳細ページが豊富 | Cardanoscanのトークン一覧も参考に補完 :contentReference[oaicite:23]{index=23} |
| **ガバナンス監視** | ガバナンス専用リスト（提出→施行） | CardanoscanのGovActionsで投票内訳を比較 :contentReference[oaicite:24]{index=24} |

---

## 5. 5段階シナリオ分析（導入→高度活用）
1) **S1: ビギナー** — 送金の着金確認をTXページで行う。  
2) **S2: デリゲータ** — Accountsで報酬サイクルを把握し、Poolsで手数料や稼働状況を比較。  
3) **S3: SPO** — プール詳細＋フィルタで自プールと競合を継続監視。重要イベントは**Telegram通知**を設定。 :contentReference[oaicite:25]{index=25}  
4) **S4: DRep/ガバナンス担当** — Governancesで案件を常時トラッキングし、投票状況を外部（Cardanoscan）でクロスチェック。 :contentReference[oaicite:26]{index=26}  
5) **S5: リサーチャ／データ担当** — **AdaStat API**で時系列データを吸い上げ、独自の可視化・検証を行う。 :contentReference[oaicite:27]{index=27}

---

## 6. 将来展望（Road-to-Open & Testnet対応）
- AdaStatは**オープンソース化やテストネット対応**を進める提案を複数回提出・実装しており、**APIの可用性拡大**や**UI/UX改善**を継続。FBLの長期的なデータ基盤として相性が良い。 :contentReference[oaicite:28]{index=28}

---

## 7. 付録：競合／補完ツールとの簡易比較

| 項目 | AdaStat | Cardanoscan | Pool.pm |
|---|---|---|---|
| 総合探索（ブロック/Tx/アカウント/プール/トークン） | ✅ | ✅ | 部分（可視化特化） :contentReference[oaicite:29]{index=29} |
| プール**高度フィルタ** | ✅（プレッジ/デリゲータ/ステーク等） :contentReference[oaicite:30]{index=30} | ✅（一覧・諸指標） :contentReference[oaicite:31]{index=31} | ビジュアル重視（直感探索） :contentReference[oaicite:32]{index=32} |
| **ガバナンス**ページ | ✅（一覧） :contentReference[oaicite:33]{index=33} | ✅（GovActions/投票内訳） :contentReference[oaicite:34]{index=34} | — |
| **API公開** | ✅（無料API） :contentReference[oaicite:35]{index=35} | （公知UIは充実） | — |
| **チャートメーカー** | ✅（独自機能） :contentReference[oaicite:36]{index=36} | — | — |
| **通知** | Telegramボット（報酬/ブロック/変更） :contentReference[oaicite:37]{index=37} | — | — |
| 強みまとめ | 横断・履歴深掘りとAPI | 豊富なUIと広いカバレッジ | リアルタイム可視化・NFTに強み :contentReference[oaicite:38]{index=38} |

---

## 8. よくある質問（FAQ）
**Q1. DaedalusやLaceの履歴と数値がわずかに違う？**  
→ 同期タイミングや集計条件で差が出る場合あり。複数ソースで相互参照を。  

**Q2. トークンの危険判定はしてくれる？**  
→ エクスプローラーは**事実の表示**が中心。銘柄の正当性は**公式発表やコミュニティ情報**で確認を。  

**Q3. テストネットも見たい**  
→ AdaStatは**Pre-prod/Preview**対応とAPI公開を進めた提案あり。稼働状況は提案ページで最新を確認。 :contentReference[oaicite:39]{index=39}

---

## 9. 参考資料（公式・一次情報）
- AdaStat.net トップ／概要／主要ページ：トップ、About、Blocks、Pools、Accounts、Tokens、Governances、API。 :contentReference[oaicite:40]{index=40}  
- Cardano.org 開発者ポータルの**Adastatインタビュー**（チャートメーカー・プールフィルタの言及）。 :contentReference[oaicite:41]{index=41}  
- プール・ビジュアル補完：**pool.pm**（リアルタイム可視化）。 :contentReference[oaicite:42]{index=42}  
- Cardanoscan の**GovActions**（投票内訳など）。 :contentReference[oaicite:43]{index=43}  
- Catalyst提案（テストネット対応、オープンソース化、再起動プロジェクト等）。 :contentReference[oaicite:44]{index=44}


---

**作成日時**：2025-08-22