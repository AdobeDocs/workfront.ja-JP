---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Adobe Workfront Fusion の組織とチーム
description: Adobe Workfront Fusion の組織とチームの機能を使用すると、企業は Fusion 内のシナリオや他の機能へのアクセスを制御できます。
author: Becky
feature: Workfront Fusion
exl-id: 601e937f-0286-4557-9a87-59aa9c0c22f1
source-git-commit: a51dfcfc3024fd7d1d2612d6f258379d4d166c49
workflow-type: tm+mt
source-wordcount: '1175'
ht-degree: 95%

---

# [!DNL Adobe Workfront Fusion] の組織とチーム

[!DNL Adobe Workfront Fusion] の組織とチーム機能を使用すると、企業は Fusion 内のシナリオや他の機能へのアクセスを制御できます。

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件は不要。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]、[!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。[!DNL Workfront Fusion] は、[!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> 
     <p>組織の [!DNL Workfront Fusion] 管理者である必要があります。</p>
     <p>チームの [!DNL Workfront Fusion] 管理者である必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

<p>**[!DNL Adobe Workfront Fusion] ライセンスについては、<a href="../../workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] ライセンス</a>を参照してください。</p>


## 組織

[!DNL Workfront Fusion] ユーザーは組織に属しています。

* [組織の役割](#organization-roles)
* [組織へのユーザーの招待](#inviting-users-to-an-organization)
* [組織間の切り替え](#switch-between-organizations)

### 組織の役割

ユーザーには、組織内で次のいずれかの役割があります。

* **[!UICONTROL 所有者]**：所有者は、組織で使用可能なすべての権限を持っています。
* **[!UICONTROL 管理者]**：管理者の役割のユーザーは、組織のチームやユーザーを作成および管理できます。
* **[!UICONTROL メンバー]**：メンバーは [!DNL Workfront Fusion] を使用できますが、組織を変更することはできません。
* **[!UICONTROL 経理担当]**：経理担当の役割のユーザーは、組織のダッシュボードでライセンス情報を表示することのみ可能です。
* **[!UICONTROL アプリ開発者]**：この役割の機能は現在使用できません。近い将来に使用可能になる予定です。現時点では、この役割にユーザーを割り当てることはお勧めしません。

各組織の役割を持つユーザーが使用できる特定のアクションについて詳しくは、 [組織とチームの役割](/help/quicksilver/workfront-fusion/organizations/organization-roles.md).

### 組織へのユーザーの招待

デフォルトでは、組織の所有者（または認可されたユーザー）は、別のユーザーを組織に招待できます。

ユーザーを組織に招待するには：

1. 画面の右上隅にある「**[!UICONTROL 詳細を変更]**」をクリックします。
1. 「**[!UICONTROL 新しいユーザーの招待]**」を選択します。

   ![](assets/fusion-organization-invite-user-350x199.png)

1. ユーザーのメールアドレスと名前を入力します。
1. ユーザーの役割を選択します。役割について詳しくは、このドキュメントの[組織の役割](#organization-roles)を参照してください。
1. （オプション）メモを追加します。このメモは、ユーザーが受け取る招待メールに表示されます。
1. 「**[!UICONTROL 保存]**」をクリックします。

[!DNL Fusion] は、特定の組織への招待と「[!UICONTROL 役割を承諾]」ボタンを含んだメールを送信します。

受信者がボタンをクリックすると、招待ページにリダイレクトされ、招待を受け入れることができます。

招待は 1 日で期限が切れます。

>[!NOTE]
>
>ユーザーが [!DNL Fusion] を初めて使用する場合、[!DNL Fusion] はそのユーザーのアカウントを自動的に作成し、仮パスワードが記載されたメールを送信し、新しいユーザーに対して、ログインしてパスワードを変更するように指示します。

### 組織間の切り替え

Fusion では、複数の組織に属している場合があります。リソースは組織間で共有されません。

右上隅の組織名をクリックし、ドロップダウンから新しい組織を選択することで、Adobe Unified Experience 内で組織を切り替えることができます。アドビ内の他の組織のメンバーである場合でも、ドロップダウンには Fusion アカウントを持つ組織のみが表示されます。

## チーム

チームとは、特定のリソースへのアクセスを共有するユーザーのグループです。これらのリソースには以下が含まれます。

* シナリオ
* 接続
* Web フック
* キー
* データストア
* データ構造
* メール通知設定

>[!NOTE]
>
>チームがリソースへのアクセスを制御するので、メンバーが 1 人だけのチームがあると便利な場合があります。例えば、トレーニングのユーザーは、個人の [!DNL Google] アカウントへの接続を作成できます。チームメンバーは個人の [!DNL Google] アカウントに接続することもできるので、この場合は、ユーザーがトレーニングチームの唯一のメンバーになることが最善です。

組織には必要な数のチームが含まれ、ユーザーは 1 つ以上のチームに属する場合があります。

ユーザーは、左側のナビゲーションパネルにあるドロップダウンリストからチームを選択できます。ユーザー自身が属するチームのみが表示されます。チームを選択すると、ユーザーはそのチームのリソースにアクセスできます。

* [チームの役割](#team-roles)
* [チーム管理](#team-management)

### チームの役割

ユーザーは、各チームで次の役割のいずれかを持ちます。

* **[!UICONTROL チーム管理者]**：管理者の役割として、他のチームの役割の機能に加え、チームメンバーの役割の追加、削除、変更をユーザーに許可します。
* **[!UICONTROL チームメンバー]**：チームメンバーの役割として、ユーザーはシナリオを作成および実行できます。
* **[!UICONTROL チームモニタリング]**：[!UICONTROL モニタリング]の役割を使用すると、ユーザーはシナリオの実行情報にアクセスできますが、シナリオを設計したり、「アクティブ」ステータスを変更したりすることはできません。
* **[!UICONTROL チームオペレーター]**：[!UICONTROL オペレーター]の役割を使用すると、ユーザーは実行データを表示し、シナリオの「アクティブ」ステータスを変更できます。
* **[!UICONTROL チーム制限メンバー]**：この役割の機能は現在使用できません。近い将来に使用可能になる予定です。現時点では、この役割にユーザーを割り当てることはお勧めしません。

各チームロールのユーザーが使用できる特定のアクションについて詳しくは、 [組織とチームの役割](/help/quicksilver/workfront-fusion/organizations/organization-roles.md).

### チーム管理

* [チームの作成](#create-a-team)
* [チーム通知オプションの設定](#set-team-notification-options)

#### チームの作成

組織の所有者と管理者は、チームを作成できます。

チームの作成方法

1. 左側のナビゲーションパネルで、「**[!UICONTROL 組織]**」をクリックします
1. 「**[!UICONTROL チーム]**」タブを選択します。
1. チームのリストの下にある「**[!UICONTROL 新しいチームを追加]**」をクリックします。
1. 新しいチームの名前を入力し、「**追加**」をクリックします。

#### チーム通知オプションの設定

>[!NOTE]
>
>次にアクセスする場合： [!DNL Fusion] から [!DNL Adobe Experience Cloud]の場合、通知は [!DNL Experience Cloud] 通知センター
>
>詳しくは、 [通知にアクセスする](/help/quicksilver/workfront-fusion/fusion-in-admin-console/fusion-unified-experience.md#access-your-notifications) in [[!DNL Adobe Unified Experience] 対象： [!DNL Workfront Fusion]](/help/quicksilver/workfront-fusion/fusion-in-admin-console/fusion-unified-experience.md)

メール通知オプションは、チームレベルで設定されます。

1. 左側のナビゲーションパネルで、「**[!UICONTROL チーム]**」をクリック
1. 「**[!UICONTROL 通知オプション]**」タブを選択します。
1. チームが受け取る通知を有効にします。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">「[!UICONTROL Warning in scenario run]」</td> 
      <td> <p>シナリオの実行で警告が発生した場合にメールを受信</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Errors in scenario run]</td> 
      <td>シナリオ実行でエラーが発生した場合に、メールを受け取ります。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Scenario deactivation]</p> </td> 
      <td><p>シナリオが非アクティブ化された場合、メールを受信します。</p><p><b>メモ：</b>エラーが原因でシナリオが自動的に非アクティブ化された場合にのみ、シナリオの非アクティブ化についての通知を受けます。手動で非アクティブ化されたシナリオに関する通知は受け取りません。</p><p>場合によっては、シナリオがパフォーマンスやその他の問題を引き起こしているため、[!DNL Workfront Fusion] エンジニアリングチームによってシナリオが非アクティブ化されることがあります。このような場合、[!DNL Workfront Fusion] では通知を受け取りません。 </p></td>

</tr>
</tbody>
</table>

通知オプションの変更は自動的に保存されます

#### チーム間の切り替え

Fusion では、複数のチームに属している場合があります。チームはリソースを共有しないので、特定のシナリオやその他のリソースにアクセスするには、チームを切り替える必要がある場合があります。

組織が AdobeUnified Experience を使用していない場合は、左側のナビゲーションでチーム名をクリックし、ドロップダウンからチームを選択して、チームを切り替えることができます。

チームが AdobeUnified Experience を使用している場合は、ヘッダーのチーム名をクリックし、ドロップダウンからチームを選択して、新しいチームを選択できます。このオプションは、シナリオページや接続ページなど、特定のチームに固有のすべてのページから使用できます。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/organization-add-team-350x181.png" style="width: 350;height: 181;"> </p>
-->