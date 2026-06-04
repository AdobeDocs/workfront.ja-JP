---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: なりすましを防止して [!DNL Adobe Workfront] SPF レコードを追加
description: ユーザーが [!DNL Adobe Workfront] メール通知を受け取らなかった場合は、ファイアウォールに [!DNL Workfront] SPF レコードを追加する必要があります。 SPF レコードを追加するには、IT チームと協力する必要があります。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: e93e3334-d72a-4f7b-9379-358f498c873b
TQID: https://experienceleague.adobe.com/6VnF205aiahPEWdP2kPk-YXF8UfPwSJ0-yJ6nGq3-FM
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 294
ht-degree: 97%

---

# スプーフィングの防止と [!DNL Adobe Workfront] SPF レコードの追加

## 問題

ユーザーが [!DNL Adobe Workfront] メール通知を受け取らなかった場合は、ファイアウォールに [!DNL Workfront] SPF レコードを追加する必要があります。 SPF レコードを追加するには、IT チームと協力する必要があります。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] パッケージ</td> 
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

[ファイアウォールの許可リストの設定](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)の説明に従って本番環境の許可リストに IP アドレスをすでに追加しているのに、ユーザーがまだメールを受信していない場合：

1. 次の SPF レコードをファイアウォールに追加します。

   *spf.workfront.com*

   これにより、すべての [!DNL Workfront] IP アドレスがファイアウォールの許可リストに自動的に追加され、（SPF レコードを使用する）すべてのスパムフィルターが [!DNL Workfront] サーバーをドメインの有効な送信者として検証できるようになります。

   >[!NOTE]
   >
   > SPF レコードは、DNS ゾーンファイルの一部である TXT レコードです。 DNS ゾーンファイルの変更はサポートされていません。

1. 設定する必要がある SPF レコードのタイプを指定する必要があります。 次に、有効な SPF レコードのタイプを示します。

   * all (https://dmarcian.com/spf-syntax-table/#all)
   * ip4 (https://dmarcian.com/spf-syntax-table/#ip4)
   * ip6 (https://dmarcian.com/spf-syntax-table/#ip6)
   * a (https://dmarcian.com/spf-syntax-table/#a)
   * mx (https://dmarcian.com/spf-syntax-table/#mx)
   * ptr (https://dmarcian.com/spf-syntax-table/#ptr)
   * exists (https://dmarcian.com/spf-syntax-table/#exists)
   * include (https://dmarcian.com/spf-syntax-table/#include)

   例えば、「v=spf1 a mx include: spf.workfront.com -all」とします。

会社ポリシーが原因で SPF レコードをファイアウォールに追加できない場合は、[!DNL Workfront] サポート担当者と協力してください。
