---
title: L1_Blockchain_Technical_Comparison_Sui_Aptos_Solana_Cardano (1)
date: 2025-05-03
epoch: 555
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

# 技術基盤から見たL1ブロックチェーン比較表（2025年版）

## 🔍 技術比較表：Sui / Aptos / Solana / Cardano

| 観点/チェーン | **Sui** | **Aptos** | **Solana** | **Cardano** |
|--------------|---------|-----------|-------------|--------------|
| **並列処理アプローチ** | オブジェクトベース並列処理（単独状態のTxは完全並列） | Block-STMによる楽観的並列処理（衝突検出・再実行） | Sealevelによる明示的並列処理（スマコン側で制御） | EUTXOモデルに基づく並列性（Hydraで並列化強化） |
| **合意アルゴリズム** | Narwhal & Bullshark（DAG + Byzantine Consistent Broadcast） | AptosBFT（改良HotStuff） | Tower BFT（PoH + BFTの組み合わせ） | Ouroboros PoS系（Praos → Genesis → Leios） |
| **スマートコントラクト実行環境** | Move VM（オブジェクト志向） | Move VM（モジュール志向） | Sealevel + LLVM系VM（Rust/Cベース） | Plutus Core（Haskell/EUTXO）＋Marlowe |
| **状態データ構造** | Versioned Object Store（高速な状態トラッキング） | Jellyfish Merkle Tree（効率的な階層構造） | アカウントモデル（フラット構造） | EUTXO + Sparse Merkle Tree（フォームな検証可能性重視） |
| **ノード設計とスケーラビリティ** | 低レイテンシ志向。検証ノード分離可能だが未成熟 | 実行/検証/ストレージを並列分離。スケーラブルな構成 | モノリシックで高速。Firedancerで多クライアント化進行中 | 実行・検証がUTXOで分離可能。MithrilやHydraにより拡張へ |

## 🔧 解説：特徴的な技術差分

- **Sui vs Aptos**：並列処理に強みを持つ点では共通だが、Suiは「状態の独立性」を使ったオブジェクト処理に特化。Aptosはより汎用的なトランザクションを並列処理できるBlock-STMを採用。
- **Solana**：並列処理は最も強力だが、スマートコントラクト開発者が排他制御を意識する必要あり。Firedancerにより単一クライアント依存から脱却中。
- **Cardano**：EUTXOモデルにより構造的に並列性を実現。Hydra（状態チャネル）やLeios（三層ブロック）により並列実行が可能に進化中。

## 🏁 総括：技術優位性の傾向

| 技術軸 | 最も優れるチェーン | 補足 |
|--------|-------------------|------|
| 並列処理 | Aptos（Block-STM） or Sui（オブジェクト） | 汎用性ではAptos、特化性ではSui |
| 合意アルゴリズム | Cardano（Ouroboros Genesis/Leios） | 数学的厳密性・省電力性で優れる |
| 実行環境 | Solana（Sealevel） | 処理速度最速だが開発は難しい |
| 状態管理 | Cardano（EUTXO + SMT） | フォーマル検証と安全性に優れる |
| ノード拡張性 | Aptos or Cardano | Aptosはパイプライン処理、CardanoはMithril等で拡張中 |

---

📅 この比較表は 2025年05月03日 03:40（JST）作成 に作成されました。
