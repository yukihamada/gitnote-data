---
id: "019cffcf-1485-7683-b1ec-60d9d70aad07"
tags:
  - ios
  - swift
  - p2p
  - solana
  - tier1
icon: "✨"
aliases:
  - "Elio P2P推論"
---

# Elio

iOS向けP2P分散AI推論アプリ。→ [[Yuki Hamada - プロジェクト全体像|全体像]]

## P2PInference (2,920行 Swift)
- **EBR Token Gate**: Solana, [[ENAI Token]] mint
- **PII Filter**: 7カテゴリ、3レベル
- **Distributed Query Manager**: クエリ分散・集約
- **Ledger Server**: port 8766, Bonjour

## DePIN
- オンチェーンリワード: `/api/v1/depin/report`