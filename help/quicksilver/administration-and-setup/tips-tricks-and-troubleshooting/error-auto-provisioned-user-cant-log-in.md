---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 「エラー：自動プロビジョニングされたユーザーがログインできません」
description: 自動プロビジョニングされたユーザーが初めてログインしようとし、システムがアクセスレベルを割り当てていないというエラーが表示された場合は、リクエストライセンスに関連付けられたアクセスレベルがシステムにない可能性があります。自動プロビジョニングではリクエストライセンスタイプを使用するので、リクエストライセンスに関連付けられたアクセスレベルを作成することで、この問題を修正できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4c88933e-d3da-447e-ab6c-be9261a94a19
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: ht
source-wordcount: '260'
ht-degree: 100%

---

# エラー：自動プロビジョニングされたユーザーがログインできません

自動プロビジョニングされたユーザーが初めてログインしようとすると、次のエラーが表示されます。

## 問題

システムが新規ユーザーにアクセスレベルを割り当てていません。

デフォルトでは、自動プロビジョニングはリクエストライセンスタイプを使用します。リクエストライセンスを持つアクセスレベルが存在しない場合、システムはユーザーにアクセスレベルを割り当てることができません。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>ユーザーは [!DNL Workfront] 管理者である必要があります。詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーへの完全な管理アクセス権の付与</a>を参照してください。</p> <p><b>メモ</b>：それでもアクセスできない場合は、アクセスレベルに追加の制限が設定されていないかどうかを [!DNL Workfront] 管理者にお問い合わせください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## ソリューション

リクエストライセンスを持つ基本的なアクセスレベルを作成します。

1. **[!UICONTROL 設定]**／**[!UICONTROL アクセスレベル]**&#x200B;に移動します。

1. 「**[!UICONTROL 新規アクセス レベル]**」をクリックします。
1. 「**[!UICONTROL 名前]**」を入力します。
1. **[!UICONTROL ライセンスタイプ]**&#x200B;ドロップダウンメニューから、「リクエスト」を選択します。
1. 「**[!UICONTROL 変更を保存]**」をクリックします。

リクエストライセンスを持つアクセスレベルを作成したら、ユーザーに SSO 資格情報を使用してログインしてもらいます。
