---
title: AI アシスタントを有効または無効にする
content-type: reference
description: AI アシスタントにアクセスできる、組織内のアクセスレベルを制御できます。
author: Becky
feature: Get Started with Workfront
exl-id: eec9f484-e29b-4256-b9ef-b45eb2e78eac
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 16%

---

# AI アシスタントを有効または無効にする

Workfront管理者は、組織内で AI アシスタントを有効にしているユーザーを制御できます。 これはアクセスレベルで管理します。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>標準</p>
   <p>プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront管理者である必要があります</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## Workfrontでの AI アシスタントの有効化または無効化

特定のアクセスレベルに対して AI アシスタントを有効にするには：

{{step-1-to-setup}}

1. 左側のナビゲーションで **アクセスレベル** を選択します。
1. 目的のアクセスレベルを選択し、リストの上にある **編集**![ 編集アイコン ](assets/edit-icon.png) アイコンをクリックします。
1. **アクセスレベルを編集** ボックスの「**追加の制限を設定…**」領域で、「**Workfront AI アシスタントを無効にする**」チェックボックスをオフにします。
1. 「**保存**」をクリックします。
1. AI アシスタントを有効にするアクセスレベルごとに、手順 3 ～ 5 を繰り返します。



>[!NOTE]
>
>* 管理者以外のユーザーは、AI アシスタントはデフォルトで無効になっています。
>* 管理者以外のユーザーがWorkfrontの「AI アシスタント」アイコンを操作すると、AI アシスタント契約書が表示され、管理者以外のユーザーに契約条件の同意を求められます。 契約書に同意すると、レイアウトテンプレートで無効になっている AI アシスタントを使用できます。

