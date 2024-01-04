---
title: アクセスレベルの要件
content-type: reference
product-area: system-administration
keywords: アクセス，レベル，システム，管理者，プランナー，ワーカー，レビュー担当者，要求者，外部，ユーザー
navigation-topic: access-levels
description: Workfrontドキュメントのハウツー記事には、その手順に必要なアクセスと権限の説明を記載した表が含まれています。 この記事では、アクセス要件の表の詳細を説明し、詳細情報のリンクを含んでいます。
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
source-git-commit: 96f88c4b31b92998cfb8fa25ed1de0dfa0c70462
workflow-type: tm+mt
source-wordcount: '884'
ht-degree: 0%

---

# アクセスレベルの要件 ( Workfrontドキュメント )

Workfrontドキュメントのハウツー記事には、その手順に必要なアクセス要件と権限要件を説明した表が含まれています。 このアクセス要件の表では、Workfrontで特定のアクションを実行できるかどうか、または実行できない理由を把握できます。 この記事では、アクセス要件テーブルの各要素について説明し、トラブルシューティングのヒントと、より詳細な情報へのリンクを示します。

特定の記事の「アクセス要件」テーブルに行がない場合、そのアクションに対してそのタイプの要件はありません。

一部の行には、「新規」と「現在」というラベルの付いた情報が含まれています。 これは、Workfrontが新しい価格とパッケージのモデルに移行し、一部の組織が新しいモデルで運用され、他の組織が現在のモデルを引き続き使用しているためです。 組織で使用しているモデルを確認するには、Workfront管理者に問い合わせてください。 詳細および情報へのリンクは、 [アクセス要件テーブル](#the-access-requirements-table) 」の節を参照してください。

>[!NOTE]
>
>このテーブルのフィールドのいずれかが自分にどのように適用されるかについて質問がある場合は、Workfront管理者にお問い合わせください。

## アクセス要件テーブル

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td> Adobe Workfrontプランとは、組織が購入した一連の機能を指します。 Workfrontのほとんどの機能は、いくつかの例外を除き、すべてのプランで使用できます。主に戦略的な計画およびエンタープライズ管理に関連しています。 
   <ul><li>組織が新しいパッケージモデルか現在のパッケージモデルかなど、Adobe Workfrontで組織が使用するプランを確認するには、Workfront管理者に問い合わせてください。</li>
   <li>Workfront管理者が組織のWorkfrontプランを見つける方法については、 <a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-plan" class="MCXref xref">組織のクラスターとWorkfrontプランを表示</a>.</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td> Adobe Workfrontライセンスとは、割り当てられているライセンスに含まれるWorkfront機能のセットを指します。 例えば、あるユーザーが、作業項目の完了とログ記録時間を含むライセンスを持っている一方、別のユーザーがアセットの承認または要求の送信のみを許可するライセンスを持っているとします。 <p> 
   <ul>
   <li>割り当てられているライセンスを確認するには、Workfront管理者に問い合わせてください。</li>
   <li>Adobe Workfrontは、新しい価格とパッケージのモデルに移行しつつあります。 ライセンスの詳細については、以下を参照してください。
   <ul>
   <li>新規： <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">新しいライセンスの概要</a></li>
   <li>現在： <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">ライセンスの概要</a></li></ul></li>
   <li>正しいアクセスレベルを持っていて、まだアクセス権がない場合は、Workfront管理者にアクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.
   </ul>
      </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>Workfrontでは、Workfrontに加えて、いくつかの製品を購入できます。
   <p>これらの追加製品内で実行される手順を説明する記事は、必要な製品をここにリストします。</p>
   <ul>
   <li>Adobe Experience Manager AssetsまたはAssets Essentials </li>
   <li>Workfront Fusion</li>
   <li>Workfront Goals</li>
   <li>Workfront Scenario Planner</li>
   </ul>
   <p>これらの追加製品の 1 つを購入したかどうかを確認するには、Workfront管理者に問い合わせてください。</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル</td> 
   <td> アクセスレベルは、Workfrontで実行できるアクションに対する一連の権限で、Workfront管理者が設定します。 <p>WorkfrontにはWorkfrontライセンスに対応する組み込みのアクセスレベルがありますが、Workfront管理者は、組織で必要な権限セットをより正確に反映するために、より多くのアクセスレベルを作成できます。</p>
   <ul>
    <li>Adobe Workfrontは、新しい価格とパッケージのモデルに移行しつつあります。 各モデルのアクセス・レベルの詳細は、次を参照してください。
   <ul>
   <li>新規： <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md" class="MCXref xref">新しいアクセスレベルの概要</a></li>
   <li>現在： <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref">アクセスレベルの概要</a></li></ul></li>
    <li>アクセスレベルの詳細を確認するには、Workfront管理者に問い合わせてください</li>
    <li>Workfront管理者の場合は、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Adobe Workfrontへのアクセスの設定</a> を参照して、アクセスレベルで特定のオブジェクトに対するアクセス権を付与する方法の詳細を確認してください。</li>  
   <li>正しいアクセスレベルを持っていて、まだアクセス権がない場合は、Workfront管理者にアクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</li>
    </td>
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td><p>オブジェクト権限とは、個々のWorkfrontオブジェクトの作成時または共有時にそのオブジェクトに対して持つアクセス権を指します。 例えば、アクセスレベルでプロジェクトを表示できる場合でも、プロジェクトを表示するには、特定のプロジェクトに対する表示アクセス権が必要です。 「アクセス要件」テーブルのこのセクションでは、この記事でアクションを実行するために必要な特定のオブジェクト権限について説明します。</p>
   <p>オブジェクトへの追加アクセス権のリクエストについては、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>Workfrontでは、Workfrontに加えて、いくつかの製品を購入できます。
   <p>これらの追加製品内で実行される手順を説明する記事は、必要な製品をここにリストします。</p>
   <ul>
   <li>Adobe Experience Manager AssetsまたはAssets Essentials </li>
   <li>Workfront Fusion *</li>
   <li>Workfront目標*</li>
   <li>Workfrontシナリオプランナー*</li>
   </ul>
   <p>* Workfront Ultimate プランに含まれる
   <p>お客様の組織がこれらの追加製品の 1 つを購入したかどうか、またはお客様の組織がWorkfront Ultimate プランに参加している場合は、Workfront管理者にお問い合わせください。</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion ライセンス</td> 
   <td>Adobe Workfront Fusion には、Workfrontとは別のライセンスモデルがあります。 
   <ul><li>現在：現在のライセンスモデルは、実行された操作の数に基づいており、組織が実行できる操作に制限はありません。 </li>
   <li>レガシー：従来のライセンスは、シナリオがサードパーティのアプリケーションに接続できるかどうか、またはシナリオがWorkfront自動化にのみ使用されるかどうかに基づきます。 </li>
   </ul>
   Fusion ライセンスについて詳しくは、 <a href="/help/quicksilver/workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">Workfront Fusion ライセンス</a>.
   </td> 
  </tr> 
 </tbody> 
</table>


