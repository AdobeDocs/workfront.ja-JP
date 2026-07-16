---
title: Workfront ドキュメントのアクセス要件
content-type: reference
product-area: system-administration
keywords: アクセス, レベル, システム, 管理者, 計画担当者, 作業者, レビュアー, 要求者, 外部, ユーザー
navigation-topic: access-levels
description: Workfront ドキュメントの操作手順記事には、その手順に必要なアクセス権と権限を説明した表が含まれています。 この記事では、アクセス要件の表を詳しく説明するほか、詳細情報のリンクも示してあります。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 39ea0d53-ec31-4644-b772-cfe260b8e013
TQID: https://experienceleague.adobe.com/DP4cAQiJdCpE59ppP-EvU3UcJomEd9TUxza6DIB1cDg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: ee260723331ddff4e8d89f7d9ca2b807835d6130
workflow-type: tm+mt
source-wordcount: 1070
ht-degree: 62%

---

# Workfront ドキュメントのアクセス要件

Workfront ドキュメントの操作手順記事には、その手順に必要なアクセス権と権限を説明した表が含まれています。 アクセス要件の表では、Workfront で特定のアクションを実行できるかどうかや、実行できない場合の理由を理解できます。 この記事では、アクセス要件表の各要素について説明し、トラブルシューティングのヒントや、より詳細な情報へのリンクを示します。

その記事のアクセス要件表に行がない場合、そのアクションに対するそのタイプの要件はありません。

>[!NOTE]
>
>この表のフィールドのどれに該当するかについてご質問がある場合は、Workfront 管理者にお問い合わせください。

## アクセス要件表

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> Adobe Workfrontのパッケージとは、組織が購入した機能セットを指します。 Workfrontの機能の多くは、すべてのパッケージで利用できます。一部のパッケージを除き、主に戦略的プランニングとエンタープライズ管理に関連しています。 <p>2022年以前に存在していたパッケージはリストに含まれていません。</p>
   <p>Workfrontのパッケージは、3つの領域に分かれています。 一部の地域では、Select、Prime、Ultimateなど、様々なパッケージが提供されています。<p>
   <ul>
   <li><b>Workfront ワークフロー</b>: タスク管理、承認、タイムシートなど、操作に関連する機能が含まれます。 このパッケージは、ワークフロー選択、ワークフローPrime、ワークフローUltimateの各パッケージにさらに分かれています。</li>
   <li><b>Workfront計画</b>：戦略的プランニングに関連する機能が含まれます。 このパッケージは、Planning Select、Planning Prime、Planning Ultimateの各パッケージにさらに分かれています。</li>
   <li><b>Workfront Automation and Integration</b>: プロセスの自動化と他のアプリケーションとの統合に関連する機能が含まれます。</li>
   </ul>
  <p>お客様は、これらの領域の1つ以上でWorkfront パッケージを購入した可能性があります。</p>
  <p>以前、Workfrontでは、Workfront Select、Workfront Prime、Workfront Ultimateの各パッケージが提供されていましたが、ワークフロー、プランニング、自動処理および統合は区別されていませんでした。 組織は、これらのレガシーパッケージの1つに属している可能性があります。 
   <ul><li>現在のパッケージモデルと従来のパッケージモデルのどちらを使用しているかなど、組織で使用されているAdobe Workfront パッケージを確認するには、Workfront管理者にお問い合わせください。</li>
   <li>Workfront管理者が組織のWorkfront パッケージを見つける方法については、<a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-package" class="MCXref xref">組織のクラスターとWorkfront パッケージの表示</a>を参照してください。</li><li>Workfront パッケージについて詳しくは、<a href="https://business.adobe.com/products/workfront/pricing.html">Adobe Workfrontの価格とパッケージ </a>を参照してください。</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td> Adobe Workfront ライセンスとは、割り当てられたライセンスに含まれている Workfront 機能のセットを指します。 例えば、作業アイテムを完了とマークする機能と時間を記録する機能を含むライセンスを持っているユーザーもいれば、アセットの承認またはリクエストの送信のみが可能なライセンスを持っているユーザーもいます。 <p> 
   <p>Adobe Workfront ライセンスは、次の種類のライセンスを参照できます。</p>
   <ul><li>Workfront Workflow ライセンス</li>
  <li>Workfront計画ライセンス</li></ul>

<p>割り当てられているライセンスを確認するには、Workfront 管理者にお問い合わせください。</p>
   <p>ライセンスについては、以下を参照してください。</p>
   <ul>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md">カスタムアクセスレベルの作成と変更</a></li>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">新しいライセンスの概要</a></li>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">ライセンスの概要</a></li></ul>
   <p>正しいアクセスレベルがあるにも関わらずアクセスできない場合は、アクセスレベルにその他の制限が設定されていないか Workfront 管理者にお問い合わせください。 Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-package" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td><p>Workfrontは他のAdobe製品と緊密に連携しているため、Workfrontの一部の手順では、これらの製品と直接やり取りします。 この手順に従うには、組織はその製品を購入している必要があります。 例えば、WorkfrontでAdobe Experience Manager Assetsを利用できるようにする機能を使用するには、Adobe Experience Manager Assetsを購入している必要があります。</p>
   <p>追加製品で実行された手順について説明する記事では、この表の製品ラインに必要な製品をリストします。</p>
   <p>これらの追加製品のいずれかを所属組織が購入済みかどうかを確認するには、Workfront 管理者にお問い合わせください。</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル</td> 
   <td> アクセスレベルは、Workfront で実行できるアクションに対する一連の権限であり、Workfront 管理者により設定されます。 <p>Workfront には Workfront ライセンスに対応するビルトインのアクセスレベルがありますが、Workfront 管理者は、組織で必要な権限セットをより正確に反映するために、さらにアクセスレベルを作成できます。</p>
   <ul>
    <li>アクセス・レベルについては、次を参照してください。
   <ul>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md" class="MCXref xref">新規アクセスレベルの概要</a></li>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref">アクセスレベルの概要</a></li></ul></li>
    <li>ご利用のアクセスレベルの詳細を確認するには、Workfront 管理者にお問い合わせください</li>
    <li>Workfront 管理者の場合、アクセスレベルで特定のオブジェクトへのアクセス権がどのように付与されるかについて詳しくは、<a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Adobe Workfront へのアクセス権の設定</a>を参照してください。</li>  
   <li>正しいアクセスレベルがあるにも関わらずアクセスできない場合は、アクセスレベルにその他の制限が設定されていないか Workfront 管理者にお問い合わせください。 Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</li>
    </td>
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td><p>オブジェクト権限とは、個別の Workfront オブジェクトの作成時または共有時に、そのオブジェクトに対してユーザーが持っているアクセス権を指します。 例えば、アクセスレベルでプロジェクトを表示できる場合でも、プロジェクトを表示するには、特定のプロジェクトに対する表示アクセス権が必要です。 「アクセス要件」テーブルのこのセクションでは、この記事でアクションを実行するために必要な特定のオブジェクト権限について説明します。</p>
   <p>プロジェクトへの追加アクセス権のリクエストについて詳しくは、<a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトの利用申請</a>を参照してください。</p><p>オブジェクトの共有について詳しくは、<a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md" class="MCXref xref">オブジェクトの共有</a>を参照してください。</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">レイアウトテンプレート</td> 
   <td><p>レイアウトテンプレートは、メインメニューに表示される内容を制御し、Workfront 管理者が設定します。 この行には、アクションを実行するためにメインメニューに含める必要がある Workfront の特定のエリアが記載されます。</p><p>一般的に、メインメニューのエリアをクリックするように記事内に指示があります。そのエリアがメインメニューに表示されない場合は、Workfront 管理者に問い合わせて、そのエリアを使用できるかどうかを確認してください。</p><p>
   Workfront 管理者がメインメニューを設定する方法について詳しくは、<a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref">レイアウトテンプレートを使用したメインメニューのカスタマイズ</a>を参照してください。</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion ライセンス</td> 
   <td>Adobe Workfront Fusion には、Workfront とは別のライセンスモデルがあります。 
   <ul><li>現在のライセンスモデルは、実行された操作数に基づいており、組織が実行できるアクションに制限はありません。 </li>
   <li>従来のライセンスは、シナリオがサードパーティ製アプリケーションに接続できるかどうか、またはシナリオがWorkfront自動処理にのみ使用されるかどうかに基づいています。 </li>
   </ul>
   Fusion ライセンスについて詳しくは、<a href="https://experienceleague.adobe.com/en/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration" class="MCXref xref">Workfront Fusion ライセンス</a>を参照してください。
   </td> 
  </tr> 
 </tbody> 
</table>
