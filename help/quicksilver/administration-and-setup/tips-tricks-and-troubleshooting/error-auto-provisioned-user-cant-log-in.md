---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "エラー：自動プロビジョニングされたユーザーがログインできない"
description: 自動プロビジョニングされたユーザーが初めてログインしようとし、システムがアクセスレベルを割り当てていないというエラーが表示された場合は、システムに Request ライセンスに関連するアクセスレベルがない可能性があります。 自動プロビジョニングは要求ライセンスの種類を使用するので、要求ライセンスに関連付けられたアクセスレベルを作成することで、この問題を修正できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4c88933e-d3da-447e-ab6c-be9261a94a19
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 1%

---

# エラー：自動プロビジョニングされたユーザーがログインできない

自動プロビジョニングされたユーザーが初めてログインしようとすると、次のエラーが表示されます。

## 問題

新しいユーザーにアクセスレベルを割り当てていない。

デフォルトでは、自動プロビジョニングは「リクエスト」ライセンスタイプを使用します。 要求ライセンスを持つアクセスレベルが存在しない場合、システムはユーザーにアクセスレベルを割り当てることができません。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>次の条件を満たす必要があります。 [!DNL Workfront] 管理者。 詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> <p><b>注意</b>:まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者はアクセスレベルを変更できます。詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 解決策

リクエストライセンスを使用して基本的なアクセスレベルを作成します。

1. に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL アクセスレベル]**.

1. クリック **[!UICONTROL 新しいアクセスレベル]**.
1. を入力します。 **[!UICONTROL 名前]**.
1. 内 **[!UICONTROL ライセンスの種類]** ドロップダウンメニューから、「リクエスト」を選択します。
1. クリック **[!UICONTROL 変更を保存]**.

Request ライセンスでアクセスレベルを作成したら、ユーザーに SSO 認証情報を使用してログインしてもらいます。
