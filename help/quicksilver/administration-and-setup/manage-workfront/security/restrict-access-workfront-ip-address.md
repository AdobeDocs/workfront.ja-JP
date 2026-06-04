---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Adobe WorkfrontへのアクセスをIP アドレスで制限する
description: Adobe Workfront IP 許可リストを設定して、Workfront へのアクセスを 75 個の IP アドレス、または指定した IP アドレスの範囲に制限することができます。 これにより、Workfront アプリケーションのセキュリティレイヤーがさらに強化されます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: aed65b42-d534-453a-885d-f922114987bc
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/lF3yMazoaB-W2h4ePgavnN96SZ98YYiJYuC927ImYcs
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 405
ht-degree: 98%

---

# IP アドレスで Adobe Workfront へのアクセスを制限

<!--
>[!IMPORTANT]
>
>This functionality is not currently available to organizations that have been onboarded to the Adobe Admin Console. It will be available in the Adobe Admin Console in a future release.
-->

Adobe Workfront IP 許可リストを設定して、Workfront へのアクセスを 75 個の IP アドレス、または指定した IP アドレスの範囲に制限することができます。 これにより、Workfront アプリケーションのセキュリティレイヤーがさらに強化されます。

これらの IP アドレスまたは IP アドレス範囲は、ネットワーク管理者によって提供される必要があります。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>標準</p><p>プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## その他の許可リスト

ファイアウォールやメールサーバーが、特定のベンダーへのアクセスのみを許可するように設定されている場合は、特定の IP アドレスをその許可リストに追加する必要があります。 これにより、環境と Adobe Workfront サーバー間の通信が開始されます。 詳しくは、[ファイアウォールの許可リストの設定](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)を参照してください。

また、組織がエンタープライズプランを使用している場合は、Workfront メール許可リストを作成して、どのメールドメインが Workfront からのメールの受け入れを許可されるか、そしてユーザーが Workfront ユーザープロファイルで指定するメールアドレスにどのメールドメインを含めることができるかを制御できます。 詳しくは、[メール許可リストの設定](../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md)を参照してください。

## IP アドレスをホワイトリストに追加

IP アドレスを Workfront 許可リストに追加すると、それらの IP アドレスのみが Workfront へのアクセスに使用できるようになります。 ユーザーが別の IP アドレスから Workfront にアクセスしようとすると、IP アドレスがブロックされていることを示すエラーメッセージが表示されます。

{{step-1-to-setup}}

1. **システム**／**顧客情報**&#x200B;をクリックします。

1. **IP 許可リスト**&#x200B;セクションで、「**IP 許可リストを有効にする**」を選択します。

   このオプションはデフォルトでは無効になっています。

1. Workfront システムへのアクセスに現在使用している IP アドレスを指定します。

   または

   Workfront システムへのアクセスに現在使用している IP アドレスを含む IP アドレスの範囲を指定します。

   Workfront へのアクセスに使用している IP アドレスは、許可リストを有効にする前に許可リストに加える必要があります。

1. 「**IP 範囲の追加**」をクリックし、Workfront にアクセスできるようにする IP アドレスまたは IP アドレスの範囲を指定します。
1. （オプション）前の手順を繰り返して、追加の IP アドレスまたは IP アドレス範囲を追加します。

   最大 75 個のアドレスまたは範囲を追加できます。

1. 「**保存**」をクリックします。
