---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: リクエストタイプの設定
description: プロジェクトの作業中に、予期しないイベントが発生することがあります。 これらの予期しないイベントは、特定のプロジェクトまたはタスクの問題として記録できます。 リクエストキューとして指定されたプロジェクトの問題として記録されたリクエストを送信することもできます。 問題とリクエストは、Adobe Workfrontで交換可能と見なされます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 81e74a70-ea7e-4ed8-8b30-f01df0e73645
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# リクエストタイプの設定

プロジェクトの作業中に、予期しないイベントが発生することがあります。 これらの予期しないイベントは、特定のプロジェクトまたはタスクの問題として記録できます。 リクエストキューとして指定されたプロジェクトの問題として記録されたリクエストを送信することもできます。 問題とリクエストは、Adobe Workfrontで交換可能と見なされます。

での問題の作成に関する情報 [!DNL Workfront]を参照してください。 [イシューの作成](../../../manage-work/issues/manage-issues/create-issues.md). でのリクエスト作成について詳しくは、 [!DNL Workfront]を参照してください。 [作成して送信 [!DNL Adobe Workfront] リクエスト](../../../manage-work/requests/create-requests/create-submit-requests.md). 要求タイプとプロジェクトの関連付けについては、 [プロジェクトの要求タイプの定義](../../../manage-work/requests/create-and-manage-request-queues/define-request-types-for-project.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td>[!UICONTROL プラン ]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>次の条件を満たす必要があります。 [!DNL Workfront] 管理者。</p> <p><b>注意</b>:まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者はアクセスレベルを変更できます。詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
THIS IS DRAFTED IN FLARE
<h2>Set what issue or request types are allowed for a project</h2>
<p>You can organize the kind of issues or requests that are logged in Workfront by Request Types. This organization is useful for reporting reasons and for helping users understand what kind of unexpected work might occur during the lifetime of a project.</p>
<p>You can specify the type of requests that can be logged on a project when you configure the <strong>Queue Details</strong> area for the project. </p>
<ol>
<li value="1"> <p> Click <strong>Projects</strong> in the Main Menu. <img src="assets/main-menu-icon.png"> </p> </li>
<li value="2">Click the name of the project to open it.</li>
<li value="3"> In the left panel, click <strong>Queue Details</strong>. </li>
<li value="4"> <p>In the <strong>Queue Properties</strong> section, select the <strong>Request Types</strong> you want for the project.</p> <note type="note">
You must have at least one request type selected. You can select multiple request types.
</note> </li>
<li value="5"> <p>Click <strong>Save</strong>.</p> <p>The request types you specified will be available to select when you enter a new issue on a task or a project, or when you submit a new request to the project.</p> </li>
</ol>
</div>
-->

## リクエストタイプの名前のカスタマイズ

As a [!DNL Workfront] 管理者は、システムでリクエストタイプの名前を設定できます。 新しい名前は、 [!DNL Workfront] ここで、 **[!UICONTROL 問題のタイプ]** または **[!UICONTROL リクエストタイプ]** フィールドの表示：

* 内 **[!UICONTROL キューの詳細]** 問題またはリクエストを受け取るプロジェクトの領域。
* 1 つのリクエストキューに対して複数のリクエストタイプが選択されている場合、 **[!UICONTROL 新しい問題] フォーム** 内 **[!UICONTROL 問題のタイプ]** フィールドに入力します。

   での問題の作成について詳しくは、 [!DNL Workfront]を参照してください。  [イシューの作成](../../../manage-work/issues/manage-issues/create-issues.md)

   でのリクエスト作成について詳しくは、 [!DNL Workfront]を参照してください。  [作成して送信 [!DNL Adobe Workfront] リクエスト](../../../manage-work/requests/create-requests/create-submit-requests.md).

* の **[!UICONTROL トピックの詳細をキュー]** フォームを開きます。\
   キュートピックの作成の詳細については、 [キュートピックを作成](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

リクエストタイプの名前をカスタマイズするには：

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. クリック **[!UICONTROL プロジェクト環境設定]** > **[!UICONTROL ステータス]**.

1. 次をクリック： **[!UICONTROL 問題]** タブをクリックします。
1. の上部 **[!UICONTROL 問題]** 「 」タブで、リクエストタイプの名前の上にマウスポインターを置いて、 **[!UICONTROL 編集]** 表示されるアイコン。

   ![](assets/edit-request-type-name-nwe.png)

1. 表示されるボックスに新しい名前を入力し、 **[!UICONTROL 入力]**.

## 様々なリクエストタイプ内での問題ステータスの設定

各リクエストタイプを異なる問題ステータスに関連付けることができます。 また、イシューのタイプに応じて、イシューに対するステータスの表示順を変更することもできます。

問題ステータスのデフォルトの順序の変更と問題ステータスの設定について詳しくは、 [ステータスの作成または編集](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) セクション [ステータスの作成または編集](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
