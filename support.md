---
title: サポート / Support
permalink: /support/
---

# サポート / Support

## よくある質問 / FAQ

### Q. モデルはどうやって入手しますか？ / How do I get a model?

アプリにモデルは同梱されていません。Hugging Face などの公式配布元から **GGUF 形式**のモデルをダウンロードし、次のいずれかで取り込みます。

1. **Files アプリ / Finder 経由（推奨）**: ダウンロードした GGUF を本アプリの「書類」フォルダに置くと、自動で取り込まれます（コピー不要・即時）。
2. **アプリ内から**: モデル画面の「GGUFをファイルから取り込む」でファイルを選択します。

The app bundles no models. Download a **GGUF** model from an official source (e.g., Hugging Face) and either drop it into the app's Documents folder via the Files app / Finder (recommended — instant, no copy), or use "Import GGUF" on the Models screen.

### Q. どのくらいのサイズのモデルが動きますか？ / What model sizes work?

端末の RAM に依存します。モデル画面に「利用可能メモリ目安」が表示され、足りない場合は読み込み前に警告します。目安として 2〜4B クラスの Q4 量子化モデル（約1.5〜3GB）が快適です。

It depends on your device's RAM. The Models screen shows available memory and warns before loading anything too large. As a rule of thumb, 2–4B-class models at Q4 quantization (≈1.5–3GB) run comfortably.

### Q. データはどこに保存されますか？ / Where is my data stored?

すべて端末内です。ノート・チャット・モデル・添付・文字起こしが外部に送信されることはありません。詳細は[プライバシーポリシー](../privacy/)をご覧ください。

Everything stays on your device. See the [Privacy Policy](../privacy/) for details.

### Q. 音声の文字起こしはネットに繋がりますか？ / Does transcription use the network?

いいえ。Apple のオンデバイス音声認識のみを使用し、音声が端末外に送信されることはありません。

No. Transcription uses Apple's on-device speech recognition only.

### Q. 広告を消せますか？ / Can I remove ads?

設定画面の買い切り型「広告を除去」（約1,500円・サブスクリプションではありません）ですべての広告を削除できます。

A one-time "Remove Ads" purchase (≈ JPY 1,500, not a subscription) removes all ads.

## 不具合報告・お問い合わせ / Bug reports & contact

ご質問・不具合報告は下記までお寄せください。**端末名・iOS バージョン・使用モデル名（GGUF）**を添えていただけると解決が早くなります。

For questions or bug reports, please include your device, iOS version, and the GGUF model you were using.

**morikisei@gmail.com**
