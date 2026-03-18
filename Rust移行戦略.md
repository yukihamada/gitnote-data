---
id: "019cffcf-1bdd-79d1-ba16-4256d449b882"
tags:
  - strategy
  - rust
  - migration
icon: "🦀"
aliases:
  - "Rust移行戦略"
---

# Rust + Fly.io + SQLite 移行戦略

→ [[Yuki Hamada - プロジェクト全体像|全体像]]

## 共通パターン
- axum 0.7 + Askama + rusqlite (WAL) + Fly.io (nrt)

## 優先順位
1. enablerdao.com ✅ 完了
2. [[StayFlow]] 🎯 次 (1-2週、ROI最大)
3. [[JiuFlow]] (2-3週)
4. BANTO (2-3週)
5. [[SOLUNA]] (1週)

## メリット
- Supabase不要 → コスト削減
- パフォーマンス向上
- 統一スキル・統一デプロイ