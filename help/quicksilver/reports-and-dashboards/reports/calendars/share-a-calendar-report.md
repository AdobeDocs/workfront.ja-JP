---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: カレンダーレポートの共有
description: カレンダーを他のユーザーと共有して公開し、 [!DNL Adobe Workfront]  ライセンスを持たない人がカレンダーを表示できるようにできます。
author: Lisa
feature: Reports and Dashboards
exl-id: 77eed0fe-2d47-40c4-a03d-590f7fa17dbe
source-git-commit: e5a3024b1657942cd7abdfff76a7a6795127a4f5
workflow-type: ht
source-wordcount: '622'
ht-degree: 100%

---

# カレンダーレポートの共有

カレンダーを他のユーザーと共有して公開し、[!DNL Adobe Workfront] ライセンスを持たない人がカレンダーを表示できるようにできます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL Review] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>[!UICONTROL to Reports]、[!UICONTROL Dashboards] および [!UICONTROL Calendars] に対する [!UICONTROL View] 以上のアクセス権</p> <p>メモ：まだアクセス権がない場合は、[!DNL Workfront] 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>カレンダーレポートに対する [!UICONTROL View] 以上の権限、および共有するためのアクセス権</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## [!DNL Workfront] ユーザーとのカレンダーの共有 {#share-a-calendar-with-workfront-users}

カレンダーの共有は、他のオブジェクトの共有と似ています。[!DNL Adobe Workfront] でのオブジェクトの共有について詳しくは、[オブジェクトに対する共有権限の概要](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)を参照してください。

共有されているカレンダーの名前の横には、アスタリスク（&#42;）が表示されます。

[!DNL Workfront] 内でカレンダーを共有するには：

1. 共有するカレンダーに移動します。
1. 「**[!UICONTROL カレンダーのアクション]**」をクリックして、「**[!UICONTROL 共有]**」をクリックします。

1. **** へのアクセス権限付与の相手フィールドに、カレンダーを共有するユーザー、チーム、役割、グループまたは会社の名前を入力し、ドロップダウンリストに名前が表示されたらクリックします。\
   権限の設定について詳しくは、[オブジェクトに対する共有権限の概要](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)を参照してください。

1. （オプション）カレンダーへのアクセスを許可するユーザー、チーム、役割またはグループごとに手順 3 を繰り返します。
1. 手順 3 で追加した各ユーザー、チーム、役割、グループまたは会社に対する権限を指定するには、ドロップダウンメニューをクリックし、付与する権限レベルを選択します。

   * **[!UICONTROL 表示]：**&#x200B;ユーザーは、カレンダーを確認し、共有できます。

     ![カレンダーを表示アクセスで共有](assets/calendar-share-view-permissions-350x249.png)

   * **[!UICONTROL 管理]：** ユーザーは、カレンダーへのフルアクセス権を持ち、アクセスレベルで付与される管理権限を除き、すべての表示権限を持ちます。

     ![カレンダーをアクセス管理で共有](assets/calendar-share-manage-permissions-350x241.png)

     >[!NOTE]
     >
     >[!DNL Workfront] 管理者とカレンダーの作成者は、これらのエンティティから権限を削除できます。

1. （オプション）ユーザーの役割に応じて、「**[!UICONTROL 詳細オプション]**」、「**[!UICONTROL 共有]**」の順にクリックして、ユーザーが他のユーザーとカレン&#x200B;ダーを共有できるようにできる場合があります。

   権限レベルについて詳しくは、[オブジェクトに対する共有権限の概要](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)を参照してください。

1. （オプション）カレンダーをすべての [!DNL Workfront] ユーザーが使用できるようにするには 、歯車アイコンをクリックし、ドロップダウンメニューで「**[!UICONTROL システム全体で表示]**」をクリックして、すべての [!DNL Workfront] ユーザーがオブジェクトを利用できるようにします。\
   すべてのユーザーは、設定した権限に基づいてオブジェクトを表示できます。

1. 「**[!UICONTROL 保存]**」をクリックします。

## パブリックリンクとのカレンダーの共有

カレンダーを公開し、[!DNL Workfront] ライセンスを持たないユーザーとリンクを共有できます。

1. 共有するカレンダーに移動します。
1. 「**[!UICONTROL カレンダーのアクション]**」をクリックして、「**[!UICONTROL 共有]**」をクリックします。

1. 歯車アイコンをクリックし、「**[!UICONTROL これを外部ユーザーに公開する]**」をクリックします。
1. 「**[!UICONTROL リンクをコピー]**」をクリックします。
1. 「**[!UICONTROL 保存]**」をクリックします。

## カレンダーをプライベートリンクと共有する

[!DNL Workfront] ユーザーとプライベートカレンダーリンクを共有できます 。リンクを使用する際にカレンダーを表示するには、ログインする必要があります。

1. 共有するカレンダーに移動します。
1. 「**[!UICONTROL カレンダーのアクション]**」をクリックして、「**[!UICONTROL 共有可能なリンクを取得]**」をクリックします。

1. 「**[!UICONTROL リンクをコピー]**」をクリックします。

   >[!NOTE]
   >
   >[!DNL Workfront] ユーザーがリンクを使用してカレンダーにアクセスするには、カレンダーへのアクセス権を持っている必要があります。アクセス権を付与するには、[ [!DNL Workfront]  ユーザーとのカレンダーの共有](#share-a-calendar-with-workfront-users)を参照してください。\
   >ユーザーがアクセス権を持っていない場合、リンクをブラウザーに貼り付けた後にリクエストできます。
