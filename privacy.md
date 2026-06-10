---
title: プライバシーポリシー / Privacy Policy
permalink: /privacy/
---

# LocalMind プライバシーポリシー / Privacy Policy

---

# プライバシーポリシー（日本語）

**最終更新日 / 発効日：2026-06-10**

LocalMind（以下「本アプリ」）は、ユーザーが自ら入手したオープンソースの大規模言語モデル（GGUF 形式、llama.cpp）を、端末上で完全にオフラインで実行する iOS アプリです。本ポリシーは、本アプリがどのような情報を取り扱うか、何が端末内に留まり、何が外部に送信されるかを説明します。

本アプリの開発者・運営者（以下「当方」）は、本ポリシーに従って情報を取り扱います。

---

## 1. 基本方針：コンテンツは端末から出ません

本アプリの中核となる以下のデータは、**（後述「任意のWEB検索機能」をユーザーが明示的に有効化し検索クエリを送信する場合を除き）端末外へ送信されず、当方を含む第三者のサーバーへ送信・アップロード・保存されることはありません。** これらはすべてユーザーの端末内（SwiftData によるローカル保存）でのみ処理・保存されます。

- **ノート、フォルダ、ワークスペース、双方向リンクの内容**
- **チャットのプロンプト（入力）および AI の応答（出力）**（WEB検索を有効化して送信する検索クエリのみ例外。後述の「任意のWEB検索機能」参照）
- **オンデバイス RAG（検索拡張生成）のためのインデックス、埋め込み、参照されるノート本文**
- **ユーザーが import した LLM モデルファイル（GGUF）およびその出力**
- **ペルソナ（システムプロンプトのプリセット）の内容**
- **テーマ設定その他のアプリ内設定**

LLM の推論（生成）はすべて端末内の CPU/メモリ上で行われ、ネットワーク接続を必要としません。当方はこれらのコンテンツにアクセスできず、収集も行いません。

**モデルについて：** 本アプリはいかなるモデルも同梱・配布しません。ユーザーは外部ブラウザを通じて公式の配布元（例：Hugging Face）から GGUF ファイルを自ら入手します。各モデルのライセンス遵守はユーザーの責任となります。

---

## 1-2. 任意のWEB検索機能（既定でオフ）

本アプリには、モデルが自らの知識では不十分と判断した場合等に、ユーザーが手動で有効化できる任意のWEB検索機能があります。本機能は**既定で無効**であり、設定画面（インターネット検索）でユーザーが明示的にオンにした場合に限り動作します。

- 本機能を有効にして検索を実行すると、**ユーザーが入力した検索クエリ（質問文）またはそれに基づきモデルが生成した短い検索文字列のみ**が、選択した検索プロバイダ（既定：Wikipedia／提供元 Wikimedia Foundation）へ送信されます。
- 送信先プロバイダが受領するのは、当該**検索クエリ文字列**、通信に伴う**IPアドレス・通信メタデータ**のみです（既定のWikipediaはAPIキーやアカウントを要しません）。
- **ノート・フォルダ・双方向リンク・RAGで参照されるノート本文・ペルソナ・モデルファイルの内容、および組み立て済みのプロンプト全体は送信されません。** 送信対象は当該検索のためのクエリ文字列のみです。
- 既定プロバイダである Wikipedia（Wikimedia Foundation）の検索結果は CC BY-SA 4.0 で提供され、本アプリは出典を画面に表示します。取り扱いは Wikimedia のプライバシーポリシーに従います：https://foundation.wikimedia.org/wiki/Policy:Privacy_policy
- 本機能はいつでも設定画面で無効化できます。無効の間、いかなるクエリも外部送信されません。

## 2. 広告 SDK（Google AdMob）が収集・送信する情報

本アプリは無料で提供され、その費用を賄うため **Google AdMob** による広告を表示します（チャット・一覧画面のバナー、GGUF ロード時のアプリ起動広告、ユーザー操作による画面遷移時の頻度制限付きインタースティシャル、および 100% オプトイン方式のリワード広告）。

広告の配信・表示・測定・不正防止のため、**Google（AdMob／Google AdSense／関連する広告測定サービス）は、本アプリを通じてユーザーの端末から以下の情報を取得し、Google のサーバー（米国を含む国外）へ送信します。**

外部送信される情報（送信先：Google LLC、利用目的：広告配信・表示頻度の最適化・広告効果測定・不正防止）：

- **広告識別子（IDFA：Advertising Identifier。ATT で許可された場合のみ）**
- **ベンダー識別子（IDFV）その他の端末・アプリ識別子**
- **IP アドレス（これにより推定されるおおよその位置情報）**
- **端末情報（機種、OS バージョン、言語、タイムゾーン、画面情報、ネットワーク種別など）**
- **広告の表示・操作（インプレッション、タップ、視聴完了等）に関する情報**
- **おおよそのアプリ利用状況（広告枠の表示文脈に関する最小限の情報）**

これらの情報の取り扱いは Google のプライバシーポリシーに従います。
- Google プライバシーポリシー：https://policies.google.com/privacy
- Google が広告で情報を利用する方法：https://policies.google.com/technologies/partner-sites

**重要：** 上記で送信されるのは広告関連の識別子・技術情報のみであり、**第 1 章に記載したノート・プロンプト・RAG・モデルの内容は一切含まれません。**

本アプリはアナリティクス SDK（例：Firebase Analytics 等）やクラッシュレポート SDK による独自のユーザー追跡を行いません。当方が運営するサーバーは存在せず、当方がユーザーの個人データを直接収集・保有することはありません。

---

## 3. App Tracking Transparency（ATT）

iOS の **App Tracking Transparency** の要件に従い、本アプリは、広告識別子（IDFA）を用いた**トラッキング**を行う前に、システムの許可ダイアログを表示して同意を求めます。

- 許可しない場合でも本アプリは利用でき、広告は引き続き表示されますが、**パーソナライズされない（非追跡型の）広告**となります。
- 許可は、iOS の「設定 > プライバシーとセキュリティ > トラッキング」からいつでも変更できます。

---

## 4. EEA／英国の利用者向け：UMP・GDPR

欧州経済領域（EEA）、英国、スイスの利用者に対しては、**Google UMP（User Messaging Platform）による同意管理画面**を表示します。GDPR／UK GDPR に基づき、パーソナライズ広告等のために情報を利用する前に、利用者の**同意**を取得します。

- 同意しない場合は、**非パーソナライズ広告**または同意を要しない範囲での処理のみが行われます。
- 同意はアプリ内の設定（プライバシー設定／同意の管理）からいつでも変更・撤回できます。

**法的根拠（GDPR 第 6 条）：**
- パーソナライズ広告のための識別子の利用・送信：**同意（第 6 条 1 項 (a)）**
- 非パーソナライズ広告の配信、不正防止、広告の基本的な配信・測定：**正当な利益（第 6 条 1 項 (f)）**（適用法および同意要件が優先する範囲で）
- 課金（IAP）の処理：Apple との**契約の履行（第 6 条 1 項 (b)）**

EEA／英国の利用者は、アクセス・訂正・削除・処理の制限・異議申立て・データポータビリティ・同意撤回の権利を有します。当方はノート等のコンテンツを保有しないため、これらの権利は主に Google が処理する広告関連データに関して、Google に対して行使できます。監督機関へ苦情を申し立てる権利もあります。

---

## 5. 日本の利用者向け：個人情報保護法（APPI）および電気通信事業法（外部送信規律）

**個人情報保護法（APPI）について：**
当方は、当方が運営するサーバーで個人情報を直接収集・保有しません。広告に関連して送信される識別子等は Google が取得・処理し、Google が定めるプライバシーポリシーに従って取り扱われます。広告 ID 等が個人関連情報に該当する場合があり、その取り扱いは本ポリシーおよび Google のポリシーによります。

**電気通信事業法 第27条の12（外部送信規律）に基づく開示：**
本アプリは、利用者の端末に記録された情報を、以下のとおり外部（当方以外の第三者）へ送信します。

| 送信される情報 | 送信先 | 利用目的 |
|---|---|---|
| 広告識別子（IDFA、ATT 許可時） | Google LLC | 広告配信・表示・効果測定・最適化・不正防止 |
| ベンダー識別子（IDFV）・端末/アプリ識別子 | Google LLC | 同上 |
| IP アドレス | Google LLC | 同上（おおよその地域判定を含む） |
| 端末情報（機種・OS・言語・タイムゾーン・画面・ネットワーク種別等） | Google LLC | 広告の最適化・表示 |
| 広告の表示・操作情報（インプレッション・タップ・視聴完了等） | Google LLC | 広告効果測定・不正防止 |
| おおよそのアプリ利用文脈情報 | Google LLC | 広告配信の最適化 |

- 送信先である Google のプライバシーポリシー：https://policies.google.com/privacy
- ATT で許可しない場合、IDFA は送信されません。後述の広告除去 IAP を購入した場合、上記の広告目的の外部送信は停止します。
- **ノート、プロンプト、RAG、モデルの内容は上記のいずれにも含まれず、外部送信されません。**

---

## 6. データの保存期間

- **端末内データ（ノート、プロンプト、RAG、モデル、設定等）：** ユーザーが本アプリ内で削除するか、本アプリ／端末上のデータを削除するまで、ユーザーの端末内に保存されます。当方はこれらに対する保存期間を設定・管理しません。
- **広告関連データ：** Google が取得したデータの保存期間は、Google のプライバシーポリシーおよびデータ保持方針に従います。当方はこれを保有しません。

本アプリをアンインストールすると、端末内に保存されたすべてのアプリデータ（ノート、モデル等）は削除されます。

---

## 7. 子どもについて

本アプリの App Store 年齢レーティングは **17+** です。本アプリは子ども向けではなく、子どもを対象として設計・提供されていません。当方は 13 歳未満（または各国法が定める年齢未満）の子どもから、意図的に個人情報を収集しません。本アプリは「ユーザー自身が入手・実行する生成 AI」という性質上、出力に不適切・不正確な内容が含まれる可能性があります。

---

## 8. ユーザーの権利と選択

- **広告のパーソナライズの制御：** ATT（iOS 設定）および UMP（EEA／英国）を通じて、追跡・パーソナライズ広告を拒否できます。
- **広告の完全除去（IAP）：** 後述の買い切り型 IAP により、広告および広告ネットワークへの外部送信を停止できます（第 9 章）。
- **コンテンツの削除：** ノート等は本アプリ内でいつでも削除でき、アンインストールにより端末内データを消去できます。
- **アクセス・訂正・削除等の請求：** 広告関連データについては Google に対して権利を行使できます。本ポリシーに関するお問い合わせは下記連絡先までご連絡ください。

---

## 9. 買い切り型 IAP（広告除去）

本アプリは、約 **1,500 円（税込・地域により変動）** の**買い切り型アプリ内課金（サブスクリプションではありません）**を提供します。これを購入すると：

- **すべての広告が削除されます**（バナー、アプリ起動広告、インタースティシャル、リワード広告）。
- その結果、**Google AdMob による上記の広告目的の外部送信（IDFA・IDFV・IP・端末情報等）が停止します。**
- リワード広告で付与される各種ブースト（生成拡張等）が**恒久的に付与**されます。

購入処理は **Apple（App Store／StoreKit）**を通じて行われます。Apple は購入の処理のために必要な情報を取り扱います。当方はクレジットカード番号等の決済情報を受領・保有しません。Apple のプライバシーポリシー：https://www.apple.com/legal/privacy/

---

## 10. 第三者サービス

- **Google AdMob**（広告）：https://policies.google.com/privacy
- **Apple**（アプリ配信・課金）：https://www.apple.com/legal/privacy/
- **モデル配布元（例：Hugging Face）**：ユーザーが外部ブラウザでアクセスして GGUF を入手します。当該サイトの利用には各サイトのポリシーが適用されます。

---

## 11. データの国外移転

広告関連データは、Google により米国を含む日本国外のサーバーで処理される場合があります。これらの移転は Google の方針および適用される標準契約条項等の適切な保護措置に従って行われます。

---

## 12. セキュリティ

本アプリのコンテンツは端末内に保存され、ネットワーク送信されないため、外部からの傍受リスクは最小化されています。端末自体のセキュリティ（パスコード、生体認証、OS の更新等）の維持はユーザーの責任です。

---

## 13. 免責事項

LLM の出力の正確性は保証されません。本アプリは医療・法律・財務その他の専門的助言を提供するものではありません。出力の利用および各モデルのライセンス遵守は、ユーザーの責任となります。

---

## 14. 本ポリシーの変更

当方は、法令の変更やアプリ機能の変更に応じて本ポリシーを改定することがあります。重要な変更がある場合は、アプリ内またはストアの掲載情報を通じて通知します。改定後の継続利用をもって、変更への同意とみなします。

---

## 15. お問い合わせ

本ポリシーまたはプライバシーに関するお問い合わせは、以下までご連絡ください。
**連絡先：morikisei@gmail.com**

---
---

# Privacy Policy (English)

**Last updated / Effective date: 2026-06-10**

LocalMind ("the App") is an iOS application that runs user-supplied, open-source large language models (GGUF format via llama.cpp) fully offline on your device. This Privacy Policy explains what information the App handles, what stays on your device, and what is transmitted off your device.

The developer/operator of the App ("we," "us," "our") handles information in accordance with this Policy.

---

## 1. Core Principle: Your Content Never Leaves Your Device

The following core data is **never transmitted off your device** and is **never sent, uploaded, or stored on any server operated by us or any third party.** All of it is processed and stored exclusively on your device (locally, via SwiftData):

- **Notes, folders, workspaces, and bidirectional link content**
- **Chat prompts (your input) and AI responses (output)**
- **On-device RAG (Retrieval-Augmented Generation) indexes, embeddings, and referenced note content**
- **LLM model files (GGUF) you import, and their outputs**
- **Persona (system-prompt preset) content**
- **Theme and other in-app settings**

All LLM inference (generation) runs locally on your device's CPU/memory and requires no network connection. We cannot access and do not collect any of this content.

**About models:** The App does not bundle or distribute any model. You obtain GGUF files yourself from official sources (e.g., Hugging Face) via your external browser. Compliance with each model's license is your responsibility.

---

## 2. Information Collected and Transmitted by the Ad SDK (Google AdMob)

The App is provided free of charge. To support it, we display ads via **Google AdMob** (banners on chat and list screens, an app-open ad at GGUF load, frequency-capped interstitials on user-initiated transitions, and 100% opt-in rewarded ads).

To deliver, display, measure, and prevent fraud in advertising, **Google (AdMob / Google AdSense / related ad-measurement services) collects the following information from your device through the App and transmits it to Google's servers (including in countries outside your own, such as the United States).**

Information transmitted externally (recipient: Google LLC; purposes: ad delivery, frequency optimization, ad measurement, fraud prevention):

- **Advertising Identifier (IDFA — only if permitted via ATT)**
- **Identifier for Vendors (IDFV) and other device/app identifiers**
- **IP address (and the approximate location inferred from it)**
- **Device information (model, OS version, language, time zone, screen attributes, network type, etc.)**
- **Ad interaction data (impressions, taps, completed views, etc.)**
- **Approximate app usage (minimal context about the ad placement)**

This information is handled in accordance with Google's privacy policies:
- Google Privacy Policy: https://policies.google.com/privacy
- How Google uses information for advertising: https://policies.google.com/technologies/partner-sites

**Important:** Only advertising-related identifiers and technical information are transmitted. **None of the note, prompt, RAG, or model content described in Section 1 is ever included.**

The App does not use analytics SDKs (e.g., Firebase Analytics) or crash-reporting SDKs for its own user tracking. We operate no server of our own, and we do not directly collect or hold your personal data.

---

## 3. App Tracking Transparency (ATT)

In accordance with Apple's **App Tracking Transparency** requirements, the App presents the system permission prompt and requests your consent before any **tracking** using the Advertising Identifier (IDFA).

- If you do not allow tracking, you can still use the App and will still see ads, but they will be **non-personalized (non-tracking).**
- You can change your choice at any time in iOS **Settings > Privacy & Security > Tracking.**

---

## 4. For Users in the EEA / UK: UMP and GDPR

For users in the European Economic Area (EEA), the United Kingdom, and Switzerland, we present a **consent management interface via Google UMP (User Messaging Platform).** In accordance with the GDPR / UK GDPR, we obtain your **consent** before using information for purposes such as personalized advertising.

- If you do not consent, only **non-personalized advertising** or processing that does not require consent will occur.
- You can change or withdraw your consent at any time via the App's settings (Privacy settings / Manage consent).

**Legal bases (GDPR Article 6):**
- Use/transmission of identifiers for personalized advertising: **Consent (Art. 6(1)(a))**
- Non-personalized ad delivery, fraud prevention, and basic ad serving/measurement: **Legitimate interests (Art. 6(1)(f))** (to the extent permitted, where consent requirements do not override)
- Processing of the in-app purchase: **Performance of a contract with Apple (Art. 6(1)(b))**

EEA/UK users have the rights of access, rectification, erasure, restriction of processing, objection, data portability, and withdrawal of consent. Because we do not hold your note or other content, these rights apply mainly to advertising-related data processed by Google and may be exercised with Google. You also have the right to lodge a complaint with a supervisory authority.

---

## 5. For Users in Japan: APPI and the Telecommunications Business Act (External Transmission Rules)

**Act on the Protection of Personal Information (APPI):**
We do not directly collect or hold personal information on any server operated by us. Identifiers transmitted in connection with advertising are collected and processed by Google and handled in accordance with Google's privacy policy. Where advertising IDs may constitute "personally referable information," their handling is governed by this Policy and Google's policies.

**Disclosure under Article 27-12 of the Telecommunications Business Act (External Transmission Rules):**
The App transmits information stored on your device to external parties (third parties other than us) as follows:

| Information transmitted | Recipient | Purpose |
|---|---|---|
| Advertising Identifier (IDFA, when permitted via ATT) | Google LLC | Ad delivery, display, measurement, optimization, fraud prevention |
| IDFV / device/app identifiers | Google LLC | Same as above |
| IP address | Google LLC | Same as above (including approximate region detection) |
| Device information (model, OS, language, time zone, screen, network type, etc.) | Google LLC | Ad optimization and display |
| Ad interaction data (impressions, taps, completed views, etc.) | Google LLC | Ad measurement, fraud prevention |
| Approximate app usage context | Google LLC | Ad delivery optimization |

- Recipient Google's privacy policy: https://policies.google.com/privacy
- If you do not permit ATT, the IDFA is not transmitted. If you purchase the ad-removal IAP (below), the above external transmissions for advertising purposes cease.
- **Note, prompt, RAG, and model content is not included in any of the above and is never transmitted externally.**

---

## 6. Data Retention

- **On-device data (notes, prompts, RAG, models, settings, etc.):** Stored on your device until you delete it within the App or delete the App's/device's data. We do not set or manage a retention period for this data.
- **Advertising-related data:** Retention of data collected by Google is governed by Google's privacy and data-retention policies. We do not hold it.

Uninstalling the App removes all app data stored on your device (notes, models, etc.).

---

## 7. Children

The App's App Store age rating is **17+.** The App is not directed to children and is not designed or offered for children. We do not knowingly collect personal information from children under 13 (or the applicable age under local law). By its nature (generative AI that you obtain and run yourself), outputs may contain inappropriate or inaccurate content.

---

## 8. Your Rights and Choices

- **Control over ad personalization:** You can decline tracking and personalized ads via ATT (iOS Settings) and UMP (EEA/UK).
- **Complete ad removal (IAP):** A one-time in-app purchase stops ads and external transmission to the ad network (Section 9).
- **Deleting content:** You can delete notes and other content within the App at any time, and uninstalling erases on-device data.
- **Access, correction, deletion, etc.:** For advertising-related data, you may exercise your rights with Google. For questions about this Policy, contact us using the details below.

---

## 9. One-Time In-App Purchase (Ad Removal)

The App offers a **one-time in-app purchase (not a subscription)** of approximately **1,500 JPY** (tax included; price varies by region). When purchased:

- **All ads are removed** (banners, app-open ad, interstitials, rewarded ads).
- As a result, **Google AdMob's external transmissions for the advertising purposes described above (IDFA, IDFV, IP, device information, etc.) cease.**
- The boosts otherwise granted via rewarded ads (e.g., extended generation) are **granted permanently.**

The purchase is processed through **Apple (App Store / StoreKit).** Apple handles information necessary to process the purchase. We do not receive or hold payment details such as credit card numbers. Apple's Privacy Policy: https://www.apple.com/legal/privacy/

---

## 10. Third-Party Services

- **Google AdMob** (advertising): https://policies.google.com/privacy
- **Apple** (app distribution and billing): https://www.apple.com/legal/privacy/
- **Model sources (e.g., Hugging Face):** You access these via your external browser to obtain GGUF files. Each site's own policies apply to your use of it.

---

## 11. International Data Transfers

Advertising-related data may be processed by Google on servers outside your country, including in the United States. Such transfers are carried out in accordance with Google's practices and appropriate safeguards (such as Standard Contractual Clauses) where applicable.

---

## 12. Security

Because the App's content is stored on your device and not transmitted over the network, the risk of interception is minimized. You are responsible for maintaining the security of your device itself (passcode, biometrics, OS updates, etc.).

---

## 13. Disclaimers

The accuracy of LLM outputs is not guaranteed. The App does not provide professional medical, legal, financial, or other professional advice. You are responsible for your use of outputs and for compliance with each model's license.

---

## 14. Changes to This Policy

We may revise this Policy in response to changes in law or app functionality. If we make material changes, we will notify you through the App or the store listing. Your continued use after the revision constitutes acceptance of the changes.

---

## 15. Contact

For questions about this Policy or your privacy, please contact us:
**Contact: morikisei@gmail.com**
