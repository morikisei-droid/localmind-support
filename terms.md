---
title: 利用規約 / Terms of Use
permalink: /terms/
---

# LocalMind 利用規約およびエンドユーザー免責事項 / Terms of Use and End-User Disclaimer

**最終更新日 / Last updated: 2026-06-03**

---

## 日本語版（Japanese）

> 本書は、本アプリ「LocalMind」（以下「本アプリ」）の利用規約および免責事項です。オンボーディング画面の「同意する」操作は、本書全体への同意を意味します。本アプリを利用される前に、必ず本書をお読みください。本アプリをインストール、起動、または利用した時点で、利用者は本書の各条項に同意したものとみなされます。同意いただけない場合は、本アプリを利用しないでください。

### 1. 定義

- 「本アプリ」とは、LocalMind（iOSアプリケーション）およびこれに付随する一切のソフトウェア・ドキュメントをいいます。
- 「提供者」とは、本アプリの開発・配信を行う者をいいます。
- 「利用者」とは、本アプリをインストール・利用する個人または団体をいいます。
- 「モデル」とは、利用者が外部から取得して本アプリに読み込ませるGGUF形式等のオープンソース大規模言語モデル（LLM）の重みファイルをいいます。
- 「出力」とは、本アプリ上で利用者が読み込んだモデルがオンデバイスで生成したテキスト等をいいます。
- 「ノートコンテンツ」とは、利用者が本アプリ内のノート・フォルダ・ワークスペース機能で作成・編集する情報をいいます。

### 2. 本アプリの性質

2.1 本アプリは、iOS 17以降を対象とし、SwiftUI / SwiftDataで構築されたオンデバイスAIアプリです。利用者自身が取得したオープンソースLLM（GGUF / llama.cpp）を**完全にオフラインで端末上で実行**します。

2.2 本アプリは、Obsidianに類似した階層型ノートシステム（ワークスペース＞フォルダ＞ノート、双方向リンク）およびオンデバイスRAG（検索拡張生成）機能を提供します。

2.3 **本アプリは、いかなるLLMモデルも同梱・配布しません。** 本アプリは、Hugging Face等の公式配布元への外部ブラウザリンクを提供するのみであり、モデルの取得・ダウンロードは利用者自身の責任と判断において行われます。

2.4 推論エンジンはアプリに同梱されたバイナリであり、動的なコードのダウンロードや実行は行いません。GGUFファイルは実行コードではなく、データ（重み）として扱われます。

### 3. モデルライセンスに関する利用者の責任

3.1 利用者が本アプリに読み込む各モデルには、それぞれ固有のライセンス（例：Llama Community License、Apache-2.0、MIT、Gemma Terms of Use 等）が適用されます。

3.2 **各モデルのライセンス条項を確認し、これを遵守する責任は、すべて利用者にあります。** これには、商用利用の可否、再配布の制限、利用許諾範囲、帰属表示義務、利用制限条項（acceptable use policy）等が含まれますが、これらに限られません。

3.3 提供者は、利用者によるモデルの取得・利用・ライセンス遵守について一切の責任を負いません。利用者がモデルのライセンスに違反した場合の一切の結果は、利用者が負うものとします。

### 4. 出力に関する免責（正確性の不保証）

4.1 **本アプリの出力の正確性、完全性、信頼性、最新性、特定目的への適合性について、提供者は一切保証しません。** 大規模言語モデルは、事実と異なる情報（いわゆる「ハルシネーション」）を生成することがあります。

4.2 出力の品質は、利用者が選択したモデル、設定、入力内容、端末性能等に大きく依存します。

4.3 利用者は、出力をそのまま信頼せず、重要な判断を行う前に必ず独立した情報源で検証する責任を負います。

### 5. 専門的助言の不提供

5.1 **本アプリおよびその出力は、医療・法律・財務・税務・その他の専門的助言を構成するものではなく、これらに代わるものでもありません。**

5.2 健康、法律、金融、投資、税務その他専門的判断を要する事項については、必ず有資格の専門家にご相談ください。

5.3 提供者は、利用者が出力を専門的助言として用いたことに起因する一切の損害について責任を負いません。

### 6. 許容される利用（アクセプタブルユース）

6.1 利用者は、本アプリおよびオンデバイスで生成された出力を、適用される法令を遵守して利用するものとします。

6.2 利用者は、以下の行為を行ってはなりません。

- 違法な目的での利用、または第三者の権利（知的財産権、プライバシー権、肖像権等）を侵害する行為
- 他者に対する嫌がらせ、脅迫、誹謗中傷、差別、ヘイトスピーチの生成・流布
- マルウェア、フィッシング、詐欺、その他有害なコンテンツの生成
- 児童の性的搾取に関するコンテンツその他法令で禁止されるコンテンツの生成
- 各モデルのライセンスまたは利用ポリシーに違反する利用
- 本アプリのリバースエンジニアリング（適用法で認められる範囲を除く）、不正な改変、または本アプリの安全機構（RAMセーフな単一モデル読み込み制御等）の回避

6.3 出力は利用者の端末上でローカルに生成されます。生成された出力の内容、保存、共有、公開、二次利用について、その責任はすべて利用者にあります。

### 7. プライバシーと広告

7.1 **ノート・プロンプト・RAGの各コンテンツは、利用者の端末外に送信されません。** モデルの推論は完全にオンデバイスで行われます。

7.2 本アプリは無料で提供され、Google AdMobによる広告を表示します。広告（バナー、アプリ起動時広告、頻度制限付きインタースティシャル、完全オプトインのリワード広告）は、デバイス識別子等を送信する場合があります。

7.3 利用者には、AppTrackingTransparency（ATT）による許諾、ならびにEEA/英国の利用者に対するUMP（同意管理プラットフォーム）による同意取得を行います。日本の改正電気通信事業法に基づく外部送信に関する情報の開示も別途行います。

7.4 広告およびプライバシーの詳細は、本アプリ内のプライバシーポリシーをご参照ください。

### 8. アプリ内課金（IAP）および広告に関する条件

8.1 本アプリは、約1,500円（税込、価格はApp Storeの表示および為替により変動し得ます）の**買い切り型（一回限り）アプリ内課金**を提供します。サブスクリプション（定期購読）はありません。

8.2 当該IAPを購入すると、**すべての広告が除去**され、リワード広告で得られるブースト（延長生成等）が**恒久的に付与**されます。

8.3 リワード広告は100%オプトインであり、視聴により延長生成ブースト、24時間広告非表示パス、またはコスメティック（外観カスタマイズ）等の特典が付与されます。

8.4 IAPの決済、課金、返金は、Appleの定めるApp Storeの規約および手続きに従います。返金はAppleの規定に準じ、提供者が直接返金を行うことはできません。

8.5 IAPで付与される特典は、当該端末・Apple IDに紐づき、譲渡できません。Appleの「購入の復元」機能により再取得が可能な場合があります。

### 9. 無保証

9.1 本アプリは、**現状有姿（"AS IS"）および提供可能な範囲（"AS AVAILABLE"）**で提供されます。

9.2 提供者は、明示・黙示を問わず、商品性、特定目的への適合性、権利非侵害、エラーや中断のないこと、出力の正確性を含む一切の保証を行いません（適用法で除外が認められない範囲を除く）。

### 10. 責任の制限

10.1 適用法で認められる最大限の範囲において、提供者は、本アプリまたは出力の利用・利用不能に起因または関連して生じる、間接損害、付随的損害、特別損害、結果的損害、懲罰的損害、逸失利益、データの喪失、信用の毀損について、一切責任を負いません。

10.2 適用法で認められる最大限の範囲において、本アプリに関する提供者の累積的な賠償責任の総額は、利用者が本アプリに関して過去12か月間に提供者へ実際に支払った金額（無料利用の場合は0円）を上限とします。

10.3 法域によっては、黙示的保証の除外や付随的・結果的損害の制限が認められない場合があります。その場合、上記の制限は当該利用者に適用されない範囲で限定的に解釈されます。本条は、消費者契約法その他の強行法規により消費者に認められる権利を制限するものではありません。

### 11. 第三者サービス

本アプリは、Google AdMob、Apple App Store / StoreKit、ならびに利用者が選択するモデル配布元（Hugging Face等）といった第三者サービスを利用または参照します。これら第三者サービスには、それぞれの規約およびプライバシーポリシーが適用され、提供者はその内容について責任を負いません。

### 12. 年齢制限

本アプリのApp Store年齢区分は**17歳以上**です。利用者は、本アプリを利用するために必要な年齢に達していること、および居住地の法令上、本書に同意する法的能力を有することを表明・保証します。

### 13. 規約の変更

提供者は、本書を随時改定することができます。重要な変更を行う場合は、アプリ内での告知等、合理的な方法で通知します。改定後に本アプリを継続して利用した場合、改定後の規約に同意したものとみなされます。

### 14. 契約終了

利用者が本書に違反した場合、本書に基づく利用者の権利は自動的に終了します。利用者は、いつでも本アプリをアンインストールすることで利用を終了できます。第3条、第4条、第5条、第9条から第11条、第15条の規定は、契約終了後も存続します。

### 15. 準拠法および管轄

15.1 本書は、**日本法**に準拠し、これに従って解釈されます。

15.2 本書に起因または関連する一切の紛争については、**東京地方裁判所**を第一審の専属的合意管轄裁判所とします。

15.3 本条は、利用者が消費者として有する強行法規上の権利を妨げるものではありません。

### 16. お問い合わせ

本書に関するお問い合わせは、以下までご連絡ください。
**連絡先 / Contact: morikisei@gmail.com**

---

## English Version

> This document constitutes the Terms of Use and End-User Disclaimer for the "LocalMind" application (the "App"). Tapping "I Agree" during onboarding signifies your acceptance of this entire document. Please read it carefully before using the App. By installing, launching, or using the App, you agree to be bound by these terms. If you do not agree, do not use the App. In the event of any discrepancy between the Japanese and English versions, the **Japanese version shall prevail**.

### 1. Definitions

- "App" means LocalMind (the iOS application) and all accompanying software and documentation.
- "Provider" means the party that develops and distributes the App.
- "User" means the individual or entity that installs and uses the App.
- "Model" means an open-source large language model (LLM) weight file (e.g., GGUF format) that the User obtains from external sources and loads into the App.
- "Output" means text and other content generated on-device by a Model that the User has loaded into the App.
- "Note Content" means information created or edited by the User within the App's note, folder, and workspace features.

### 2. Nature of the App

2.1 The App targets iOS 17 and later, is built with SwiftUI / SwiftData, and is an on-device AI application. It runs open-source LLMs (GGUF / llama.cpp) **fully offline on the User's device**, using Models that the User obtains independently.

2.2 The App provides an Obsidian-like hierarchical note system (Workspace > Folder > Note, with bidirectional links) and on-device RAG (Retrieval-Augmented Generation).

2.3 **The App bundles and distributes no LLM Models whatsoever.** The App merely provides external browser links to official distribution sources (such as Hugging Face). The acquisition and download of any Model is performed solely at the User's own discretion and responsibility.

2.4 The inference engine is a binary bundled within the App. The App performs no dynamic download or execution of code. GGUF files are treated as data (weights), not as executable code.

### 3. User Responsibility for Model Licenses

3.1 Each Model the User loads into the App is subject to its own license (e.g., the Llama Community License, Apache-2.0, MIT, the Gemma Terms of Use, etc.).

3.2 **The User is solely responsible for reviewing and complying with the license terms of EACH Model.** This includes, without limitation, restrictions on commercial use, redistribution limitations, the scope of the granted license, attribution requirements, and any acceptable-use provisions.

3.3 The Provider bears no responsibility for the User's acquisition, use, or license compliance with respect to any Model. The User bears all consequences arising from any breach of a Model's license.

### 4. Output Disclaimer (Accuracy Not Guaranteed)

4.1 **The Provider makes no guarantee as to the accuracy, completeness, reliability, timeliness, or fitness for a particular purpose of any Output.** Large language models may generate information that is factually incorrect (so-called "hallucinations").

4.2 The quality of Output depends heavily on the Model selected by the User, the configuration, the input provided, and device performance.

4.3 The User is responsible for independently verifying Output before relying on it for any important decision.

### 5. Not Professional Advice

5.1 **The App and its Output do not constitute, and are not a substitute for, professional medical, legal, financial, tax, or other professional advice.**

5.2 For matters concerning health, legal, financial, investment, tax, or other professional judgment, always consult a qualified professional.

5.3 The Provider is not liable for any damages arising from the User's reliance on Output as professional advice.

### 6. Acceptable Use

6.1 The User shall use the App and any on-device-generated Output in compliance with all applicable laws.

6.2 The User shall not:

- Use the App for any unlawful purpose or to infringe the rights of third parties (including intellectual property, privacy, and publicity rights);
- Generate or disseminate content that harasses, threatens, defames, discriminates against, or constitutes hate speech toward others;
- Generate malware, phishing, fraudulent, or otherwise harmful content;
- Generate content involving child sexual exploitation or any content prohibited by law;
- Use the App in any manner that violates any Model's license or use policy;
- Reverse-engineer the App (except to the extent permitted by applicable law), make unauthorized modifications, or circumvent the App's safety mechanisms (such as RAM-safe single-Model loading controls).

6.3 Output is generated locally on the User's device. The User bears sole responsibility for the content, storage, sharing, publication, and any downstream use of generated Output.

### 7. Privacy and Advertising

7.1 **Note, prompt, and RAG content never leaves the User's device.** Model inference is performed entirely on-device.

7.2 The App is offered free of charge and displays advertising via Google AdMob. Advertising (banners, an app-open ad at GGUF load, frequency-capped interstitials, and fully opt-in rewarded ads) may transmit device identifiers and similar data.

7.3 The Provider obtains consent via AppTrackingTransparency (ATT) and, for users in the EEA/UK, via a UMP consent management platform. A separate external-transmission disclosure is provided in accordance with Japan's revised Telecommunications Business Act.

7.4 For details on advertising and privacy, please refer to the in-app Privacy Policy.

### 8. In-App Purchase (IAP) and Advertising Terms

8.1 The App offers a **one-time, non-consumable in-app purchase** of approximately JPY 1,500 (tax included; the price may vary based on App Store display and exchange rates). There is **no subscription**.

8.2 Purchasing this IAP **removes ALL advertising** and **permanently grants** the boosts otherwise available through rewarded ads (such as extended generation).

8.3 Rewarded ads are 100% opt-in; viewing them grants benefits such as an extended-generation boost, a 24-hour ad-free pass, or cosmetic customizations.

8.4 Payment, billing, and refunds for IAPs are governed by Apple's App Store terms and procedures. Refunds are handled in accordance with Apple's policies; the Provider cannot issue refunds directly.

8.5 Benefits granted via IAP are tied to the device and Apple ID and are non-transferable. They may be re-obtained via Apple's "Restore Purchases" function where available.

### 9. No Warranty

9.1 The App is provided on an **"AS IS" and "AS AVAILABLE"** basis.

9.2 To the extent permitted by applicable law, the Provider disclaims all warranties, whether express or implied, including merchantability, fitness for a particular purpose, non-infringement, freedom from errors or interruptions, and the accuracy of Output.

### 10. Limitation of Liability

10.1 To the maximum extent permitted by applicable law, the Provider shall not be liable for any indirect, incidental, special, consequential, or punitive damages, or for any loss of profits, data, or goodwill, arising out of or in connection with the use of, or inability to use, the App or any Output.

10.2 To the maximum extent permitted by applicable law, the Provider's aggregate liability relating to the App shall not exceed the amount the User actually paid to the Provider in connection with the App during the preceding twelve (12) months (or JPY 0 for free use).

10.3 Some jurisdictions do not allow the exclusion of implied warranties or the limitation of incidental or consequential damages; in such cases, the above limitations apply only to the extent permitted. Nothing in this Section limits any rights granted to consumers under the Consumer Contract Act or other mandatory law.

### 11. Third-Party Services

The App uses or references third-party services, including Google AdMob, the Apple App Store / StoreKit, and the Model distribution sources the User selects (such as Hugging Face). Each such third-party service is subject to its own terms and privacy policy, for which the Provider is not responsible.

### 12. Age Restriction

The App's App Store age rating is **17+**. The User represents and warrants that they meet the minimum age required to use the App and have the legal capacity to agree to this document under the laws of their place of residence.

### 13. Changes to These Terms

The Provider may revise this document from time to time. For material changes, the Provider will provide notice by reasonable means, such as an in-app notification. Continued use of the App after a revision constitutes acceptance of the revised terms.

### 14. Termination

If the User breaches this document, the User's rights hereunder terminate automatically. The User may terminate use at any time by uninstalling the App. Sections 3, 4, 5, 9 through 11, and 15 survive termination.

### 15. Governing Law and Jurisdiction

15.1 This document is governed by and construed in accordance with **the laws of Japan**.

15.2 Any dispute arising out of or relating to this document shall be subject to the exclusive jurisdiction of the **Tokyo District Court** as the agreed court of first instance.

15.3 This Section does not impair any mandatory rights the User holds as a consumer.

### 16. Contact

For inquiries regarding this document, please contact:
**Contact: morikisei@gmail.com**
