---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 「エラー：自動プロビジョニングされたユーザーはログインできません」
description: 自動プロビジョニングされたユーザーが初めてログインしようとすると、システムによってアクセスレベルが割り当てられていないというエラーが表示される場合は、リクエストのライセンスに関連付けられたアクセスレベルがシステムにない可能性があります。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4c88933e-d3da-447e-ab6c-be9261a94a19
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 72%

---

# エラー：自動プロビジョニングされたユーザーがログインできません

自動プロビジョニングされたユーザーが初めてログインしようとすると、次のエラーが表示されます。

`Expect one user but found 0. ${subdomain} ${lane} ${email}`

## 問題

システムが新規ユーザーにアクセスレベルを割り当てていません。

デフォルトでは、自動プロビジョニングはリクエストライセンスタイプを使用します。リクエストライセンスを持つアクセスレベルが存在しない場合、システムはユーザーにアクセスレベルを割り当てることができません。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td>
   <p>新規：標準</p>
   <p>または</p>
   <p>現在：プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td>  
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ソリューション

リクエストライセンスを持つ基本的なアクセスレベルを作成します。

1. **[!UICONTROL 設定]**／**[!UICONTROL アクセスレベル]**&#x200B;に移動します。

1. 「**[!UICONTROL 新規アクセス レベル]**」をクリックします。
1. 「**[!UICONTROL 名前]**」を入力します。
1. **[!UICONTROL ライセンスタイプ]**&#x200B;ドロップダウンメニューから、「リクエスト」を選択します。
1. 「**[!UICONTROL 変更を保存]**」をクリックします。

リクエストライセンスを持つアクセスレベルを作成したら、ユーザーに SSO 資格情報を使用してログインしてもらいます。


