---
id: "019cffcf-2349-7683-a3fa-fd0f651bbad6"
tags:
  - hardware
  - swift
  - rust
  - esp32
icon: "🎙️"
aliases:
  - "Koe音声入力"
---

# Koe

音声入力マルチプラットフォーム。→ [[Yuki Hamada - プロジェクト全体像|全体像]]

## 4コンポーネント
1. macOS (Swift) — Koe-swift/
2. Windows (Rust)
3. ESP32 デバイス — koe-device/
4. Web (koe.live)

## コンセプト
ハードウェアボタンで音声入力→リアルタイム文字起こし→任意アプリへ送信