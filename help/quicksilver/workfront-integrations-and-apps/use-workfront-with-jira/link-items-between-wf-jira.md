---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: ' [!DNL Adobe Workfront]  と  [!DNL Jira] 間で項目をリンク'
description: ' [!DNL Jira]  のイシューを、 [!DNL Adobe Workfront]  のタスクまたはイシューに、自動または手動でリンクできます。'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 1c37f361-e866-4ac6-b672-408848a80ed6
source-git-commit: b1b55b8046aa771abb2cceda333940ccf827356a
workflow-type: tm+mt
source-wordcount: '1378'
ht-degree: 49%

---

# [!DNL Adobe Workfront] と [!DNL Jira] 間で項目をリンク

<!-- Audited: 5/2025 -->

>[!IMPORTANT]
>
>より安定したスケーラブルな統合を実現するために、アドビでは、Workfront Automation and Integration （Fusion）を使用した最新の柔軟な統合アプローチに移行しています。 この移行プロセスの一環として、Workfront for Jira の統合は **2026 年 2 月 28 日** 以降は利用できなくなります。
>
>Jira を使用する場合は、組織の統合のニーズに合わせてWorkfront Automation and Integration を使用することをお勧めします。
>
>Workfrontの自動処理と統合の概要については、[Adobe Workfront Fusion の概要 ](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview) を参照してください。
>
>Jira 用のWorkfront Automation and Integration Modules の具体的な機能については、「[Jira ソフトウェアモジュール ](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules)」を参照してください。

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

[!DNL Jira] のイシューを、[!DNL Adobe Workfront] のタスクまたはイシューに、自動または手動でリンクできます。

[!DNL Workfront] の中の 1 つの項目のみが、[!DNL Jira] 内の 1 つの項目にリンクできます。1 つの [!DNL Workfront] 項目を複数の [!DNL Jira] イシュー、または 1 つの [!DNL Jira] イシューを複数の [!DNL Workfront] 項目にリンクさせることはできません。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td><p>任意</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>標準 </p>
       <p>プラン </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Jira アクセス</td> 
   <td> <p>システム管理者のアクセス権</p> <p>重要：ユーザーに関連付けられた既存のシステム管理者アカウントを使用するのではなく、Jira とWorkfrontで個別のシステム管理者アカウントを作成して、この統合専用にすることをお勧めします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## [!DNL Workfront] for [!DNL Jira] のインストール

[!DNL Workfront] for [!DNL Jira] OnDemand のインストール方法は、[!DNL Jira] サーバーインスタンスにインストールする場合と同じです。

[!DNL Workfront] アドオンをインストールするには、[!DNL Jira] 管理者である必要があります。

[!DNL Jira] 管理者でない場合は、[!DNL Workfront] アドオンを参照して、そのインストールをリクエストできます。リクエストは [!DNL Jira] 管理者に送信されて、承認後にインストールが行われます。

[!DNL Jira] アプリケーションへのアドオンのインストールをリクエストする方法について詳しくは、[ユーザーのアドオンリクエストの管理](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)を参照してください。

[!DNL Workfront for Jira] をインストールするには、次の手順に従います。

1. [!DNL Jira] に [!DNL Jira] 管理者としてログインします。
1. [[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview) で **[!DNL Workfront for Jira]** アドオンを検索します。

1. 「**[!UICONTROL 今すぐ入手]**」をクリックしてインストールします。

   インストールが完了したら、[!DNL Jira] から [!DNL Workfront] にログインし統合を設定できます。

   詳しくは、[Adobe Workfront の Jira 向け設定](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)を参照してください。

## 前提条件

[!DNL Workfront] と [!DNL Jira] の間で項目をリンクする前に、次の操作を行う必要があります。

* [!DNL Workfront] 用に [!DNL Jira] をインストールします。

  手順については、[Jira 用Adobe Workfrontのインストール ](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md) を参照してください。

* Jira 用に [!DNL Workfront] を設定します。

  手順については、[Adobe Workfront for Jira の設定 ](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md) を参照してください。

## [!DNL Workfront] の項目を [!DNL Jira] のイシューに自動でリンク

[!DNL Workfront] 管理者は、タスクまたは [!DNL Jira] のイシューで特定の条件が満たされるたびに [!DNL Workfront] で自動的にイシューを作成するトリガーを定義できます。 Workfront と [!DNL Jira] の項目がリンクされます。

Jira 用 [!DNL Workfront]の設定を完了すると、[!DNL Workfront] で項目が作成または更新されてトリガーに一致したとき、[!DNL Jira] で新しい項目が自動作成されます。

Workfront の項目を作成および更新する Workfront ユーザーには、[!DNL Jira] の項目作成をトリガーするための [!DNL Jira] ライセンスは必要ありません。

詳しくは、[Jira 用に設定  [!DNL Adobe Workfront]  を参照してください ](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)。

>[!NOTE]
>
>プロジェクトにテンプレートを添付することで、[!DNL Jira] 項目を自動作成できます。テンプレートに、[!DNL Jira] のトリガーに一致する割り当てを持つタスクが含まれる場合、新しいタスクによって [!DNL Jira] の新しいイシューが生成されます。

[!DNL Workfront] のイシューを [!DNL Jira] のイシューに自動でリンクすることと、[!DNL Workfront] のタスクを [!DNL Jira] のイシューに自動でリンクすることは同じです。

[!DNL Workfront] のタスクを [!DNL Jira] のイシューに自動でリンク

1. [!DNL Workfront] 項目が割り当てられたときに [!DNL Jira] のイシューを自動作成するトリガーを [!DNL Jira] システム管理者が設定したことを確認し、タスクの作成が許可されているアクセスレベルで [!DNL Workfront] にログインします。

   タスクへのアクセス権について詳しくは、[タスクへのアクセス権を付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)を参照してください。

{{step1-to-projects}}

1. **プロジェクト** ページで、プロジェクトを選択します。

1. プロジェクトの左パネルで、「**[!UICONTROL タスク]**」を選択します。

1. 「**+新規タスク**」をクリックします。

   >[!NOTE]
   >
   >既存のWorkfront項目を Jira の課題にリンクするには、項目の **詳細****詳細** アイコンから ![ 編集 ](assets/more-icon.png) を選択します。

1. タスクに使用できるフィールドを指定または更新します。
1. 「**[!UICONTROL 割り当て]**」フィールドで、[!DNL Jira] 統合でトリガーとして指定されているユーザー、ロールまたはチームを検索して選択します。

1. **タスクを作成** をクリックします。 タスクがWorkfrontで作成され、タスクの **更新** タブに新しいコメントが表示され、[!DNL Jira] でも新しいイシューが作成されたことを示します。

1. （任意）タスクまたは問題ヘッダーの **[!UICONTROL 詳細]** セクションの **[!UICONTROL 統合]** 領域で、**[!UICONTROL Jira に移動]** リンクをクリックして Jira で問題を開きます。

   システム管理者またはグループ管理者がレイアウトテンプレートに[!UICONTROL 統合]フィールドを追加して、タスクまたはイシューのヘッダーに表示する必要があります。詳しくは、[レイアウトテンプレートを使用してオブジェクトヘッダーをカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)を参照してください。

   [!DNL Jira] ユーザーはすぐに [!DNL Workfront] から自動作成された項目の作業を開始でき、その更新は [!DNL Workfront] ライセンスがなくても [!DNL Workfront] に移行されます。

   自分が [!DNL Workfront] 管理者として [!DNL Workfront] アドオンの設定時に設定したフィールドのみが更新されます。

   Workfrontと Jira 間でのフィールドの同期について詳しくは、[Jira 用Workfrontの設定 ](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md) の「Jira 用Adobe Workfrontの設定」の節を参照してください。

   >[!NOTE]
   >
   >[!DNL Jira] のイシューがWorkfrontから自動的に作成される場合、[!DNL Jira] 内の誰にも割り当てられていません。

## [!DNL Jira] のイシューを [!DNL Workfront] 項目に手動でリンク

[!DNL Jira] で項目を作成し、[!DNL Workfront] 互いに独立したら、[!DNL Jira] のイシューを既存の [!DNL Workfront] のタスクまたはイシューに手動でリンクできます。

[!DNL Workfront] 項目を、[!DNL Workfront] から既存の [!DNL Jira] 項目に手動でリンクすることはできません。

>[!NOTE]
>
>[!DNL Workfront] 統合でトリガーと識別されないプロジェクト上に [!DNL Jira] イシューが存在しない場合、[!DNL Jira] オンプレミスとの統合を利用して Workfront 項目に手動でリンクすることはできません。\
>Workfront から Jira へのワークフローのトリガー設定について詳しくは、[Workfront の項目を Jira のイシューに自動的にリンク](#automatically-link-workfront-items-to-jira-issues)を参照してください。

[!DNL Workfront] および [!DNL Jira] 項目がリンクされている場合、ある項目の特定のフィールドは、別の項目の特定のフィールドを自動的に更新できます。\
リンクされた項目の更新について詳しくは、[Jira と Adobe Workfront の間のリンクされた項目を更新](../../workfront-integrations-and-apps/use-workfront-with-jira/update-linked-items-between-jira-wf.md)を参照してください。

手動で [!DNL Jira] イシューを [!DNL Workfront] 項目にリンクするには、次の手順に従います。

1. （条件付き） [!DNL Workfront] にログインし、[!DNL Jira] のイシューにリンクするイシューまたはタスクを見つけます。
1. （条件付き） **タスクの詳細** または **イシューの詳細** タブの **基本情報** セクションで、Workfrontの項目の **[!UICONTROL 参照番号]** をコピーします。

   または

   項目のアドレスバーから、Workfront内の項目の **URL** をコピーします。

   >[!IMPORTANT]
   >
   >組織がAdobe Unified Experience にオンボーディングされている場合、Workfrontの項目を Jira にリンクするには **参照番号** を使用する必要があります。 （URL オプションは使用できますが、使用するとエラーが返されます。） 統合エクスペリエンスについて詳しくは、[Workfront用Adobe統合エクスペリエンス ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md) を参照してください。
   >
   >Adobe Unified Experience 以外の組織の場合、URL は変わる可能性があるので、「URL」オプションを使用することはお勧めしません。

   >[!NOTE]
   >
   >[!DNL Workfront] にログインするには、[!DNL Workfront] ライセンスが必要です。それ以外の場合は、[!DNL Workfront] ユーザーからこの情報の提供を受ける必要があります。

1. [!DNL Jira] で、手動で [!DNL Workfront] 項目にリンクするイシューに移動します。
1. 右 [!DNL Workfront] のパネルに、リンク先の **[!UICONTROL 項目の]** 参照番号 **または** URL[!DNL Workfront] を貼り付けます。

1. **[!UICONTROL リンク]** をクリックします。 2 つの項目がリンクされ、[!DNL Workfront] の右側のパネルに [!DNL Workfront] 項目からの情報が入力されます。

   デフォルトでは、右 [!DNL Workfront] のパネルの [!DNL Jira] に次の [!DNL Workfront] フィールドが表示されます。

   * 項目の **[!UICONTROL 名前]**。 [!DNL Workfront] 項目にアクセスするには、パネル内の名前をクリックします。
   * **[!UICONTROL プロジェクト名]**。
   * 項目の **[!UICONTROL ステータス]**。
   * アイテムの **[!UICONTROL 優先度]**。
   * [!DNL Workfront] に作成された日付。
   * 品目の **[!UICONTROL 予定時間数]**。
   * **[!UICONTROL 参照番号]**。 [!DNL Workfront] 項目にアクセスするには、パネルの **参照番号** をクリックします。

   追加のフィールドを右側のパネルに表示する方法については、「設定 [!DNL Jira]」の「[!DNL Workfront] と [ の項目間のフィールド同期の設定  [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md) を参照してください。 統合に関連づけられた [!DNL Workfront] 管理者からのコメントは、新しく [!DNL Jira] 項目が作成されたことを確認するために、[!DNL Jira] イシューの「**[!DNL Workfront]**」タブに投稿されます。コメントには、[!DNL Jira] イシューへのリンクが含まれます。

## [!DNL Jira] と [!DNL Workfront] 間の項目のリンクを解除

[!DNL Jira] と [!DNL Workfront] の間のリンクされた項目は、[!DNL Jira] で手動でリンクを解除できます。 [!DNL Workfront] で [!DNL Jira] から [!DNL Workfront] 項目のリンクを解除することはできません。

手動でリンクされた項目のリンクを解除するには、次のアクセス権が必要です。

* 自分が手動で項目をリンクしたユーザーです。
* [!DNL Jira] のシステム管理者です。

>[!NOTE]
>
>[!DNL Workfront] 管理者のみが、自動でリンクされた項目のリンクを解除できます。

[!DNL Workfront] 項目から [!DNL Jira] イシューのリンクを解除するには、次の手順に従います。

1. Jira にログインします。
1. [!DNL Workfront] のタスクまたはイシューにリンクされているイシューに移動します。
1. 右側のパネルの **Workfront** に移動します。
1. **[!UICONTROL リンク解除]** アイコン、**[!UICONTROL リンク解除]** の順にクリックします。 以前にリンクされた [!DNL Jira] と [!DNL Workfront] の項目のリンクが解除されます。

   将来更新されるフィールド、コメント、ドキュメントは、他のアプリケーションの以前の対応物では更新されません。
