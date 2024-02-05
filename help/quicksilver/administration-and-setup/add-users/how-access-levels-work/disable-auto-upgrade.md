---
title: 新しいライセンスプランの有料ユーザーに対して自動アップグレードオプションを無効にする
user-type: administrator
content-type: reference
product-area: system-administration
keywords: アクセス、レベル、システム、管理者、標準、ライト、コントリビューター
navigation-topic: access-levels
description: Workfront にログインして作業するためのアクセスレベルがすべてのユーザーに必要です。アクセスレベルを使用して、Workfront の特定のオブジェクトや領域でユーザーが表示したり実行したりする項目を制御できます。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 58c76187-fc74-4ab4-80e8-c3e296a84f27
source-git-commit: 7467e75cf468fa6a1dd14dbc0f4fdcda87de1b1e
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 97%

---

# 新しいライセンスプランの有料ユーザーに対して自動アップグレードオプションを無効にする

プルーフおよびドキュメントの決定は、新しいプランでは 無償 Workfront ライセンスすべてに対して制限されます。ユーザーが割り当てられた決定数に達すると、デフォルトでライトライセンスにアップグレードされます。

設定エリアで「自動アップグレード」オプションを無効にできます。自動アップグレードの動作について詳しくは、[無償ユーザーに対する限定的なドキュメントおよびプルーフの決定の概要](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md)を参照してください。

>[!IMPORTANT]
>
>無効にすると、割り当てられた決定数を超えた無償ユーザーが自動的にアップグレードされなくなります。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td>新規プラン：標準
   <p>または</p>
   <p>現在のプラン：プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p></td> 
  </tr> 
 </tbody> 
</table>

## 無償ユーザーの自動アップグレードを無効にする

{{step-1-to-setup}}

1. 左側のナビゲーションで「[!UICONTROL **システム**]」を展開し、「[!UICONTROL **環境設定**]」をクリックします。
1. 「[!UICONTROL **一般環境設定**]」セクションで、「[!UICONTROL **アクセスレベル内で自動アップグレードを無効化**]」ボックスにチェックを入れます。
1. 「[!UICONTROL **保存**]」をクリックします。
