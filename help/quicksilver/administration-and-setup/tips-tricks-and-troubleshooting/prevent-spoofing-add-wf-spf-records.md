---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: スプーフィングの防止と [!DNL Adobe Workfront] SPF レコードの追加
description: ユーザーが [!DNL Adobe Workfront] メール通知を受け取らなかった場合は、ファイアウォールに [!DNL Workfront] SPF レコードを追加する必要があります。SPF レコードを追加するには、IT チームと協力する必要があります。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e93e3334-d72a-4f7b-9379-358f498c873b
source-git-commit: 8bcc2859b3b6ce7a264c8f234536a93b7761ab6b
workflow-type: ht
source-wordcount: '321'
ht-degree: 100%

---

# スプーフィングの防止と [!DNL Adobe Workfront] SPF レコードの追加

## 問題

ユーザーが [!DNL Adobe Workfront] メール通知を受け取らなかった場合は、ファイアウォールに [!DNL Workfront] SPF レコードを追加する必要があります。SPF レコードを追加するには、IT チームと協力する必要があります。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>[!DNL Workfront] の管理者になる必要があります。詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与</a>を参照してください。</p> <p><b>メモ</b>：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか [!DNL Workfront] 管理者にお問い合わせください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## ソリューション

[ファイアウォールの許可リストの設定](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)の説明に従って実稼動環境の許可リストに IP アドレスをすでに追加しているのに、ユーザーがまだメールを受信していない場合：

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
