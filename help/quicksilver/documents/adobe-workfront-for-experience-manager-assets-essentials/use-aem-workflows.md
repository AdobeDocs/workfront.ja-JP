---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Experience Manager Assets Essentials 統合でのワークフローの使用
description: Experience Manager Assets Essentials 統合でのワークフローの使用
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4c1e5ec1-3fd1-4527-ba8a-9db1a2350f69
source-git-commit: 706e531be6f6269a927f94fee4d2c37d9367c9af
workflow-type: tm+mt
source-wordcount: '816'
ht-degree: 82%

---

# Experience Manager Assets 統合でのワークフローの使用

ワークフローとは、Workfront を Adobe Experience Manager as a Cloud Service に接続する一連のアクションです。Workfront 管理者は、Workfront でワークフローを設定し、プロジェクトテンプレートに割り当てることができます。ワークフローが割り当てられているプロジェクトテンプレートを使用してプロジェクトを作成すると、ワークフローで定義されたアクションがトリガーされます。

>[!NOTE]
>
>ワークフローを使用できるのは Adobe Experience Manager as a Cloud Service 統合のみで、Adobe Experience Manager Assets Essentials との統合では使用できません。


## アクセス要件

以下が必要です。

<table>
  <tr>
   <td><strong>Adobe Workfront プラン*</strong>
   </td>
   <td>任意
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront ライセンス*</strong>
   </td>
   <td>リクエスト以上
   </td>
  </tr>
  <tr>
   <td><strong>製品</strong>
   </td>
   <td><p>Experience Manager Assets as a Cloud Service または Assets Essentials を使用するには、Admin Console に製品にユーザーとして追加されていることが必要です。</p><p>Adobe Experience Managerのリポジトリへの書き込みアクセス権が必要です。</p>
   </td>
  </tr>
  <tr>
   <td><strong>アクセスレベル設定*</strong>
   </td>
   <td>ドキュメントへのアクセスを編集
<p>
<strong>メモ</strong>：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<strong>カスタムアクセスレベルの作成または変更</strong>を参照してください。
   </td>
  </tr>
  <tr>
   <td><strong>オブジェクトの権限</strong>
   </td>
   <td>プロジェクトでのアクセス権以上の管理 
<p>
追加のアクセス権のリクエストについて詳しくは、<strong>オブジェクトへのアクセス権のリクエスト</strong>を参照してください。
   </td>
  </tr>
</table>

## 前提条件

開始する前に、

* Workfront 管理者は、Adobe Experience Manager 統合でワークフローを設定する必要があります。詳しくは、[Experience Manager Assets as a Cloud Service 統合の設定](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional)を参照してください。

## テンプレートへのワークフローの追加

ワークフローはプロジェクトテンプレートに追加することが可能で、。テンプレートから作成されたすべてのプロジェクトに適用されます。

1. 「メインメニュー」で「**テンプレート**」をクリックしてテンプレートを開き、リストからテンプレートを選択します。
1. 左側のナビゲーションパネルで「**Experience Manager Assets**」をクリックします。

   >[!NOTE]
   >
   >左側のナビゲーションに「Experience Manager Assets」セクションが表示されていない場合は、Workfront 管理者が組織のワークフローを有効にしていません。<!--Is this right?-->

1. 「**自動化されたワークフローの統合を選択**」フィールドで、このテンプレートから作成されるプロジェクトに使用するワークフローとの統合を選択します。
1. （オプション）このテンプレートから作成されるプロジェクトに適用するワークフローを編集します。

   特定のワークフローの手順については、 [プロジェクト内のワークフロー値の編集](#edit-workflow-values-in-a-project) 」を参照してください。

   テンプレートまたはプロジェクトで使用できるのは、「設定」の「Experience Manager」エリアでアクティベートされたワークフローのみです。

1. 変更内容は自動的に保存されます。<!-- do they though??-->

## プロジェクトへのワークフローの追加

プロジェクトの作成時にワークフローを追加したり、既存のプロジェクトにワークフローを追加したりできます。どちらの場合も、プロジェクトテンプレートを使用してワークフローを追加します。

### プロジェクト作成時のワークフローの追加

1. プロジェクトの作成を開始します。

   手順については、[テンプレートを使用したプロジェクトの作成](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md)を参照してください。

1. プロジェクトのテンプレートを選択する場合は、そのプロジェクトで使用するワークフローを含むテンプレートを選択します。
1. （オプション）プロジェクトのワークフローを編集します（[プロジェクトでのワークフローの編集](#edit-workflow-values-in-a-project)を参照）。

   テンプレートまたはプロジェクトで使用できるのは、「設定」の「Experience Manager」エリアでアクティベートされたワークフローのみです。


### 既存のプロジェクトへのワークフローの追加

1. プロジェクトへのテンプレートの追加を開始します。

   手順については、[プロジェクトへのテンプレートの添付](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md)を参照してください。

1. プロジェクトのテンプレートを選択する場合は、そのプロジェクトで使用するワークフローを含むテンプレートを選択します。
1. （オプション）プロジェクトのワークフローを編集します（[プロジェクトでのワークフローの編集](#edit-workflow-values-in-a-project)を参照）。

   テンプレートまたはプロジェクトで使用できるのは、「設定」の「Experience Manager」エリアでアクティベートされたワークフローのみです。

### プロジェクト内のワークフロー値の編集

プロジェクトレベルでワークフロー値を編集できます。プロジェクトレベルのワークフロー値は、プロジェクトテンプレートで設定された値を上書きします。これは、Adobe Experience Manager Assets 統合で設定されたデフォルト値に優先します。

すべてのワークフロー値は、次の場所にあります。

* プロジェクトを作成またはプロジェクトを編集ウィンドウのワークフローセクション。
* 左ナビゲーションの Adobe Experience Manager セクション。


  >[!NOTE]
  >
  >これらのエリアが表示されない場合、Workfront 管理者は組織のワークフローを有効にしていません。

#### リンクされているフォルダー

リンクされているフォルダーのワークフローを編集するには：

1. 切り替え **[!UICONTROL リンクされたフォルダーを作成]** 必要に応じてオンまたはオフにします。
1. （条件付き）リンクされたフォルダーを有効にする場合、すべてのリンクされたフォルダーをこの統合に関連付ける場所を示すフォルダーパスを選択します。
1. クリック **[!UICONTROL 保存]** を使用している場合、 [!UICONTROL プロジェクトを作成] または [!UICONTROL プロジェクトを編集] ウィンドウ

   または

   次の場合、 [!DNL Adobe Experience Manager area]を設定すると、変更内容は自動的に保存されます。 <!--Do they though?-->


#### アセットの公開

アセット公開のワークフローを編集するには：

1. 切り替え **アセットを自動的に公開** 必要に応じてオンまたはオフにします。
1. （条件付き）公開を有効にする場合、公開サービス、Brand Portal またはその両方に公開するかどうかを選択します。
1. クリック **[!UICONTROL 保存]** を使用している場合、 [!UICONTROL プロジェクトを作成] または [!UICONTROL プロジェクトを編集] ウィンドウ

   または

   次の場合、 [!DNL Adobe Experience Manager area]を設定すると、変更内容は自動的に保存されます。 <!--Do they though?-->


