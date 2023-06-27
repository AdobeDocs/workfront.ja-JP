---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Adobe Workfront Fusion の組織とチーム
description: Adobe Workfront Fusion の組織とチームの機能により、企業は Fusion 内のシナリオや他の機能へのアクセスを制御できます。
author: Becky
feature: Workfront Fusion
exl-id: 601e937f-0286-4557-9a87-59aa9c0c22f1
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '1119'
ht-degree: 1%

---

# [!DNL Adobe Workfront Fusion] 組織とチーム

[!DNL Adobe Workfront Fusion]の組織およびチーム機能により、企業は Fusion 内のシナリオや他の機能へのアクセスを制御できます。

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計画*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：いいえ [!DNL Workfront Fusion] ライセンス要件。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] [!UICONTROL] の [!UICONTROL] [!DNL Workfront Fusion] 自動化 (WA)</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] がある場合 [!DNL Adobe Workfront] プラン（組織で購入する必要がある） [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。 [!DNL Workfront Fusion] は、[!UICONTROL Ultimate] に含まれています [!DNL Workfront] プラン</p>
   <p>または</p>
   <p>従来の製品要件：組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> 
     <p>次の条件を満たす必要があります。 [!DNL Workfront Fusion] 組織の管理者。</p>
     <p>次の条件を満たす必要があります。 [!DNL Workfront Fusion] チームの管理者。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

<p>** [!DNL Adobe Workfront Fusion] ライセンス， 「 <a href="../../workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] ライセンス</a></p>


## 組織

[!DNL Workfront Fusion] ユーザーが組織に属している。

* [組織の役割](#organization-roles)
* [組織へのユーザーの招待](#inviting-users-to-an-organization)
* [組織間の切り替え](#switch-between-organizations)

### 組織の役割

組織内のユーザーの役割は次のいずれかです。

* **[!UICONTROL 所有者]**:所有者には、組織で使用できるすべての権限があります。
* **[!UICONTROL 管理者]**:管理者の役割を使用すると、ユーザーは組織のチームやユーザーを作成および管理できます。
* **[!UICONTROL メンバー]**:メンバーは [!DNL Workfront Fusion] ただし、組織の変更を行うことはできません。
* **[!UICONTROL 会計士]**:会計士の役割を持つユーザーは、組織のダッシュボードでライセンス情報を表示することのみ可能です。
* **[!UICONTROL アプリ開発者]**:この役割の機能は現在ご利用いただけません。近い将来にご利用いただける予定です。 現時点では、この役割にユーザーを割り当てることはお勧めしません。

### 組織へのユーザーの招待

デフォルトでは、組織の所有者（または承認済みユーザー）は、別のユーザーを組織に招待できます。

ユーザーを組織に招待するには：

1. クリック **[!UICONTROL 詳細を変更]** をクリックします。
1. 選択 **[!UICONTROL 新しいユーザーの招待]**.

   ![](assets/fusion-organization-invite-user-350x199.png)

1. ユーザーの電子メールアドレスと名前を入力します。
1. ユーザーの役割を選択します。 役割について詳しくは、 [組織の役割](#organization-roles) 」を参照してください。
1. （オプション）メモを追加します。 このメモは、ユーザーが受け取る招待メールに表示されます。
1. 「**[!UICONTROL 保存]**」をクリックします。

[!DNL Fusion] 特定の組織に招待メールを送信し、 [!UICONTROL 役割を承認] 」ボタンをクリックします。

![](assets/accept-the-role.png)

受信者が「 」ボタンをクリックすると、招待ページにリダイレクトされ、招待を受け入れることができます。

招待は 1 日で失効します。

>[!NOTE]
>
>ユーザーが [!DNL Fusion], [!DNL Fusion] は自動的にアカウントを作成し、仮パスワードが記載された電子メールを送信し、新しいユーザーにログインしてパスワードを変更するよう指示します。

### 組織間の切り替え

Fusion では、複数の組織に属している場合があります。 リソースは組織間で共有されません。

右上隅の組織名をクリックし、ドロップダウンから新しい組織を選択することで、AdobeUnified Experience 内で組織を切り替えることができます。 Adobe内の他の組織のメンバーである場合でも、ドロップダウンには Fusion アカウントを持つ組織のみが表示されます。

## チーム

チームとは、特定のリソースへのアクセスを共有するユーザーのグループです。 以下のリソースが含まれます。

* シナリオ
* 接続
* Webhook
* キー
* データストア
* データ構造
* 電子メール通知設定

>[!NOTE]
>
>チームがリソースへのアクセスを制御するので、チームが 1 人のメンバーだけを持つと便利です。 例えば、トレーニングのユーザーは、個人への接続を作成できます [!DNL Google] アカウント。 チームメンバーは個人にも接続できます [!DNL Google] アカウントに組み込む必要があるので、この場合は、ユーザーをトレーニングチームの唯一のメンバーにすることが最善です。

組織には必要な数のチームが含まれ、ユーザーは 1 つ以上のチームに属する場合があります。

ユーザーは、左側のナビゲーションパネルにあるドロップダウンリストからチームを選択できます。 ユーザーには、自分が属するチームのみが表示されます。 チームを選択すると、ユーザーはそのチームのリソースにアクセスできます。

* [チームの役割](#team-roles)
* [チーム管理](#team-management)

### チームの役割

ユーザーは、各チームで次の役割のいずれかを持ちます。

* **[!UICONTROL チーム管理者]**:管理者ロールでは、他のチームロールの機能に加えて、チームメンバーのロールの追加、削除、変更を行うことができます。
* **[!UICONTROL チームメンバー]**:チームメンバーの役割を使用すると、シナリオを作成および実行できます。
* **[!UICONTROL チーム監視]**:この [!UICONTROL 監視] 役割を使用すると、シナリオの実行情報にアクセスできますが、シナリオを設計したり、「アクティブ」ステータスを変更したりすることはできません。
* **[!UICONTROL チームオペレーター]**:この [!UICONTROL 演算子] 役割を使用すると、ユーザーは実行データを表示し、シナリオの「アクティブ」ステータスを変更できます。
* **[!UICONTROL チーム制限メンバー]**:この役割の機能は現在ご利用いただけません。近い将来にご利用いただける予定です。 現時点では、この役割にユーザーを割り当てることはお勧めしません。

### チーム管理

* [チームの作成](#create-a-team)
* [チーム通知オプションの設定](#set-team-notification-options)

#### チームの作成

組織の所有者と管理者は、チームを作成できます。

チームを作成するには：

1. 左側のナビゲーションパネルで、 **[!UICONTROL 組織]**
1. を選択します。 **[!UICONTROL チーム]** タブをクリックします。
1. クリック **[!UICONTROL 新しいチームを追加]** をクリックします。
1. 新しいチームの名前を入力し、 **追加**.

#### チーム通知オプションの設定

電子メール通知オプションは、チームレベルで設定されます。

1. 左側のナビゲーションパネルで、 **[!UICONTROL チーム]**
1. を選択します。 **[!UICONTROL 通知オプション]** タブをクリックします。
1. チームが受信する通知を有効にします。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">'[!UICONTROL シナリオ実行時の警告 ]'</td> 
      <td> <p>シナリオの実行で警告が発生した場合に電子メールを受信</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL シナリオ実行時のエラー ]</td> 
      <td>シナリオ実行でエラーが発生した場合に電子メールを受け取ります。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL シナリオの非アクティブ化 ]</p> </td> 
      <td><p>シナリオが非アクティブ化されると、電子メールを受信します。</p><p><b>注意：</b> シナリオの非アクティブ化についての通知は、エラーが原因でシナリオが自動的に非アクティブ化された場合にのみ表示されます。 手動で非アクティブ化されたシナリオに関する通知は受け取りません。</p><p>場合によっては、 [!DNL Workfront Fusion] エンジニアリングチームに問題が発生しています。 この場合、 [!DNL Workfront Fusion]. </p></td>

</tr>
</tbody>
</table>

通知オプションの変更は自動的に保存されます

#### チーム間の切り替え

Fusion では、複数のチームに属している可能性があります。 チームはリソースを共有しないので、特定のシナリオや他のリソースにアクセスするためにチームを切り替える必要が生じる場合があります。

組織がAdobeUnified Experience に登録されていない場合は、左側のナビゲーションでチーム名をクリックし、ドロップダウンからチームを選択して、チームを切り替えることができます。

チームがAdobeUnified Experience を使用している場合は、ヘッダーのチーム名をクリックし、ドロップダウンからチームを選択して、新しいチームを選択できます。 このオプションは、シナリオページや接続ページなど、特定のチームに固有のすべてのページから使用できます。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/organization-add-team-350x181.png" style="width: 350;height: 181;"> </p>
-->