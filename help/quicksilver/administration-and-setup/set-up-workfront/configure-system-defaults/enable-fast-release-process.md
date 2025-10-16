---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 組織の迅速リリースを有効または無効にする
description: 新しい Workfront 機能を毎月受け取るか、四半期ごとに受け取るかを選択できます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 71ef7a50-7a9f-43c4-b67c-8d9fc722569f
source-git-commit: 7ca27795ec115a112acb55113bfade4a5fee15ad
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 94%

---

# 組織の高速リリースを有効化または無効化

Adobe Workfront には、新機能と更新をリリースするためのモデルが 2 つあります。新機能を四半期ごとに受け取るか、より早いリリーススケジュールで受け取るかを選択できます。

どちらのモデルでも、同じ機能と更新が提供されます。タイミングが異なるだけです。

例：

* X 社が迅速リリースプロセスを有効にしました。8月に機能 A、9月に機能 B、10月に機能 C がそれぞれ提供されます。
* Y 社が迅速リリースプロセスを無効にしました。10月の四半期リリースで機能 A、B および C が提供されます。

>[!NOTE]
>
>* 23.3 リリース（2023年7月）以降に Workfront を購入したお客様の場合は、迅速リリースプロセスがデフォルトで有効になっており、オプトアウトできます。
>* 23.3 リリースより前に Workfront を購入したお客様の場合は、迅速リリースプロセスがデフォルトで無効になっており、オプトインできます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>標準</p> <p>プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>Workfront 管理者である必要があります。 </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 迅速リリースプロセスを有効または無効にする際の考慮事項

迅速リリースプロセスを有効または無効にする際は、次の点を考慮してください。

* 四半期半ばに迅速リリースプロセスを&#x200B;**有効に**&#x200B;すると、組織は、既に迅速リリースされている特長や機能にアクセスできるようになります。

  例えば、機能 A が 8月にリリースされ、機能 B が 9月にリリースされた場合、9月に迅速リリースプロセスを有効にした組織は直ちに機能 A および B にアクセスできます。

* 迅速リリースプロセスを&#x200B;**無効に**&#x200B;しても、次の四半期リリースまでは効力を生じません。

  例えば、迅速リリースを有効にした組織が 8月に無効にした場合でも、次の四半期リリースが 10月に発生するまでは四半期リリースに移行しないので、迅速リリースされる機能は 9月も引き続き提供されます。

## 組織の迅速リリースプロセスを有効化または無効化

迅速リリースプロセスを有効または無効にするには、次の手順に従います。

{{step-1-to-setup}}

1. 左側のナビゲーションで「**システム**」を展開し、「**環境設定**」をクリックします。
1. 迅速リリースを有効にするには、「**迅速リリースプロセスを有効にする**」チェックボックスをオンにします。

   または

   迅速リリースを無効にして四半期ごとのリリースサイクルに移るには、「**迅速リリースプロセスを有効にする**」チェックボックスをオフにします。

1. ポップアップウィンドウで選択内容を確認します。
1. 「**保存**」をクリックします。
