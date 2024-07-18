---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Experience Manager Assets Essentials 統合でのワークフローの使用
description: Experience Manager Assets Essentials 統合でのワークフローの使用
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4c1e5ec1-3fd1-4527-ba8a-9db1a2350f69
source-git-commit: b87839d6c6dbfe978a3e14ef4b448560742f95c3
workflow-type: tm+mt
source-wordcount: '1053'
ht-degree: 98%

---

# Experience Manager Assets 統合でのワークフローの使用

ワークフローとは、Workfront を Adobe Experience Manager as a Cloud Service に接続する一連のアクションです。Workfront 管理者は、Workfront でワークフローを設定し、プロジェクトテンプレートに割り当てることができます。ワークフローが割り当てられているプロジェクトテンプレートを使用してプロジェクトを作成すると、ワークフローで定義されたアクションがトリガーされます。

>[!NOTE]
>
>ワークフローを使用できるのは Adobe Experience Manager as a Cloud Service 統合のみで、Adobe Experience Manager Assets Essentials との統合では使用できません。


## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

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
   <td><p>Experience Manager Assets as a Cloud Service または Assets Essentials を使用するには、Admin Console に製品にユーザーとして追加されていることが必要です。</p><p>Adobe Experience Manager のリポジトリへの書き込みアクセス権が必要です。</p>
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

+++

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

   特定のワークフローの手順について詳しくは、[プロジェクト内のワークフロー値の編集](#edit-workflow-values-in-a-project)を参照してください。

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

>[!NOTE]
>
>プロジェクトの作成時に実行されるワークフロー（リンクされたフォルダーの作成など）は、テンプレートが既存のプロジェクトに添付されている場合は実行されません。テンプレートからプロジェクトを作成する場合にのみ実行されます。

1. プロジェクトへのテンプレートの追加を開始します。

   手順については、[プロジェクトへのテンプレートの添付](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md)を参照してください。

1. プロジェクトのテンプレートを選択する場合は、そのプロジェクトで使用するワークフローを含むテンプレートを選択します。
1. （オプション）プロジェクトのワークフローを編集します（[プロジェクトでのワークフローの編集](#edit-workflow-values-in-a-project)を参照）。

   テンプレートまたはプロジェクトで使用できるのは、「設定」の「Experience Manager」エリアでアクティベートされたワークフローのみです。



### プロジェクト内のワークフロー値の編集

プロジェクトレベルでワークフロー値を編集できます。プロジェクトレベルのワークフロー値は、プロジェクトテンプレートで設定された値を上書きします。これは、Adobe Experience Manager Assets 統合で設定されたデフォルト値に優先します。

すべてのワークフロー値は、次の場所にあります。

* プロジェクトを作成またはプロジェクトを編集ウィンドウのワークフローまたはリンクされているフォルダーセクション。
* 左ナビゲーションの Adobe Experience Manager セクション。


  >[!NOTE]
  >
  >これらのエリアが表示されない場合、Workfront 管理者は組織のワークフローを有効にしていません。



#### リンクされているフォルダー

>[!NOTE]
>
>リンクされているフォルダーはプロジェクトの作成時に作成されるので、既存のプロジェクトでリンクされているフォルダーのワークフローを編集しても効果はありません。プロジェクトの作成時にこれらの値を編集すると、期待どおりに機能します。

リンクされているフォルダーのワークフローを編集するには：

1. 必要に応じて、**[!UICONTROL リンクされたフォルダーを作成]**&#x200B;をオンまたはオフに切り替えます。オンにすると、リンクされているフォルダーの設定を編集できます。

   リンクされているフォルダーの設定について詳しくは、[[!UICONTROL Experience Manager Assets as a Cloud Service] 統合の設定](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)の記事の [Adobe Experience Manager にリンクされたフォルダーの作成](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md#create-adobe-experience-manager-linked-folders)を参照してください。

1. （オプション）プロジェクトに添付されたカスタムフォームに特定の値が存在する場合にのみフォルダーツリーを作成する場合は、そのフォルダツリーの「**フィルターを適用**」をクリックし、フィールド、フィールド、フィールド値を含むカスタムフォームを選択します。新しいプロジェクトに添付されたカスタムフォームのフィールドに選択した値が含まれている場合、フォルダーツリーが作成されます。
1. （オプション）フォルダー名を設定する際は、次のオプションから選択できます。

   * **名前**：フォルダーの名前を入力します。

   * **オブジェクトデータ**：プロジェクト名などのフォルダー名のソースを選択します。

   * **カスタムフォームデータ**：フォルダー名として使用するカスタムフォームデータを選択します。

     フォルダー名にカスタムフォームデータを使用することは、テンプレートレベルでのみ使用でき、統合レベルでは設定できません。

     プロジェクトに添付されているカスタムに存在しないカスタムデータに対してフォルダー名を設定した場合、フォルダー名としてランダムな ID が割り当てられます。

1. フォルダーツリーを表示するには、**プレビュー** ![プレビューアイコン](assets/preview-icon.png) アイコンをクリックします。
1. 「**[!UICONTROL 保存]**」をクリックします。

#### アセットの公開

アセットを公開するためのワークフローを編集するには：

1. 必要に応じて、**アセットを自動的に公開**&#x200B;のオンとオフを切り替えます。
1. （条件付き）公開を有効にする場合、公開サービス、Brand Portal またはその両方に公開するかどうかを選択します。
1. 「**[!UICONTROL 保存]**」をクリックします。
