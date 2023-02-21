---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: 項目をリンク [!DNL Adobe Workfront] および [!DNL Jira]
description: 次のリンクが可能： [!DNL Jira] 問題 [!DNL Adobe Workfront] タスクまたは問題は、自動または手動で実行します。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 1c37f361-e866-4ac6-b672-408848a80ed6
source-git-commit: f22a67cd3235a3111f7b874637ec05f8299de271
workflow-type: tm+mt
source-wordcount: '1160'
ht-degree: 0%

---

# 項目をリンク [!DNL Adobe Workfront] および [!DNL Jira]

次のリンクが可能： [!DNL Jira] 問題 [!DNL Adobe Workfront] タスクまたは問題は、自動または手動で実行します。

次の中の 1 つの項目のみ： [!DNL Workfront] は [!DNL Jira]. リンクできません [!DNL Workfront] 項目を複数に [!DNL Jira] 問題は一つも [!DNL Jira] 複数の [!DNL Workfront] 項目。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] 計画]</a>*</td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] ライセンスの概要</a>*</td> 
   <td> <p>計画</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jira アクセス</td> 
   <td> <p>システム管理者のアクセス権</p> <p><b>重要</b>

で別々のシステム管理者アカウントを作成することをお勧めします。 [!DNL Jira] および [!DNL Workfront] ユーザーに付随する可能性のある既存の統合を使用するのではなく、この統合専用にする場合。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>次の条件を満たす必要があります。 [!DNL Workfront] 管理者。 詳しくは、 [!DNL Workfront] 管理者向け： <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> <p><b>メモ</b>

まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者はアクセスレベルを変更できます。詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## 前提条件

次の間で項目をリンクする前に [!DNL Workfront] および [!DNL Jira]を

* インストール [!DNL Workfront] 対象 [!DNL Jira]

   Jira 用Workfrontのインストール手順については、 [Adobe Workfront for Jira のインストール](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* 設定 [!DNL Workfront] ジラのために

   Jira 用のWorkfrontの設定手順については、 [Jira 用Adobe Workfrontの設定](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## 自動リンク [!DNL Workfront] 項目 [!DNL Jira] 問題

As a [!DNL Workfront] 管理者は、 [!DNL Jira] タスクまたは問題で特定の条件が満たされるたびに [!DNL Workfront]. 201.Workfrontと [!DNL Jira] 項目がリンクされます。

設定が完了したら、 [!DNL Workfront] Jira の場合、 [!DNL Workfront] トリガーを一致させるために、新しい項目が [!DNL Jira].\
Workfront項目を作成および更新するWorkfrontユーザーは、 [!DNL Jira] のアイテムのトリガーを許可するライセンス [!DNL Jira].

Jira の問題を自動的に作成するトリガーの定義について詳しくは、  [設定 [!DNL Adobe Workfront] ジラのために](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

>[!NOTE]
>
>次の項目を作成できます。 [!DNL Jira] テンプレートをプロジェクトにアタッチすると、項目が自動的に追加されます。 テンプレートに、 [!DNL Jira] トリガー、新しいタスクが新しいタスクを生成する [!DNL Jira] 問題。

自動的なリンク [!DNL Workfront] に対する問題 [!DNL Jira] 問題は、 [!DNL Workfront] タスクを [!DNL Jira] 問題。

自動的に [!DNL Workfront] タスクを [!DNL Jira] 問題：

1. 次を確認します。 [!DNL Jira] システム管理者が自動作成用のトリガーを設定しました [!DNL Jira] 問題： [!DNL Workfront] 項目が割り当てられ、次の場所にログインする： [!DNL Workfront] タスクを作成できるアクセスレベルを持つ

   タスクへのアクセスについて詳しくは、 [タスクへのアクセス権の付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

1. プロジェクトに移動し、「 」を選択します。 **[!UICONTROL タスク]** ![](assets/tasks-icon-in-left-panel-14x14.png) をクリックします。

1. クリック **[!UICONTROL 新規タスク]**

   または

   既存のタスクを選択し、「 **編集**.

1. タスクに使用できるフィールドを指定または更新します。
1. クリック **[!UICONTROL 割り当て]** タスクを、 [!DNL Jira] 統合とも呼ばれます。

1. クリック **変更を保存**.

   新しいタスクがWorkfrontに作成されます。

   内 **[!UICONTROL 更新]** 新しいタスクの領域に、新しいイシューが [!DNL Jira].

1. （オプション）Jira イシューへのリンクをクリックして、Jira で開きます。

   または

   次をクリック： **[!UICONTROL ジラに移動]** リンク **[!UICONTROL 統合]** 領域 **[!UICONTROL 詳細]** セクションまたはタスクまたはイシューのヘッダーを使用して、 [!DNL Jira] 問題。

   システム管理者またはグループ管理者が [!UICONTROL 統合] フィールドをレイアウトテンプレートに追加して、タスクまたはイシューのヘッダーに表示します。 詳しくは、 [レイアウトテンプレートを使用したオブジェクトヘッダーのカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   任意 [!DNL Jira] ユーザーは、次から自動的に作成されたアイテムの作業をすぐに開始できます： [!DNL Workfront] 更新は次の場所に転送されます： [!DNL Workfront] 免許を必要とせずに [!DNL Workfront] そうする必要がある。

   自分が as a として使用するフィールドのみ [!DNL Workfront] 管理者が [!DNL Workfront] アドオンが更新されました。

   Workfrontと Jira 間のフィールドの同期について詳しくは、 [Jira 用Workfrontの設定](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#configuring-the-add-on-for-jira) セクション  [Jira 用Adobe Workfrontの設定](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

   >[!NOTE]
   >
   >この [!DNL Jira] 問題は [!DNL Jira] Workfrontから自動的に作成されたとき。

## 手動リンク [!DNL Jira] 問題 [!DNL Workfront] 項目

項目が [!DNL Jira] および [!DNL Workfront]を使用する場合、 [!DNL Jira] 既存の [!DNL Workfront] タスクまたは問題。\
手動で [!DNL Workfront] 項目： [!DNL Workfront] 既存の [!DNL Jira] 項目。

>[!NOTE]
>
>この [!DNL Jira] 問題は、 [!DNL Workfront] 統合： [!DNL Jira] オンプレミス：\
>Workfrontから Jira へのワークフローのトリガーの設定について詳しくは、 [Workfrontの項目を Jira の問題に自動的にリンク](#automatically-link-workfront-items-to-jira-issues).

条件 [!DNL Workfront] および [!DNL Jira] 項目がリンクされ、ある項目の特定のフィールドは、別の項目の特定のフィールドを自動的に更新できます。\
リンクされた項目の更新の詳細については、 [Jira とAdobe Workfrontの間のリンクされた項目を更新](../../workfront-integrations-and-apps/use-workfront-with-jira/update-linked-items-between-jira-wf.md).

手動でリンクするには [!DNL Jira] 問題 [!DNL Workfront] 項目：

1. （条件付き）にログインします。 [!DNL Workfront] リンク先のタスクまたはイシューを検索します [!DNL Jira] 問題。
1. （条件付き）項目のアドレスバーから、 **URL** Workfrontの項目の

   または

   次の [!UICONTROL 詳細] 領域、コピー **[!UICONTROL 参照番号]** Workfrontの項目の

   >[!NOTE]
   >
   >次をお持ちの場合は、 [!DNL Workfront] にログインするためのライセンス [!DNL Workfront]. それ以外の場合は、 [!DNL Workfront] ユーザーがこの情報をユーザーに提供する必要があります。

1. In [!DNL Jira]をクリックし、 [!DNL Workfront] 項目。
1. 内 [!DNL Workfront] 右側のパネル、 **URL** または **[!UICONTROL 参照番号]** の [!DNL Workfront] リンク先の項目です。

1. クリック **[!UICONTROL リンク]**.

   2 つの項目がリンクされ、 [!DNL Workfront] 右側のパネルに、 [!DNL Workfront] 項目。

   以下 [!DNL Workfront] フィールドは [!DNL Jira]( デフォルトでは、 [!DNL Workfront] 右パネル：

   * この **[!UICONTROL 名前]** 項目の：次にアクセス： [!DNL Workfront] 項目を選択するには、パネル内の名前をクリックします。
   * **[!UICONTROL プロジェクト名]**
   * この **[!UICONTROL ステータス]** 項目の
   * この **[!UICONTROL 優先度]** 項目の
   * 作成日 [!DNL Workfront]
   * この **[!UICONTROL 予定時間]** 項目の
   * この **[!UICONTROL 参照番号]**:次にアクセス： [!DNL Workfront] 項目をクリック [!UICONTROL 参照番号] 」と入力します。

右側のパネルに追加のフィールドを表示できるようにする方法について詳しくは、 [次の間のフィールド同期の設定 [!DNL Jira] および [!DNL Workfront] 項目](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#setting-up-field-synchronization) セクション [設定 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md). 次からのコメント： [!DNL Workfront] 統合に関連付けられた管理者は、 **[!DNL Workfront]** タブ [!DNL Jira] 新たに確認する問題 [!DNL Jira] 項目が作成されました。 コメントには、 [!DNL Jira] 問題。

## 間の項目のリンクを解除 [!DNL Jira] および [!DNL Workfront]

次の間にリンクされた項目： [!DNL Jira] および [!DNL Workfront] 手動でリンクを解除できる [!DNL Jira].\
リンクを解除することはできません [!DNL Workfront] 項目から [!DNL Jira] 対応する [!DNL Workfront].

手動でリンクされた項目のリンクを解除するには、次のアクセス権が必要です。

* 項目を手動でリンクしたユーザーです
* あなたは [!DNL Jira] システム管理者

a のみ [!DNL Workfront] 管理者は、自動的にリンクされた項目のリンクを解除できます。

リンクを解除するには [!DNL Jira] ～からの問題 [!DNL Workfront] 項目：

1. In [!DNL Jira]、 [!DNL Workfront] タスクまたは問題。
1. 次に移動： [!DNL Workfront] 右側のパネルをクリックし、 **[!UICONTROL リンク解除]** アイコンをクリックし、 **[!UICONTROL リンク解除]**.

   以前にリンクされた [!DNL Jira] および [!DNL Workfront] 項目のリンクが解除されました。 今後、それらに対して個別に更新される可能性のあるフィールド、コメント、ドキュメントは、他のアプリケーションの以前の対応するドキュメントには更新されません。
