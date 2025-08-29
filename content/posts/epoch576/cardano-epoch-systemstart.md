---
title: Cardano Epoch計算とsystemStartの由来・ジェネシスファイル解説
date: 2025-08-14
epoch: 576
tags:
  - 観測記録
  - カルダノ
  - FBL
  - ADA
  - Epoch
  - systemStart
draft: false
---

## 1. EPOCHの計算式

Cardano Mainnet のエポック番号は、以下の式で求められる。

```
エポック番号 = floor( (対象日時 − systemStart) / エポック長 )
```

- **systemStart**: `2017-09-23T21:44:51Z`（ジェネシスブロック開始時刻）
- **エポック長**: 5日（432,000秒）
- **スロット秒数**: 1秒／スロット（Mainnet）

### JavaScriptによる計算例

```javascript
const systemStart = Date.parse("2017-09-23T21:44:51Z");
const EPOCH_LEN_MS = 5 * 24 * 60 * 60 * 1000;  // 432,000秒

function calculateEpoch(dateUtc) {
  return Math.floor((dateUtc.getTime() - systemStart) / EPOCH_LEN_MS);
}

// 例：2025-08-14 UTC のエポックを計算
const dt = Date.parse("2025-08-14T00:00:00Z");
console.log("Epoch:", calculateEpoch(new Date(dt)));
// => 576
```

---

## 2. systemStartの由来

`systemStart` は、Cardanoネットワークにおけるエポック0の開始時刻を定義する重要パラメータである。  
Shelleyジェネシスファイル内に記録され、メインネットの歴史的ローンチ時刻として固定されている。

- **技術的役割**: エポック計算の基準時刻（slot 0 の開始）
- **歴史的背景**: Byronメインネット稼働開始時刻に設定
- **秒数のズレ（21:45ではなく21:44:51）**: 起動処理やログ記録上の誤差、ブロック生成時刻の仕様による可能性

---

## 3. ジェネシスファイルの中身（抜粋例）

```jsonc
{
  "systemStart": "2017-09-23T21:44:51Z",
  "networkMagic": 764824073,
  "protocolParams": {
    "decentralisationParam": 0.5,
    "maxBlockBodySize": 65536,
    "maxTxSize": 16384
  },
  "epochLength": 432000,  // スロット数（5日）
  "slotLength": 1,        // 1秒／スロット
  "securityParam": 2160,
  "activeSlotsCoeff": 0.05
}
```

---

## 4. まとめ表

| 項目                  | 値・内容                                           |
|-----------------------|----------------------------------------------------|
| systemStart           | `2017-09-23T21:44:51Z`（ジェネシス開始時刻）        |
| エポック長             | 432,000秒（5日）                                   |
| スロット秒数           | 1秒／スロット                                      |
| 計算式                 | floor((対象日時 - systemStart) / 432000秒)          |
| 小さな秒数ズレの理由   | 起動処理・生成プロセスの技術的仕様による可能性      |
| エポック計算への影響   | 実用上ほぼ無視可能                                 |

---
作成日時: 2025-08-14
