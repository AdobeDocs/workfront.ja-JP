---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: スプーフィングの防止と SPF レコード  [!DNL Adobe Workfront]  追加
description: ユーザーが [!DNL Adobe Workfront] メール通知を受け取らなかった場合は、ファイアウォールに [!DNL Workfront] SPF レコードを追加する必要があります。SPF レコードを追加するには、IT チームと協力する必要があります。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: e93e3334-d72a-4f7b-9379-358f498c873b
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 92%

---

# スプーフィングの防止と [!DNL Adobe Workfront] SPF レコードの追加

## 問題

ユーザーが [!DNL Adobe Workfront] メール通知を受け取らなかった場合は、ファイアウォールに [!DNL Workfront] SPF レコードを追加する必要があります。SPF レコードを追加するには、IT チームと協力する必要があります。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
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
   > SPF レコードは、DNS ゾーンファイルの一部である TXT レコードです。DNS ゾーンファイルの変更はサポートされていません。

1. 設定する必要がある SPF レコードのタイプを指定する必要があります。次に、有効な SPF レコードのタイプを示します。

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
