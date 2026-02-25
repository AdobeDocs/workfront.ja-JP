---
title: AI アシスタントの有効化と無効化
content-type: reference
description: AI アシスタントにアクセスできる、組織内のアクセスレベルを制御できます。
author: Becky
feature: Get Started with Workfront
exl-id: eec9f484-e29b-4256-b9ef-b45eb2e78eac
source-git-commit: e8e10f02f77f6c1df9f0af380eb16cc6bbc3b5d1
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 14%

---

# AI アシスタントの有効化と無効化

Workfront管理者は、組織内で AI アシスタントを有効にしているユーザーを制御できます。 これはアクセスレベルで管理します。

アクセスレベルに対して AI アシスタントを有効にするには、組織の AI アシスタントを有効にする必要があります。

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

## 組織の AI アシスタントを有効または無効にする

組織で AI アシスタントを有効にするには：

{{step-1-to-setup}}

1. 左側のナビゲーションで「**システム**」を選択し、「**環境設定**」を選択します。
1. 「**AI 環境設定**」セクションまでスクロールします。
1. **AI を有効にする** トグルをオンにします。

>[!IMPORTANT]
>
>AI アシスタントを使用するには、Adobeとファイルに署名済みの Gen AI 契約が必要です。
>Gen AI 契約について詳しくは、Workfrontの AI アシスタントの記事の [Adobe Gen AI 契約に署名する &#x200B;](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) を参照してください。

## アクセス レベルに対して AI アシスタントを有効または無効にする

特定のアクセスレベルに対して AI アシスタントを有効にするには：

{{step-1-to-setup}}

1. 左側のナビゲーションで **アクセスレベル** を選択します。
1. 目的のアクセスレベルを選択し、リストの上にある **編集**![&#x200B; 編集アイコン &#x200B;](assets/edit-icon.png) アイコンをクリックします。
1. **アクセスレベルを編集** ボックスの「**追加の制限を設定…**」領域で、「**Workfront AI アシスタントを無効にする**」チェックボックスをオフにします。
1. 「**保存**」をクリックします。
1. AI アシスタントを有効にするアクセスレベルごとに、手順 3 ～ 5 を繰り返します。



>[!NOTE]
>
>* 管理者以外のユーザーは、AI アシスタントはデフォルトで無効になっています。
>* 管理者以外のユーザーがWorkfrontの「AI アシスタント」アイコンを操作すると、AI アシスタント契約書が表示され、管理者以外のユーザーに契約条件の同意を求められます。 契約書に同意すると、レイアウトテンプレートで無効になっている AI アシスタントを使用できます。

