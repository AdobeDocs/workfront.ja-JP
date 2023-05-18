---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Experience Manager Assets Essentials 統合でのワークフローの使用
description: Experience Manager Assets Essentials 統合でのワークフローの使用
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
source-git-commit: 9080dfe7e46a3780d493b59c8f2a3c4efbc011e7
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 0%

---

# Experience Manager Assets統合でのワークフローの使用

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。 この機能は、プレビューサンドボックス環境でのみ使用できます。</span>

ワークフローとは、WorkfrontをAdobe Experience Manager as a Cloud Serviceに接続する一連のアクションです。 Workfrontの管理者は、Workfrontでワークフローを設定した後、それらをプロジェクトテンプレートに割り当てることができます。 ワークフローが割り当てられているプロジェクトテンプレートを使用してプロジェクトを作成すると、ワークフローで定義されたアクションがトリガーされます。

>[!NOTE]
>
>ワークフローは、Adobe Experience Manager as a Cloud Service統合でのみ使用できます。 これらは、Adobe Experience Manager Assets Essentialsとの統合では使用できません。


## アクセス要件

以下が必要です。

<table>
  <tr>
   <td><strong>Adobe Workfront plan*</strong>
   </td>
   <td>任意
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfrontライセンス*</strong>
   </td>
   <td>リクエスト以上
   </td>
  </tr>
  <tr>
   <td><strong>製品</strong>
   </td>
   <td><p>Experience Manager AssetsまたはAssets Essentialsがあり、Admin Consoleでユーザーとして製品に追加される必要があります。</p><p>リンクされたフォルダーを作成するには、Adobe Experience Managerのリポジトリへの書き込みアクセス権が必要です。</p>&gt;
   </td>
  </tr>
  <tr>
   <td><strong>アクセスレベル設定*</strong>
   </td>
   <td>ドキュメントへのアクセスを編集
<p>
<strong>注意： </strong>まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <strong>カスタムアクセスレベルの作成または変更</strong>.
   </td>
  </tr>
  <tr>
   <td><strong>オブジェクト権限</strong>
   </td>
   <td>プロジェクトでアクセス権を管理する 
<p>
追加のアクセス権のリクエストについて詳しくは、 <strong>オブジェクトへのアクセスのリクエスト </strong>.
   </td>
  </tr>
</table>

## 前提条件

始める前に

* Workfront管理者は、Adobe Experience Manager統合でワークフローを設定する必要があります。 詳しくは、 [Experience Manager Assets統合の設定](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).

## テンプレートへのワークフローの追加

プロジェクトテンプレートにワークフローを追加できます。 ワークフローは、テンプレートから作成されたすべてのプロジェクトに適用されます。

1. <!-- main menu snippet??--> 「 **テンプレート** メインメニューで、リストからテンプレートを選択します。
1. クリック **Experience Manager Assets** をクリックします。

   >[!NOTE]
   >
   >左側のナビゲーションに「 Experience Manager Assets 」セクションが表示されていない場合、Workfront管理者が組織のワークフローを有効にしていません。 <!--Is this right?-->

1. 内 **自動ワークフローフィールドの統合を選択**&#x200B;で、このテンプレートから作成されるプロジェクトに使用するワークフローとの統合を選択します。
1. （オプション）このテンプレートから作成されるプロジェクトに適用するワークフロー値を編集します。

   例えば、デフォルト値以外の場所にリンクフォルダを作成するには、リンクフォルダの場所を入力します。

   セットアップのExperience Manager領域でアクティブ化されたワークフローのみが、テンプレートまたはプロジェクトで使用できます。

1. 変更内容は自動的に保存されます。 <!-- do they though??-->

## プロジェクトへのワークフローの追加

プロジェクトの作成時にワークフローを追加したり、既存のプロジェクトにワークフローを追加したりできます。 どちらの場合も、プロジェクトテンプレートを使用してワークフローを追加します。

### プロジェクト作成時のワークフローの追加

1. プロジェクトの作成を開始します。

   手順については、 [テンプレートを使用したプロジェクトの作成](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

1. プロジェクトのテンプレートを選択する場合は、このプロジェクトで使用するワークフローを含むテンプレートを選択します。
1. （オプション）プロジェクトのワークフロー値を編集します。詳しくは、 [プロジェクト内のワークフロー値の編集](#edit-workflow-values-in-a-project).

   セットアップのExperience Manager領域でアクティブ化されたワークフローのみが、テンプレートまたはプロジェクトで使用できます。


### 既存のプロジェクトにワークフローを追加する

1. プロジェクトへのテンプレートの追加を開始します。

   手順については、 [プロジェクトへのテンプレートの添付](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

1. プロジェクトのテンプレートを選択する場合は、このプロジェクトで使用するワークフローを含むテンプレートを選択します。
1. （オプション）プロジェクトのワークフロー値を編集します。詳しくは、 [プロジェクト内のワークフロー値の編集](#edit-workflow-values-in-a-project).

### プロジェクト内のワークフロー値の編集

プロジェクトレベルでワークフロー値を編集できます。 プロジェクトレベルのワークフロー値は、プロジェクトテンプレートで設定された値を上書きします。この値は、Adobe Experience Manager Assets 統合で設定されたデフォルト値に優先します。

すべてのワークフロー値は、次の場所にあります。

* プロジェクトを作成またはプロジェクトを編集ウィンドウの「ワークフロー」セクション。
* 左ナビゲーションのAdobe Experience Managerセクション。


   >[!NOTE]
   >
   >これらの領域が表示されない場合、Workfront管理者は組織のワークフローを有効にしていません。

#### リンクされたフォルダー

リンクされたフォルダーのワークフローを編集するには：

1. 切り替え **[!UICONTROL リンクされたフォルダーを作成]** オン。
1. フォルダーパスを選択して、この統合に関連付けるリンクされたすべてのフォルダーを指定します。
1. 「プロジェクトを作成」または「プロジェクトを編集」ウィンドウを使用している場合は、「保存」をクリックします。

   または

   「Adobe Experience Manager」領域にいる場合、変更は自動的に保存されます。 <!--Do they though?-->

