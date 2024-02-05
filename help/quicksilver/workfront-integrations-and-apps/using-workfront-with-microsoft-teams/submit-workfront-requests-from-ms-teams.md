---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: ' [!DNL Microsoft]  Teams から  [!DNL Adobe Workfront]  リクエストを送信'
description: チームの所有者が Microsoft Teams 用に Adobe Workfront をインストールしたら、お使いの Microsoft Teams アカウントから Workfront のリクエストを送信できます。そのためには、リクエストを送信するためのアクセス権を持つ Workfront アカウントが必要です。Microsoft Teams 用 Workfront のインストールについて詳しくは、Microsoft Teams 用 Workfront のインストールを参照してください。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 5975d773-eae6-44ae-8296-2013504da3a8
source-git-commit: 1f2655c0e88a5cc918501e2a0ef830758111ded8
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 96%

---

# [!DNL Microsoft] Teams から [!DNL Adobe Workfront] リクエストを送信

>[!NOTE]
>
>Adobe WorkfrontとMicrosoft Teamsの統合は、現在、クラシックMicrosoft Teamsエクスペリエンスでのみサポートされています。

チームの所有者が [!DNL Adobe Workfront for Microsoft Teams] をインストールした後、[!DNL Microsoft Teams] アカウントから [!DNL Workfront] リクエストを送信することができます。そのためには、リクエストを送信するためのアクセス権を持つ Workfront アカウントが必要です。[!DNL Workfront for Microsoft Teams] のインストールについて詳しくは、[ [!DNL Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md) のインストールを参照してください。

>[!NOTE]
>
>[!DNL Microsoft Teams] は、[!DNL Internet Explorer] のサポートを終了しました。[!DNL Adobe Workfront for Microsoft Teams integration] を使用する場合は、[!DNL Internet Explorer] 以外の web ブラウザーを使用する必要があります。


## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>作業、プラン、レビュー、リクエスト</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## 前提条件

お使いの [!DNL Microsoft Teams] チーム所有者が、[!DNL Microsoft Teams] 用 [!DNL Workfront] をご自身の使用の前にインストールする必要があります。

## [!DNL Microsoft Teams] から [!DNL Workfront] リクエストの送信

1. [!DNL Microsoft Teams] の左側のナビゲーションバーにある&#x200B;**[!UICONTROL その他の追加アプリ]**（3 つのドット）のアイコンをクリックします。

1. 表示されるリストで **[!DNL Workfront]** をクリックします。
1. 「**[!UICONTROL リクエスト]**」タブをクリックします。
1. 「**[!UICONTROL 新規リクエスト]**」をクリックします。
1. **[!UICONTROL リクエストタイプを選択]**&#x200B;ボックスで、リクエストを送信するリクエストキューを選択します。
1. （オプション）リクエストキューで使用可能な場合は、トピックグループまたはキューのトピックを選択します。
1. 次の情報を指定します。

   （リクエストキューの設定方法に応じて、オプションとボックスは異なる場合があります。使用可能なフィールドの完全なリストと説明については、[ [!DNL Adobe Workfront]  リクエストを作成して送信](../../manage-work/requests/create-requests/create-submit-requests.md)を参照してください）

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">件名</td> 
      <td>リクエストの件名を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">説明</td> 
      <td>リクエストの説明を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> <p>リクエストに含めるドキュメントを添付します。ドラッグ＆ドロップを使用してドキュメントを添付するか、「[!UICONTROL Select file]」をクリックし、ファイルシステム内のドキュメントを参照して選択することができます。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション）[!DNL Workfront] 管理者がリクエストキューにカスタムフォームを添付していた場合、カスタムフォームで使用可能なフィールドに情報を入力します。
1. 新しいリクエストの下部にカスタムフォームが表示されます。
1. 「**[!UICONTROL 送信]**」をクリックします。

   リクエストが、指定したリクエストキュー内の [!DNL Workfront] に表示されます。リクエストが正常に送信されたことを示す確認メッセージが送信されます。

## [!DNL Microsoft Teams] で送信した [!DNL Workfront] リクエストを表示

1. [!DNL Microsoft Teams] の左側のナビゲーションバーにある&#x200B;**[!UICONTROL その他の追加アプリ]**（3 つのドット）のアイコンをクリックします。

1. 表示されるリストで **[!DNL Workfront]** をクリックします。
1. 「**[!UICONTROL リクエスト]**」タブをクリックします。

   送信したリクエストは、「[!UICONTROL リクエスト]」タブの[!UICONTROL 送信したリクエスト]エリアに一覧表示されます。このタブに表示される、送信したリクエストに関する情報は設定できません。

   送信されたリクエストに関する以下の情報を、「[!UICONTROL リクエスト]」タブの[!UICONTROL 送信したリクエスト]領域で表示することができます。

   * **[!UICONTROL 件名]**：リクエストの名前
   * **[!UICONTROL 参照番号]**
   * **[!UICONTROL リクエストタイプ]**：リクエストを送信したリクエストキューの名前
   * **[!UICONTROL ステータス]**
   * **[!UICONTROL 送信日]**：リクエストを送信した日付
   * **[!UICONTROL 割り当て先]**

1. （オプション）リスト内の任意の列のヘッダーをクリックして、その列でリストを並べ替えます。[!DNL Workfront] のデフォルトでは、最も新しく送信されたリクエストから順に、[!UICONTROL 送信]日でリストを並び替えます。
