---
product-area: projects
navigation-topic: use-lists
title: のリスト内のインライン編集項目 [!DNL Adobe Workfront]
description: オブジェクトがリストまたはレポートに表示されるときは、オブジェクトをインラインで編集できます。 リストまたはレポートに表示されるオブジェクトの情報を編集すると、オブジェクトは直ちに更新されます。
feature: Get Started with Workfront
author: Lisa
exl-id: a94b5aaf-71de-4fcd-946b-459ca3edf7e4
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 0%

---

# のリスト内のインライン編集項目 [!DNL Adobe Workfront]

オブジェクトがリストまたはレポートに表示されるときは、オブジェクトをインラインで編集できます。 リストまたはレポートに表示されるオブジェクトの情報を編集すると、オブジェクトは直ちに更新されます。

オブジェクトに添付されていないカスタムフォームに含まれるフィールドをインライン編集すると、カスタムフォームは自動的にオブジェクトに追加されます。 フィールドが複数のカスタムフォーム上に存在する場合、最も新しく更新されたカスタムフォームがオブジェクトに添付されます。

リストについて詳しくは、 [のリストの基本を学ぶ [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

リストまたはレポートに表示されるほとんどのオブジェクトはインラインで編集できますが、 [!DNL Adobe Workfront]には、次のような制限があります。

* 計算フィールドや [!DNL Workfront] 計算である組み込みフィールド。
* リスト内のオブジェクトに直接関連付けられているフィールドのみを編集できます。 リスト内のオブジェクトに関連付けられたオブジェクトに属するフィールドは編集できません。\
   たとえば、タスクレポートでタスクのステータスを編集することはできますが、同じレポートでタスクが関連付けられているプロジェクトの名前を編集することはできません。 プロジェクトの名前は、プロジェクトレポートでのみ編集できます。
* リストのビューにデフォルトの通貨が表示されていない場合、編集フィールドをインライン化できません。\
   デフォルトの通貨の表示について詳しくは、 [ユニーク通貨でレポートを編集](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md#editing-reports-with-unique-currencies) 記事内 [一意の為替レートを使用した財務データレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

* リストに表示されるフラグとアイコンは編集できません。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計画*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL Review] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>リストが含まれる領域への [!UICONTROL 編集 ] アクセス</p> <p>例えば、プロジェクト内の編集タスクをインライン化するには、プロジェクトへの [!UICONTROL 編集 ] アクセス権が必要です。</p> <p>注意：まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合）<br>を参照してください。 [!DNL Workfront] 管理者は、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>[!UICONTROL 管理 ]</p> <p>また、カスタムフィールド、ステータスなど、特定のフィールドを編集する権限が必要です。</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## オブジェクトをインラインで編集

1. インライン編集するオブジェクトのリストに移動します。

   リストには、リスト内のオブジェクトに関連付けられたオブジェクトに属するオブジェクトまたはフィールドに属するフィールドが表示されます。

1. 編集するオブジェクトを見つけ、リスト内の任意のフィールド内をクリックします。

   >[!TIP]
   >
   >複数のページがある場合は、次を使用してオブジェクトを特定できます。
   >
   >   
   >   
   >   * **ページ編集**:前後の矢印をクリックして、ページ間を移動します。\
      >     リストの右下隅にある、 [!UICONTROL ページ編集] リストをスクロールすると、領域は固定状態のままです。
   >   * **クイックフィルター**:フィルターアイコンをクリックするか、Alt+F キーを押してクイックフィルターを開き、テキストを入力して入力したテキストを含む項目のみを表示します。\
      >     クイックフィルターはリストツールバーにあります。 詳しくは、 [クイックフィルターをリストに適用する](../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).



   フィールドが編集可能な場合は、リストに表示されるフィールドとその他すべてのフィールドが編集可能なセルに変換されます。

   ![](assets/nwe-editable-cells-350x131.png)

1. このセル内の情報を編集し、 [!UICONTROL 入力].

   >[!NOTE]
   >
   >カスタムフィールドを書式設定を許可するように設定している場合は、更新されたリストのフィールドをインライン編集する際に、テキストを太字、斜体または下線で編集できます。\
   >カスタムフィールドの書式設定については、 [カスタムフォームの作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).\
   >更新されたリストについて詳しくは、この記事の「更新されたリストと従来のリストの違い」の節を参照してください [のリストの基本を学ぶ [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

1. 押す [!UICONTROL タブ] をクリックして、次の編集可能なセルに移動します。
1. （条件付き）編集内容を保存できず、セルが赤で囲まれている場合は、フィールド内をクリックして、セルの横に表示される検証メッセージを確認し、適切な更新を行います。

   最も一般的に、この問題は、誤った形式が使用されている場合や、必須フィールドが空白のままの場合に発生します。

1. すべてのセルの変更が終了したら、 [!UICONTROL 入力] 変更を保存します。
