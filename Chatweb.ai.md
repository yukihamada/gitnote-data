---
id: "019cffcf-08b8-7c11-ac0d-9b853198dfc4"
tags:
  - ai
  - rust
  - lambda
  - tier1
icon: "🤖"
aliases:
  - "Chatweb.ai"
---

# Chatweb.ai / teai.io

AIチャットプラットフォーム。同一Rustバイナリから2ブランド配信。
→ [[Yuki Hamada - プロジェクト全体像|全体像に戻る]]

## アーキテクチャ
- Rust (axum) on AWS Lambda ARM64 musl → [[インフラ全体マップ]]
- DynamoDB
- API Gateway (ap-northeast-1)

## ブランド分離
- サーバーサイド: `handle_root()` で25項目の文字列置換
- クライアントサイド: `IS_TEAI` フラグ

## ビルド
```bash
LAMBDA_FUNCTION_NAME=nanobot-prod ./infra/deploy-fast.sh
# 禁止: --target aarch64-unknown-linux-gnu
```

## 収益
- Stripe連携
- [[ENAI Token]]: 1 ENAI = 10 credits

## LLMバックエンド
- RunPod Nemotron 9B → Groq → Gemini (フォールバック)