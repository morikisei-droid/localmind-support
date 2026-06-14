---
title: おすすめモデル
---

# おすすめモデル（GGUF）

LocalMind で使える、**自由に使えるライセンス（Apache-2.0 / MIT）の軽量モデル**をまとめました。

> 最も簡単なのは、アプリ内の **「モデル管理 → おすすめモデルから選ぶ（アプリ内ダウンロード）」** です。下のリンクは、ブラウザから直接ダウンロードしたい場合のものです。

## 一覧

| モデル | サイズ | ライセンス | 特徴 | ダウンロード |
|---|---|---|---|---|
| **Qwen2.5 0.5B Instruct** | 約469MB | Apache-2.0 | 最軽量。動作確認・低スペック端末向け。日本語対応 | [GGUFを入手](https://huggingface.co/Qwen/Qwen2.5-0.5B-Instruct-GGUF/resolve/main/qwen2.5-0.5b-instruct-q4_k_m.gguf) |
| **Qwen2.5 1.5B Instruct**（おすすめ） | 約1.07GB | Apache-2.0 | 軽量で日本語が得意。多くのiPhoneで快適 | [GGUFを入手](https://huggingface.co/Qwen/Qwen2.5-1.5B-Instruct-GGUF/resolve/main/qwen2.5-1.5b-instruct-q4_k_m.gguf) |
| **SmolLM2 1.7B Instruct** | 約1.01GB | Apache-2.0 | 軽量・高速。英語中心 | [GGUFを入手](https://huggingface.co/bartowski/SmolLM2-1.7B-Instruct-GGUF/resolve/main/SmolLM2-1.7B-Instruct-Q4_K_M.gguf) |
| **Phi-3.5 mini Instruct** | 約2.28GB | MIT | 高品質。推論・コードに強い（要RAM多め） | [GGUFを入手](https://huggingface.co/bartowski/Phi-3.5-mini-instruct-GGUF/resolve/main/Phi-3.5-mini-instruct-Q4_K_M.gguf) |

## ブラウザから入れる手順

1. 上の「GGUFを入手」をタップしてダウンロード（端末の「ファイル」に保存されます）
2. 「ファイル」アプリで、ダウンロードした `.gguf` を **LocalMind** のフォルダに移動、または共有メニューから LocalMind を選択
3. LocalMind の「モデル管理」で自動的に取り込まれます（「GGUFをファイルから取り込む」からも選べます）

## ライセンスについて

- 掲載モデルはいずれも **Apache-2.0 または MIT** の寛容なライセンスです。配布元は [Hugging Face](https://huggingface.co/) で、各モデルのライセンスが適用されます。
- LocalMind はモデルを同梱・再配布しません。リンク先からユーザーご自身がダウンロードします。
- より多くのモデルは [Hugging Face（GGUF）](https://huggingface.co/models?library=gguf) から探せます。
