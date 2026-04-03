---
title: AI アシスタントの有効化と無効化
content-type: reference
description: 組織内のどのアクセスレベルにAI アシスタントにアクセスできるかを制御できます。
author: Becky
feature: Get Started with Workfront
exl-id: eec9f484-e29b-4256-b9ef-b45eb2e78eac
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 14%

---

# AI アシスタントの有効化と無効化

Workfront管理者は、組織内のどのユーザーがAI アシスタントを有効にするかを制御できます。 これはアクセスレベルで管理されます。

アクセス レベルでAI アシスタントを有効にする前に、組織に対してAI アシスタントを有効にする必要があります。

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
   <td> <p>あなたはWorkfrontの管理者でなければなりません</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 組織のAI アシスタントを有効または無効にする

組織でAI アシスタントを有効にするには：

{{step-1-to-setup}}

1. 左側のナビゲーションで「**システム**」を選択し、「**環境設定**」を選択します。
1. **AIの環境設定** セクションまでスクロールします。
1. 「**AIを有効にする**」切替スイッチをオンにします。

>[!IMPORTANT]
>
>AI アシスタントを使用するには、Adobeで署名済みの生成AI契約書をファイルに含める必要があります。
>生成AI契約書について詳しくは、「[Adobe生成AI契約書に署名する](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)」を参照してください。詳しくは、WorkfrontのAI アシスタントの記事を参照してください。

## アクセスレベルのAI アシスタントを有効または無効にする

特定のアクセスレベルでAI アシスタントを有効にするには：

{{step-1-to-setup}}

1. 左側のナビゲーションで「**アクセスレベル**」を選択します。
1. 目的のアクセスレベルを選択し、リストの上にある&#x200B;**編集** ![編集アイコン &#x200B;](assets/edit-icon.png) アイコンをクリックします。
1. 「**アクセスレベルを編集**」ボックスの「**追加の制限を設定…**」領域で、「**Workfront AI アシスタントを無効にする**」チェックボックスのチェックを外します。
1. 「**保存**」をクリックします。
1. AI アシスタントを有効にするアクセスレベルごとに、手順3～5を繰り返します。



>[!NOTE]
>
>* 管理者以外のユーザーの場合、AI アシスタントはデフォルトで無効になっています。
>* 管理者以外のユーザーがWorkfrontのAI アシスタントアイコンとやり取りする場合、AI アシスタント契約書が表示され、管理者以外のユーザーに利用条件への同意を求めます。 契約書に同意すると、レイアウトテンプレートでAI アシスタントが無効になっていても、AI アシスタントを使用できます。

