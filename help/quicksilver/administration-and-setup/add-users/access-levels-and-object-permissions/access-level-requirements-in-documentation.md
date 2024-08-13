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
source-git-commit: 822c4e13ab62d129d0a7c603105251e52578576d
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 99%

---

# Workfront ドキュメントのアクセス要件

Workfront ドキュメントの操作手順記事には、その手順に必要なアクセス権と権限を説明した表が含まれています。アクセス要件の表では、Workfront で特定のアクションを実行できるかどうかや、実行できない場合の理由を理解できます。この記事では、アクセス要件表の各要素について説明し、トラブルシューティングのヒントや、より詳細な情報へのリンクを示します。

その記事のアクセス要件表に行がない場合、そのアクションに対するそのタイプの要件はありません。

一部の行には、「新規」と「現在」というラベルの付いた情報が含まれています。これは、Workfront が新しい価格設定のパッケージモデルに移行中であり、新規モデルの下で運用している組織もあれば、現行モデルを引き続き使用している組織もあるからです。自分の組織で使用しているモデルを確認するには、Workfront 管理者にお問い合わせください。詳細と情報へのリンクについては、この記事の[アクセス要件表](#the-access-requirements-table)の節を参照してください。

>[!NOTE]
>
>この表のフィールドのどれに該当するかについてご質問がある場合は、Workfront 管理者にお問い合わせください。

## アクセス要件表

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> Adobe Workfront プランとは、組織が購入した機能のセットを指します。Workfront のほとんどの機能は、いくつかの例外を除き、すべてのプランで使用できます。例外は、主に戦略的計画立案やエンタープライズ管理に関連しています。 
   <ul><li>新規パッケージモデルと既存パッケージモデルのどちらを使用しているかなど、ご自分の組織が使用している Adobe Workfront プランを確認するには、Workfront 管理者にお問い合わせください。</li>
   <li>Workfront 管理者が組織の Workfront プランを確認する方法については、<a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-plan" class="MCXref xref">組織のクラスターと Workfront プランの表示</a>を参照してください。</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td> Adobe Workfront ライセンスとは、割り当てられたライセンスに含まれている Workfront 機能のセットを指します。例えば、作業アイテムを完了とマークする機能と時間を記録する機能を含むライセンスを持っているユーザーもいれば、アセットの承認またはリクエストの送信のみが可能なライセンスを持っているユーザーもいます。 <p> 
   <ul>
   <li>割り当てられているライセンスを確認するには、Workfront 管理者にお問い合わせください。</li>
   <li>Adobe Workfront は、新しい価格設定のパッケージモデルに移行しつつあります。ライセンスについては、以下を参照してください。
   <ul>
   <li>新規：<a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">新しいライセンスの概要</a></li>
   <li>現在：<a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">ライセンスの概要</a></li></ul></li>
   <li>正しいアクセスレベルがあるにも関わらずアクセスできない場合は、アクセスレベルにその他の制限が設定されていないか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-plan" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。
   </ul>
      </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>Workfront では、Workfront に追加していくつかの製品を購入できます。
   <p>それらの追加製品内で実行される手順を説明した記事には、必要な製品がリストされています。</p>
   <ul>
   <li>Adobe Experience Manager Assets または Assets Essentials </li>
   <li>Workfront Fusion</li>
   <li>Workfront Goals</li>
   <li>Workfront のシナリオプランナー</li>
   </ul>
   <p>これらの追加製品のいずれかを所属組織が購入済みかどうかを確認するには、Workfront 管理者にお問い合わせください。</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル</td> 
   <td> アクセスレベルは、Workfront で実行できるアクションに対する一連の権限であり、Workfront 管理者により設定されます。 <p>Workfront には Workfront ライセンスに対応する組み込みのアクセスレベルがありますが、Workfront 管理者は、組織で必要な権限セットをより正確に反映するために、さらにアクセスレベルを作成できます。</p>
   <ul>
    <li>Adobe Workfront は、新しい価格設定のパッケージモデルに移行しつつあります。各モデルのアクセスレベルについては、以下を参照してください。
   <ul>
   <li>新規：<a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md" class="MCXref xref">新しいアクセスレベルの概要</a></li>
   <li>現在：<a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref">アクセスレベルの概要</a></li></ul></li>
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
   <ul><li>現在：現在のライセンスモデルは、実行された操作の数に基づいており、組織が実行できるアクションに制限はありません。 </li>
   <li>レガシ：従来のライセンスは、シナリオがサードパーティのアプリケーションに接続できるかどうか、またはシナリオが Workfront 自動処理にのみ使用されるかどうかに基づきます。 </li>
   </ul>
   Fusion ライセンスについて詳しくは、<a href="/help/quicksilver/workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">Workfront Fusion ライセンス</a>を参照してください。
   </td> 
  </tr> 
 </tbody> 
</table>
