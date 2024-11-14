---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion での大きなファイルの操作
description: 現在、Workfrontおよび HTTP コネクタでは大きなファイルがサポートされています。
author: Becky
feature: Workfront Fusion
exl-id: e0be458c-a5f4-48e4-a8fb-afd5d072b6ff
source-git-commit: 4914e6e30d6c4a16de5bd2c91bc6f8e4f208c078
workflow-type: tm+mt
source-wordcount: '1100'
ht-degree: 4%

---

# Adobe Workfront Fusion での大きなファイルの操作

>[!IMPORTANT]
>
>大容量ファイル機能は、Workfront Ultimate のお客様のみが利用でき、段階的なロールアウトです。 Workfront Ultimate プランを使用するすべての Fusion 組織は、2025 年 1 月までに大容量ファイルを使用できるようになります。

Workfront Fusion で強化されたデータ転送機能が使用できるようになり、シナリオで大幅に大きなファイルを処理できるようになりました。

大きなファイルを処理するには、シナリオを更新する必要があります。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td>
   <td> <p>新規：Ultmate</p> <p>または</p> <p>現在：使用できません</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td> <p>新規：[!UICONTROL Standard]</p><p>または</p><p>現在：使用できません</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在：[!DNL Workfront Fusion] ライセンスは必要ありません。</p>
   <p>または</p>
   <p>レガシー：任意 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>新規：[!DNL Workfront Fusion] は Ultimate Workfront プランに含まれます。</p> <p>または</p>
   <p>現在：使用できません</p>
   </td> 
  </tr>
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

+++

## 大きなファイルをサポートするコネクタ

初回リリースの場合、次のコネクタは大きなファイルをサポートします。

* Workfront / ドキュメントをアップロード
* Adobe Experience Manager Assets / ドキュメントをアップロード
* Workfront Proof / ファイルをアップロード
* Adobe Authenticator / カスタム API 呼び出しを行う
* HTTP

その他のコネクタは、今後のリリースでサポートされる予定です。

## 大きなファイルを処理するためのシナリオの更新

Workfront/ドキュメントをアップロード モジュールが変更され、大きなファイルを処理できるようになりました。 このモジュールの以前のバージョンでは、モジュール名に `(Legacy)` が追加されて表示されるようになりました。 ほとんどの場合、レガシーモジュールは引き続き機能します。

大きなファイルを扱う予定がある場合は、従来のモジュールを新しいドキュメントをアップロード モジュールに置き換えることをお勧めします。 新しいドキュメントをアップロードモジュールは、タイムアウトやその他のエラーを防ぎます。

![ドキュメントをアップロード](assets/new-upload-document.png)

## よくある質問

### 新しいファイルサイズ制限は何ですか。

ユーザーは、以前の 1 GB の制限を超えるファイルを処理できるようになり、効率と生産性が向上します。  プラットフォームでは、1 回のアクション（ファイルのアップロードなど）で最大 15 GB の個々のファイルをサポートできますが、データ転送に影響を与える他の要因があります。 単一アクションのファイルサイズの制限は、最終的には Fusion が接続する web サービスに依存します。 データ転送は、1 回の実行に対する合計の処理です。 つまり、1 回の実行で複数のアクションが合計データ転送に貢献します。

Fusion は、40 分の実行制限に達するまでファイルを処理します。 大きなファイルの場合、Fusion シナリオでアップロード、ダウンロードまたは処理に時間がかかる場合があります。 個々のファイルサイズに制限はありませんが、シナリオの実行時間は 40 分に制限されています。 したがって、サイズの大きなファイルによって実行に 40 分以上かかる場合は、シナリオは失敗します。 シナリオの実行時間は、シナリオのサイズ、モジュールの複雑さ、ネットワーク速度の影響も受ける場合があります。 したがって、大きなファイルを使用する場合は、シナリオのこれらの側面を考慮することをお勧めします。

### Fusion の新しいファイル転送はどのように機能しますか？

Fusion がファイルを処理すると、大きなファイルが永続ストレージ（S3 バケットまたは Azure Blob ストレージ）に追加されます。 Fusion モジュールがアップロードやダウンロードなどのファイルアクションを実行すると、Fusion はアクティブメモリではなく、永続ストレージのファイルをソースとして使用します。

### 不完全な実行を使用してより大きなファイルを操作できますか？

はい。Fusion では、大きなファイルを含んだ不完全な実行をサポートしています。 不完全な実行は 1 つの組織でのサイズが制限されるので、積極的に管理する必要があります。

### 大きなファイルをコネクタで使用できますか？

大きなファイルをサポートするには、各 Fusion コネクタを更新する必要があります。 サポートされているコネクタには、Workfront、HTTP およびAEM Assetsがあります。 Fusion コネクタは、web サービスでサポートされているファイルサイズによって、引き続き制限されます。 ファイルサイズの制限は、通常、ファイルをダウンロードおよびアップロードする web サービスエンドポイントに関する API ドキュメントに含まれています。

### これは業務に影響を与えますか？

いいえ。モジュールが実行する操作の数は同じです。

### Fusion の UI がファイル転送データを表示するように更新されるのはいつですか？

ダッシュボードとシナリオ実行の詳細ページのファイル転送に関する Fusion の UI の更新に積極的に取り組んでおり、2025 年第 1 四半期にリリースを予定しています。

### シナリオの設計に役立つ新しいファイル処理制限について考える方法を教えてください。

実行の上限である 40 分以内に動作するようにシナリオを設計するのは複雑に思えるかもしれません。 シナリオを設計する際は、次の点に留意することをお勧めします。

* **実行時間のビジネス要件を理解する**:Fusion の実行時間のプラットフォーム制限は 40 分ですが、ほとんどのビジネスプロセスの自動化は、はるかに高速に実行されると予想されています。 例えば、ユーザーが開始し、結果に依存する続行を行う自動化は、40 分の制限内で十分に完了すると予想されます。
* **設計時の実行時間を考慮**：シナリオを設計する際は、アップロードやダウンロードなど、個々のファイルアクションのモジュール実行時間を理解することが重要です。 この知識は、複数のファイルアクションを含むシナリオを計画するのに役立ちます。  設計の正確性を確保するために、モジュールの実行時間をバッファを含むように切り上げることをお勧めします。
例えば、Fusion が 144 秒（2.4 分）でドキュメントをダウンロードする場合、1 回の実行で同様のアクションを複数回実行できると予測できます。 この例では、モジュールの実行には 144 秒かかるので、ダウンロードには 3 分間の実行時間を計画する必要があります。 要件にアップロードとダウンロードの両方が含まれる場合、予想実行時間は約 6 分です。 Fusion の実行時間は 40 分に制限されています。

* **ファイルアクションの統合**:Fusion シナリオにおけるファイルアクションの最も一般的な例は、ダウンロードとアップロードの 1 つです。 これら 2 つのアクションのみのシナリオのほとんどは、数分で実行されます。 可能であれば、Fusion デザイナーはシナリオを 1 回のダウンロードと 1 回のアップロードに制限する必要があります。

* **マッピングパネルを使用したサイズの計算**:Workfrontやその他の web サービスでは、ダウンロードモジュールの出力にファイルのファイルサイズが含まれます。 このデータを使用して、モジュールのアップロードには大きすぎるファイルや、シナリオの実行時間には大きすぎるファイルを除外できます。

* **複数のファイルを操作する際に、ファイル操作を独自のシナリオで分離する**:Fusion デザイナーは、ファイル操作を個別のシナリオに分離することを検討する必要があります。 例えば、複数のファイルが添付された新しいWorkfront リクエストでトリガーされた Fusion シナリオでは、最大 30 個のファイルを格納する必要がある場合があります。 各ファイルのアップロードとダウンロードに最大 3 分かかる場合があるので、1 回の実行ですべてのファイルを処理すると、Fusion の 40 分の実行制限を超えます。 解決策は、個々のファイルのアップロードおよびダウンロードを処理する専用のファイルアクションシナリオを作成することです。 リクエストトリガーのシナリオは、添付ファイルを繰り返し処理し、HTTP モジュールを使用して各ファイルのファイルアクションシナリオを呼び出します。 このアプローチにより、各ファイルが実行時間制限内で確実に処理されます。

<!--
## Connectors that do not support large files

Some Fusion connectors do not support large files. For these connectors, Fusion's total processing capacity for files is **1 GB**. 

This limit is based on a total memory cost. Every operation contributes to that cost. If a single file of 400 MB is downloaded and uploaded then the total cost to the file capacity would be 800 MB.

The following connectors do **not** support large files. 

* Archive
* Box
* Convert
* CSV
* Datastores
* Flow control
* FTP
* JSON
* JWT
* Markdown
* Math
* Microsoft Word templates
* MIME
* Microsoft SQL
* SFTP
* Adobe Acrobat Sign
* SOAP
* Tools
* XML

If a connector is not on this list, it does not support large files. For these connectors, Fusion's total processing capacity for files is **1 GB**. 

This limit is based on a total memory cost. Every operation contributes to that cost. If a single file of 400 MB is downloaded and uploaded then the total cost to the file capacity would be 800 MB.-->






<!--## Connectors that support large files

The following connectors support large files.

Workfront
HTTP
Webhooks
Salesforce
Microsoft Email
Workfront Proof
AEM Assets
Email
Slack
Jira
Microsoft Excel
SharePoint
Frame.io
Adobe PDF Services
Marketo
Azure Devops 
Google Email
Jira Server
Google Sheets
Microsoft OneDrive
ServiceNow 
AWS S3
Bynder
OneDrive Business
Adobe Authenticator
Google Drive
Microsoft Dynamics
Google Docs
NetSuite
Airtable
Azure AD
QuickBase 
Adobe Target
Adobe Campaign Classic
Microsoft Calendar
Workfront Planning
HubSpot CRM  
DropBox
Cloud Convert
Egnyte
Adobe Firefly
OpenAI / Chat GPT
Allocadia
Cvent
GitLab 
Google Team Drive
Google Calendar
Workfront SDL Managed Translation
Widen
Workfront Boards
Google Slides
Qualtrics
Microsoft Power BI
Adobe Photoshop
Anaplan
DocuSign 
MariaDB
Adobe Creative Cloud Libraries
Figma
AEM Forms
Datadog
GitHub 
Google Forms
Adobe I/O Events
Trello
Workday
Adobe Journey Optimizer
Adobe Lightroom


If a file is not on this list, it does not support large files. For these connectors, Fusion's total processing capacity for files is **1 GB**. 

This limit is based on a total memory cost. Every operation contributes to that cost. If a single file of 400 MB is downloaded and uploaded then the total cost to the file capacity would be 800 MB.

-->
