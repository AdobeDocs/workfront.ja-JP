---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: ' [!DNL Adobe Workfront]  と  [!DNL Jira] 間で項目をリンク'
description: ' [!DNL Jira]  のイシューを、 [!DNL Adobe Workfront]  のタスクまたはイシューに、自動または手動でリンクできます。'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 1c37f361-e866-4ac6-b672-408848a80ed6
source-git-commit: f22a67cd3235a3111f7b874637ec05f8299de271
workflow-type: ht
source-wordcount: '1160'
ht-degree: 100%

---

# [!DNL Adobe Workfront] と [!DNL Jira] 間で項目をリンク

[!DNL Jira] のイシューを、[!DNL Adobe Workfront] のタスクまたはイシューに、自動または手動でリンクできます。

[!DNL Workfront] の中の 1 つの項目のみが、[!DNL Jira] 内の 1 つの項目にリンクできます。1 つの [!DNL Workfront] 項目を複数の [!DNL Jira] イシュー、または 1 つの [!DNL Jira] イシューを複数の [!DNL Workfront] 項目にリンクさせることはできません。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] プラン]</a>*</td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] ライセンスの概要</a>*</td> 
   <td> <p>プラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jira アクセス</td> 
   <td> <p>システム管理者のアクセス権</p> <p><b>重要</b>

ユーザーに関連付けられている既存のアカウントを使用するのではなく、この統合専用のシステム管理者アカウントを [!DNL Jira] と [!DNL Workfront] に個別に作成することをお勧めします。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>[!DNL Workfront] 管理者である必要があります。[!DNL Workfront] 管理者について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーへの完全な管理アクセス権の付与</a>を参照してください。</p> <p><b>メモ</b>

まだアクセス権がない場合は、[!DNL Workfront] 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## 前提条件

[!DNL Workfront] と [!DNL Jira] の項目をリンクさせる前に、次のことが必要です。

* [!DNL Jira] 用 [!DNL Workfront] をインストール

  Jira 用 Workfront のインストールについて詳しくは、[Jira 用 Adobe Workfront をインストール](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md)を参照してください。

* Jira 用 [!DNL Workfront] を設定

  Jira 用 Workfront の設定について詳しくは、[Jira 用 Adobe Workfront を設定](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)を参照してください。

## [!DNL Workfront] の項目を [!DNL Jira] のイシューに自動でリンク

[!DNL Workfront] 管理者は、[!DNL Workfront] のタスクまたはイシューで特定の条件を満たすたびに [!DNL Jira] のイシューを自動作成するトリガーを定義できます。Workfront と [!DNL Jira] の項目がリンクされます。

Jira 用 [!DNL Workfront]の設定を完了すると、[!DNL Workfront] で項目が作成または更新されてトリガーに一致したとき、[!DNL Jira] で新しい項目が自動作成されます。\
Workfront の項目を作成および更新する Workfront ユーザーには、[!DNL Jira] の項目作成をトリガーするための [!DNL Jira] ライセンスは必要ありません。

Jira のイシューを自動作成するトリガーの定義について詳しくは、[Jira 用  [!DNL Adobe Workfront]  を設定](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)を参照してください。

>[!NOTE]
>
>プロジェクトにテンプレートを添付することで、[!DNL Jira] 項目を自動作成できます。テンプレートに、[!DNL Jira] のトリガーに一致する割り当てを持つタスクが含まれる場合、新しいタスクによって [!DNL Jira] の新しいイシューが生成されます。

[!DNL Workfront] のイシューを [!DNL Jira] のイシューに自動でリンクすることと、[!DNL Workfront] のタスクを [!DNL Jira] のイシューに自動でリンクすることは同じです。

[!DNL Workfront] のタスクを [!DNL Jira] のイシューに自動でリンク

1. [!DNL Workfront] 項目が割り当てられたときに [!DNL Jira] のイシューを自動作成するトリガーを [!DNL Jira] システム管理者が設定したことを確認し、タスクの作成が許可されているアクセスレベルで [!DNL Workfront] にログインします。

   タスクへのアクセス権について詳しくは、[タスクへのアクセス権を付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)を参照してください。

1. プロジェクトに移動し、左側のパネルで&#x200B;**[!UICONTROL タスク]** ![](assets/tasks-icon-in-left-panel-14x14.png) をクリックします。

1. 「**[!UICONTROL 新規タスク]**」をクリックします。

   または

   既存のタスクを選択し、「**編集**」をクリックします。

1. タスクに使用できるフィールドを指定または更新します。
1. 「**[!UICONTROL 割り当て]**」をクリックし、[!DNL Jira] 統合でトリガーとして指定されたユーザー、役割またはチームにタスクを割り当てます。

1. 「**変更を保存**」をクリックします。

   新しいタスクが Workfront に作成されます。

   新しいタスクの&#x200B;**[!UICONTROL 更新]**&#x200B;エリアに、[!DNL Jira] にも新しいイシューが作成されたことを示すコメントが表示されます。

1. （オプション）Jira のイシューへのリンクをクリックして、Jira で開きます。

   または

   「**[!UICONTROL 詳細]**」セクションまたはタスクやイシューのヘッダーにある&#x200B;**[!UICONTROL 統合]**&#x200B;エリアの「**[!UICONTROL JIRA に移動]**」のリンクをクリックし、[!DNL Jira] のイシューを開きます。

   システム管理者またはグループ管理者がレイアウトテンプレートに[!UICONTROL 統合]フィールドを追加して、タスクまたはイシューのヘッダーに表示する必要があります。詳しくは、[レイアウトテンプレートを使用してオブジェクトヘッダーをカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)を参照してください。

   [!DNL Jira] ユーザーはすぐに [!DNL Workfront] から自動作成された項目の作業を開始でき、その更新は [!DNL Workfront] ライセンスがなくても [!DNL Workfront] に移行されます。

   自分が [!DNL Workfront] 管理者として [!DNL Workfront] アドオンの設定時に設定したフィールドのみが更新されます。

   Workfront と Jira 間のフィールドの同期について詳しくは、[Jira 用 Adobe Workfront を設定](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)の [Jira 用 Workfront を設定](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#configuring-the-add-on-for-jira)の節を参照してください。

   >[!NOTE]
   >
   >[!DNL Jira] のイシューは、Workfront から自動作成された場合、[!DNL Jira] のいずれのユーザーにも割り当てられません。

## [!DNL Jira] のイシューを [!DNL Workfront] 項目に手動でリンク

[!DNL Jira] および [!DNL Workfront] で互いに独立した項目を作成した後に、[!DNL Jira] のイシューを既存の [!DNL Workfront] のタスクまたはイシューに手動でリンクできます。\
[!DNL Workfront] 項目を、[!DNL Workfront] から既存の [!DNL Jira] 項目に手動でリンクすることはできません。

>[!NOTE]
>
>[!DNL Workfront] 統合でトリガーと識別されないプロジェクト上に [!DNL Jira] イシューが存在しない場合、[!DNL Jira] オンプレミスとの統合を利用して Workfront 項目に手動でリンクすることはできません。\
>Workfront から Jira へのワークフローのトリガー設定について詳しくは、[Workfront の項目を Jira のイシューに自動的にリンク](#automatically-link-workfront-items-to-jira-issues)を参照してください。

[!DNL Workfront] および [!DNL Jira] 項目がリンクされている場合、ある項目の特定のフィールドは、別の項目の特定のフィールドを自動的に更新できます。\
リンクされた項目の更新について詳しくは、[Jira と Adobe Workfront の間のリンクされた項目を更新](../../workfront-integrations-and-apps/use-workfront-with-jira/update-linked-items-between-jira-wf.md)を参照してください。

手動で [!DNL Jira] イシューを [!DNL Workfront] 項目にリンクするには、次の手順に従います。

1. （条件付き）[!DNL Workfront] にログインし、[!DNL Jira] イシューにリンクするイシューまたはタスクを検索します。
1. （条件付き）項目のアドレスバーから、Workfront の項目の **URL** をコピーします。

   または

   [!UICONTROL 詳細]エリアから、Workfront の項目の&#x200B;**[!UICONTROL 参照番号]**&#x200B;をコピーします。

   >[!NOTE]
   >
   >[!DNL Workfront] にログインするには、[!DNL Workfront] ライセンスが必要です。それ以外の場合は、[!DNL Workfront] ユーザーからこの情報の提供を受ける必要があります。

1. [!DNL Jira] で、手動で [!DNL Workfront] 項目にリンクするイシューに移動します。
1. [!DNL Workfront] の右側のパネルで、**URL** またはリンクする [!DNL Workfront] 項目の&#x200B;**[!UICONTROL 参照番号]**&#x200B;をペーストします。

1. 「**[!UICONTROL リンク]**」をクリックします。

   2 つの項目がリンクされ、[!DNL Workfront] の右側のパネルに [!DNL Workfront] 項目からの情報が入力されます。

   次の [!DNL Workfront] フィールドは、[!DNL Workfront] の右側のパネルの [!DNL Jira] にデフォルトで表示されます。

   * 項目の&#x200B;**[!UICONTROL 名前]**：パネル内の名前をクリックすると、[!DNL Workfront] 項目にアクセスできます。
   * **[!UICONTROL プロジェクト名]**
   * 項目の&#x200B;**[!UICONTROL ステータス]**
   * 項目の&#x200B;**[!UICONTROL 優先度]**
   * [!DNL Workfront] で作成された日付
   * 項目の&#x200B;**[!UICONTROL 予定時間数]**
   * **[!UICONTROL 参照番号]**：パネルの[!UICONTROL 参照番号]をクリックすると、[!DNL Workfront] 項目にアクセスできます。

追加のフィールドを有効にして右側のパネルに表示する方法について詳しくは、[設定 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)の[ [!DNL Jira]  と  [!DNL Workfront]  項目間のフィールド同期を設定](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#setting-up-field-synchronization)の節を参照してください。統合に関連づけられた [!DNL Workfront] 管理者からのコメントは、新しく [!DNL Jira] 項目が作成されたことを確認するために、[!DNL Jira] イシューの「**[!DNL Workfront]**」タブに投稿されます。コメントには、[!DNL Jira] イシューへのリンクが含まれます。

## [!DNL Jira] と [!DNL Workfront] 間の項目のリンクを解除

[!DNL Jira] と [!DNL Workfront] 間でリンクされた項目は、[!DNL Jira] から手動でリンクを解除できます。\
[!DNL Workfront] で [!DNL Jira] から [!DNL Workfront] 項目のリンクを解除することはできません。

手動でリンクされた項目のリンクを解除するには、次のアクセス権が必要です。

* 項目を手動でリンクしたユーザーであること
* [!DNL Jira] システム管理者であること

[!DNL Workfront] 管理者のみが、自動でリンクされた項目のリンクを解除できます。

[!DNL Workfront] 項目から [!DNL Jira] イシューのリンクを解除するには、次の手順に従います。

1. [!DNL Jira] で、[!DNL Workfront] タスクもしくはイシューにリンクされたイシューに移動します。
1. [!DNL Workfront] の右側のパネルに移動し、**[!UICONTROL リンク解除]**&#x200B;アイコンをクリックして、「**[!UICONTROL リンク解除]**」をクリックします。

   以前にリンクされた [!DNL Jira] および [!DNL Workfront] 項目のリンクが解除されました。今後、個別に更新される可能性のあるフィールド、コメントまたはドキュメントは、他のアプリケーションでそれぞれの以前のバージョンで更新はされません。
