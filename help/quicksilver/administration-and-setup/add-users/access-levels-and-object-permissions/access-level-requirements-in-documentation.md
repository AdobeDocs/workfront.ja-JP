---
title: Workfrontのアクセス要件ドキュメント
content-type: reference
product-area: system-administration
keywords: アクセス, レベル, システム, 管理者, 計画担当者, 作業者, レビュアー, 要求者, 外部, ユーザー
navigation-topic: access-levels
description: Workfront ドキュメントの操作手順記事には、その手順に必要なアクセス権と権限を説明した表が含まれています。この記事では、アクセス要件の表を詳しく説明するほか、詳細情報のリンクも示してあります。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 39ea0d53-ec31-4644-b772-cfe260b8e013
source-git-commit: c1c30696dc9ef324103467f3bdcb83609cf5d1d8
workflow-type: tm+mt
source-wordcount: '1010'
ht-degree: 64%

---

# Workfront ドキュメントのアクセス要件

Workfront ドキュメントの操作手順記事には、その手順に必要なアクセス権と権限を説明した表が含まれています。アクセス要件の表では、Workfront で特定のアクションを実行できるかどうかや、実行できない場合の理由を理解できます。この記事では、アクセス要件表の各要素について説明し、トラブルシューティングのヒントや、より詳細な情報へのリンクを示します。

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
   <td> Adobe Workfront パッケージとは、組織が購入した一連の機能を指します。 ほとんどのWorkfront機能は、すべてのパッケージで使用できますが、いくつかの例外があり、主に戦略的計画とエンタープライズ制御に関連しています。 <p>2022 年以前に存在したパッケージは一覧に表示されません。</p>
   <p>Workfront パッケージは 3 つの領域に分かれています。 一部のエリアでは、Select、Prime、Ultimateなど、異なるパッケージを提供します。<p>
   <ul>
   <li><b>Workfront ワークフロー </b>：タスク管理、承認、タイムシートなど、操作に関連する機能が含まれます。 このパッケージは、さらに Workflow Select パッケージ、Workflow Prime パッケージおよび Workflow Ultimate パッケージに分かれています。</li>
   <li><b>Workfrontプランニング </b>：戦略的計画に関連する機能が含まれます。 このパッケージは、さらに Planning Select パッケージ、Planning Prime パッケージおよび Planning Ultimate パッケージに分かれています。</li>
   <li><b>Workfrontの自動化と統合 </b>：プロセスの自動化および他のアプリケーションとの統合に関する機能が含まれます。</li>
   </ul>
  <p>お客様の組織が、これらの領域の 1 つ以上でWorkfront パッケージを購入している可能性があります。</p>
  <p>以前は、Workfrontは、ワークフロー、計画、自動化と統合を区別することなく、Workfront Select、Workfront PrimeおよびWorkfront Ultimate パッケージを提供していました。 組織が、これらのレガシーパッケージのいずれかに属している可能性があります。 
   <ul><li>現在のパッケージモデルか従来のパッケージモデルかなど、組織で使用しているAdobe Workfront パッケージを確認するには、Workfront管理者にお問い合わせください。</li>
   <li>Workfront管理者が組織のWorkfront パッケージを見つける方法については、<a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-package" class="MCXref xref"> 組織のクラスターとWorkfrontのパッケージを表示 </a> を参照してください。</li><li>Workfront パッケージについて詳しくは、<a href="https://business.adobe.com/jp/products/workfront/pricing.html">Adobe Workfrontの価格とパッケージ </a> を参照してください。</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td> Adobe Workfront ライセンスとは、割り当てられたライセンスに含まれている Workfront 機能のセットを指します。例えば、作業アイテムを完了とマークする機能と時間を記録する機能を含むライセンスを持っているユーザーもいれば、アセットの承認またはリクエストの送信のみが可能なライセンスを持っているユーザーもいます。 <p> 
   <ul>
   <li>割り当てられているライセンスを確認するには、Workfront 管理者にお問い合わせください。</li>
   <li>ライセンスについては、以下を参照してください。
   <ul>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">新しいライセンスの概要</a></li>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">ライセンスの概要</a></li></ul></li>
   <li>正しいアクセスレベルがあるにも関わらずアクセスできない場合は、アクセスレベルにその他の制限が設定されていないか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-package" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。
   </ul>
      </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td><p>Workfrontは他のAdobe製品と緊密に連携するので、Workfrontの一部の手順では、これらの製品と直接やり取りします。 これらの手順に従うには、組織がその製品を購入している必要があります。 例えば、WorkfrontがAdobe Experience Manager Assetsとやり取りできる機能を使用するには、Adobe Experience Manager Assetsを購入する必要があります。</p>
   <p>追加製品を使用して実行される手順を説明する記事では、この表の製品ラインで必要な製品をリストします。</p>
   <p>これらの追加製品のいずれかを所属組織が購入済みかどうかを確認するには、Workfront 管理者にお問い合わせください。</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル</td> 
   <td> アクセスレベルは、Workfront で実行できるアクションに対する一連の権限であり、Workfront 管理者により設定されます。 <p>Workfront には Workfront ライセンスに対応するビルトインのアクセスレベルがありますが、Workfront 管理者は、組織で必要な権限セットをより正確に反映するために、さらにアクセスレベルを作成できます。</p>
   <ul>
    <li>アクセスレベルについて詳しくは、以下を参照してください。
   <ul>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md" class="MCXref xref">新規アクセスレベルの概要</a></li>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref">アクセスレベルの概要</a></li></ul></li>
    <li>ご利用のアクセスレベルの詳細を確認するには、Workfront 管理者にお問い合わせください</li>
    <li>Workfront 管理者の場合、アクセスレベルで特定のオブジェクトへのアクセス権がどのように付与されるかについて詳しくは、<a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Adobe Workfront へのアクセス権の設定</a>を参照してください。</li>  
   <li>正しいアクセスレベルがあるにも関わらずアクセスできない場合は、アクセスレベルにその他の制限が設定されていないか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</li>
    </td>
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td><p>オブジェクト権限とは、個別の Workfront オブジェクトの作成時または共有時に、そのオブジェクトに対してユーザーが持っているアクセス権を指します。例えば、アクセスレベルでプロジェクトを表示できる場合でも、プロジェクトを表示するには、特定のプロジェクトに対する表示アクセス権が必要です。「アクセス要件」テーブルのこのセクションでは、この記事でアクションを実行するために必要な特定のオブジェクト権限について説明します。</p>
   <p>プロジェクトへの追加アクセス権のリクエストについて詳しくは、<a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトの利用申請</a>を参照してください。</p><p>オブジェクトの共有について詳しくは、<a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md" class="MCXref xref">オブジェクトの共有</a>を参照してください。</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">レイアウトテンプレート</td> 
   <td><p>レイアウトテンプレートは、メインメニューに表示される内容を制御し、Workfront 管理者が設定します。この行には、アクションを実行するためにメインメニューに含める必要がある Workfront の特定のエリアが記載されます。</p><p>一般的に、メインメニューのエリアをクリックするように記事内に指示があります。そのエリアがメインメニューに表示されない場合は、Workfront 管理者に問い合わせて、そのエリアを使用できるかどうかを確認してください。</p><p>
   Workfront 管理者がメインメニューを設定する方法について詳しくは、<a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref">レイアウトテンプレートを使用したメインメニューのカスタマイズ</a>を参照してください。</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion ライセンス</td> 
   <td>Adobe Workfront Fusion には、Workfront とは別のライセンスモデルがあります。 
   <ul><li>現在のライセンスモデルは、実行された操作の数に基づいており、組織が実行できるアクションに制限はありません。 </li>
   <li>従来のライセンスは、シナリオがサードパーティのアプリケーションに接続できるかどうか、またはシナリオがWorkfrontの自動処理にのみ使用されるかどうかに基づいています。 </li>
   </ul>
   Fusion ライセンスについて詳しくは、<a href="https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration" class="MCXref xref">Workfront Fusion ライセンス</a>を参照してください。
   </td> 
  </tr> 
 </tbody> 
</table>
