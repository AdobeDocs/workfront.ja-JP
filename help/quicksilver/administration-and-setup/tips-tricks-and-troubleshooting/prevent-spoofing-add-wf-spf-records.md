---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: スプーフィングの防止と追加 [!DNL Adobe Workfront] SPF レコード
description: ユーザーが [!DNL Adobe Workfront] 電子メール通知： [!DNL Workfront] ファイアウォールに対する SPF レコード。 SPF レコードを追加するには、IT チームと協力する必要があります。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e93e3334-d72a-4f7b-9379-358f498c873b
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# スプーフィングの防止と追加 [!DNL Adobe Workfront] SPF レコード

## 問題

ユーザーが [!DNL Adobe Workfront] 電子メール通知： [!DNL Workfront] ファイアウォールに対する SPF レコード。 SPF レコードを追加するには、IT チームと協力する必要があります。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>次の条件を満たす必要があります。 [!DNL Workfront] 管理者。 詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> <p><b>注意</b>:まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者はアクセスレベルを変更できます。詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 解決策

実稼動環境用に既に IP アドレスを許可リストに追加している場合は、 [ファイアウォールの設定を許可リスト行う](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) ユーザーはまだメールを受信していません。

1. 次の SPF レコードをファイアウォールに追加します。

   *spf.workfront.com*

   これにより、 [!DNL Workfront] ファイアウォール上の許可リストへの IP アドレス。（SPF レコードを使用する）すべてのスパムフィルターが検証できるようにします。 [!DNL Workfront] サーバーを、お使いのドメインの有効な送信者として設定します。

   >[!NOTE]
   >
   > SPF レコードは、DNS ゾーンファイルの一部である TXT レコードです。 DNS ゾーンファイルの変更はサポートされていません。

1. 設定する必要がある SPF レコードの種類を指定する必要があります。 次に、有効な SPF レコードのタイプを示します。

   * すべて (https://dmarcian.com/spf-syntax-table/#all)
   * ip4 (https://dmarcian.com/spf-syntax-table/#ip4)
   * ip6 (https://dmarcian.com/spf-syntax-table/#ip6)
   * a (https://dmarcian.com/spf-syntax-table/#a)
   * mx (https://dmarcian.com/spf-syntax-table/#mx)
   * ptr (https://dmarcian.com/spf-syntax-table/#ptr)
   * が存在する (https://dmarcian.com/spf-syntax-table/#exists)
   * include (https://dmarcian.com/spf-syntax-table/#include)

   例えば、「v=spf1 a mx include: [spf.workfront.com](http://spf.workfront.com/) -all&quot;

会社ポリシーが原因で SPF レコードをファイアウォールに追加できない場合は、 [!DNL Workfront] サポート担当者。
