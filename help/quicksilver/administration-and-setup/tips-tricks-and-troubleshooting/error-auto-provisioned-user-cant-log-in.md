---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: エラー：自動プロビジョニングされたユーザーはログインできません
description: 自動プロビジョニングされたユーザーが初めてログインしようとすると、システムによってアクセスレベルが割り当てられていないというエラーが表示される場合は、リクエストのライセンスに関連付けられたアクセスレベルがシステムにない可能性があります。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4c88933e-d3da-447e-ab6c-be9261a94a19
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 68%

---

# エラー：自動プロビジョニングされたユーザーがログインできません

自動プロビジョニングされたユーザーが初めてログインしようとすると、次のエラーが表示されます。

`Expect one user but found 0. ${subdomain} ${lane} ${email}`

## 問題

システムが新規ユーザーにアクセスレベルを割り当てていません。

デフォルトでは、自動プロビジョニングはリクエストライセンスタイプを使用します。リクエストライセンスを持つアクセスレベルが存在しない場合、システムはユーザーにアクセスレベルを割り当てることができません。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>標準</p>
       <p>プラン</p></td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ソリューション

リクエストライセンスを持つ基本的なアクセスレベルを作成します。

1. **[!UICONTROL 設定]**／**[!UICONTROL アクセスレベル]**&#x200B;に移動します。

1. 「**[!UICONTROL 新規アクセス レベル]**」をクリックします。
1. 「**[!UICONTROL 名前]**」を入力します。
1. **[!UICONTROL ライセンスタイプ]**&#x200B;ドロップダウンメニューから、「リクエスト」を選択します。
1. 「**[!UICONTROL 変更を保存]**」をクリックします。

リクエストライセンスを持つアクセスレベルを作成したら、ユーザーに SSO 資格情報を使用してログインしてもらいます。


