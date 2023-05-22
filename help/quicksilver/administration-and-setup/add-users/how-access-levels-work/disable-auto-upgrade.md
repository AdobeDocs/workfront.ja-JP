---
title: 新しいライセンスプランの有料ユーザーに対して自動アップグレードオプションを無効にする
user-type: administrator
content-type: reference
product-area: system-administration
keywords: アクセス，レベル，システム，管理者，標準，ライト，寄稿者
navigation-topic: access-levels
description: Workfrontにログインして作業するには、すべてのユーザーにアクセスレベルが必要です。 アクセスレベルを使用して、特定のWorkfrontオブジェクトや領域でユーザーが表示したり実行したりする操作を制御できます。
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 864906732c80af12db051d1d5e6d9bc4ae125eb8
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 1%

---


# 新しいライセンスプランの有料ユーザーに対して自動アップグレードオプションを無効にする

配達確認とドキュメントの決定は、新しいプランに対する有料Workfrontライセンスすべてに対して制限されます。 ユーザーが決定された数に達すると、デフォルトで Light ライセンスにアップグレードされます。

セットアップ領域で自動アップグレードオプションを無効にできます。 自動アップグレードの動作の詳細については、 [非有料ユーザーに対する限定的なドキュメントおよび配達確認の決定の概要](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md).

>[!IMPORTANT]
>
>無効にした場合、決定の数を超えた有料以外のユーザーは、自動的にアップグレードされません。


## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td>現在のプラン：標準
   <p>または</p>
   <p>レガシープラン：プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront管理者である。</p></td> 
  </tr> 
 </tbody> 
</table>

## 有料以外のユーザーの自動アップグレードを無効にする

{{step-1-to-setup}}

1. 下にスクロールして [!UICONTROL **環境設定**].
1. 内 [!UICONTROL **一般環境設定**] セクションで、 [!UICONTROL **アクセスレベル内で自動アップグレードを無効にする**] ボックス
1. 「[!UICONTROL **保存**]」をクリックします。
