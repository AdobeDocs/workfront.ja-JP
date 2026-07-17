---
title: スタンドアロン製品としてのAdobe Workfront Planningでのユーザーの管理
description: ここでは、Planningをスタンドアロン製品として購入した場合に、Adobe Workfront Planningでユーザーおよびチームを管理する方法について説明します。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 697499fadf4d5d22292ededed381cb72e53fcae3
workflow-type: tm+mt
source-wordcount: '835'
ht-degree: 1%

---


# Adobe Workfront Planningのユーザーをスタンドアロン製品として管理する

>[!IMPORTANT]
>
>ここでは、スタンドアロン製品として購入した場合のAdobe Workfront計画について説明します。 Workfront Workflow パッケージを購入しておらず、Adobe Workfront Planningのみのパッケージを購入した場合は、この記事を参照してください。
>
>Workfront パッケージと一緒に購入した場合のAdobe Workfront計画について詳しくは、[Adobe Workfront計画の基本を学ぶ](/help/quicksilver/planning/general/planning-overview.md)を参照してください。
>

Adobe Workfront Planningでは、Adobe Workfrontと同様に、ユーザーをスタンドアロン製品として管理できます。

Workfront Planningでユーザーを割り当てることができるアクセスレベルには、いくつかの制限があります。

## アクセス要件

+++ 展開して、この記事の機能のアクセス要件を表示します。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront計画パッケージ</p></td> 
   <td> 
<p>任意のWorkfront計画をスタンドアロンパッケージとして</p>

</td> </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>計画管理者</p>
   </td> 
  </tr>

</tbody> 
</table>

Workfront as a スタンドアロンパッケージに必要なアクセスについて詳しくは、[&#x200B; スタンドアロン製品としてのAdobe Workfront Planningに必要なアクセス &#x200B;](/help/quicksilver/planning/planning-sta/access-needed-for-planning-sta.md)を参照してください。
+++    

## Adobe Workfront Planningのアクセスレベル

スタンドアロン製品として購入した場合、Workfront Planningのユーザーに次のアクセスレベルを割り当てることができます。

* 計画管理者
* 計画標準

各アクセスに含まれる機能について詳しくは、「[&#x200B; スタンドアロン製品としてのAdobe Workfront Planningに必要なアクセス &#x200B;](/help/quicksilver/planning/planning-sta/access-needed-for-planning-sta.md)」を参照してください。

Workfront Planningをスタンドアロン製品として使用する場合は、次の点を考慮してください。

* Workfront Planningでは、アクセスレベルを作成または変更することはできません。 それらは事前設定されています。

* Workfront製品の管理者としてAdobe Admin Consoleにユーザーを追加すると、ユーザーはWorkfront Planningでこのアクセスレベルに自動的に割り当てられ、そのアクセスレベルはPlanningで編集できません。
* Planning Standardのアクセスレベルは、ユーザーをAdmin Consoleに追加した後にのみ、Planningのユーザーに割り当てることができます。 これは、ユーザーに手動で割り当てることができる唯一のアクセスレベルです。

## Workfront Planningのユーザーをスタンドアロン製品として管理する

1. 計画管理者は、次のいずれかの操作を行います。

   * Workfront Planningの新規のお客様の場合は、Adobe Workfrontからメールが届き、Adobe Workfrontにアカウントが追加されたことを知らせる通知が届きます。 メール内のリンクを使用して、Admin Consoleにログインします。

   * 既存のWorkfront計画管理者で、アカウントに他のユーザーを追加する場合は、Admin Consoleにログインします。

   詳しくは、[Adobe Admin Consoleでのユーザーの管理](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)を参照してください。

1. Admin Consoleで、次のいずれかのタブでユーザーの追加を開始します。

   * **管理者**: ユーザーは、PlanningのPlanning Administrator ユーザーとして自動的に作成されます。
   * **ユーザー**: Workfront Planningでアクセス レベルを割り当てる必要があります。

1. （条件付き）Adobe CX Enterprise ホームからWorkfrontにログインします。

   Workfront Planningが開きます。
1. **メインメニュー** > **ユーザー** > **新規ユーザー**&#x200B;をクリックします。

   ![&#x200B; スタンドアロン計画の新しいユーザーボックス &#x200B;](assets/new-user-box-planning-sta.png)

1. **新規ユーザー** ボックスで、次の情報を更新します。

   * **名**: Admin Consoleに追加した名前と同じです。
   * **姓**: Admin Consoleに追加した名前と同じです。
   * **電子メールアドレス（ユーザー名）**:Admin Consoleに追加した電子メールと同じ電子メール。
   * **ユーザーがアクティブです**：ユーザーがアクティブであり、Workfront Planningにログインでき、レコードに割り当てることができることを示すには、設定をオンにします。
   * **アクセスレベル**：管理者以外のユーザーのPlanning Standardを選択します。 それが唯一の選択肢です。

     >[!TIP]
     >
     >Admin Consoleで既にAdministratorとして設定されているユーザーを追加すると、Planning Administratorのアクセスレベルが自動的にユーザーに追加されます。 これは編集できません。

   * **チーム**: ドロップダウンメニューから、ユーザーに関連付けるチームを選択します。 チームをユーザーに割り当てる前に、チームを作成する必要があります。

     詳しくは、[&#x200B; チームの管理](/help/quicksilver/planning/planning-sta/manage-teams-in-planning-sta.md)を参照してください。

1. 「**今すぐアップロード**」をクリックしてプロファイル画像を追加し、「**保存**」をクリックします。

1. 「**保存**」または「**ユーザーを追加して別の**&#x200B;を開始」をクリックし、ユーザーを保存して別のユーザーを追加します。

   ユーザーが追加され、Workfront Planningにログインするための電子メールが送信されます。
1. （オプション）既存のユーザーを編集するには、次のいずれかの操作を行います。

   * リスト内のユーザー名にカーソルを合わせ、**詳細** メニュー![詳細メニュー](assets/more-menu.png) > **ユーザーの編集**&#x200B;をクリックします
   * リストでユーザーを選択し、ページ下部の青いツールバーの「**ユーザーを編集**」をクリックします。
1. （オプション）ユーザーを削除するには、次のいずれかの操作を行います。

   * リスト内のユーザー名にカーソルを合わせ、**詳細** メニュー![詳細メニュー](assets/more-menu.png) > **ユーザーの削除**&#x200B;をクリックします
   * リストでチームを選択し、ページ下部の青いツールバーの&#x200B;**ユーザーの削除**&#x200B;をクリックします
1. 「**削除**」をクリックして確認します。
1. （オプション）ユーザーを非アクティブ化するには、次のいずれかの操作を行います。

   * リスト内のユーザー名にカーソルを合わせ、**詳細** メニュー![詳細メニュー](assets/more-menu.png) > **非アクティブ化**&#x200B;をクリックします
   * リストでチームを選択し、ページ下部の青いツールバーの&#x200B;**無効化**&#x200B;をクリックします
1. 「**非アクティブ化**」をクリックして確認します。

   作業履歴を保存するには、ユーザーを削除するのではなく、非アクティブにすることをお勧めします。

