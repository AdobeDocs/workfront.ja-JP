---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: IP アドレスで Adobe Workfront へのアクセスを制限
description: Adobe Workfront IP 許可リストを設定して、Workfront へのアクセスを 45 個の IP アドレス、または指定した IP アドレスの範囲に制限することができます。これにより、Workfront アプリケーションのセキュリティレイヤーがさらに強化されます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: aed65b42-d534-453a-885d-f922114987bc
source-git-commit: 7bd3d2252b124a07a112aaa2b7798063087e7cab
workflow-type: ht
source-wordcount: '448'
ht-degree: 100%

---

# IP アドレスで Adobe Workfront へのアクセスを制限

Adobe Workfront IP 許可リストを設定して、Workfront へのアクセスを 45 個の IP アドレス、または指定した IP アドレスの範囲に制限することができます。これにより、Workfront アプリケーションのセキュリティレイヤーがさらに強化されます。

これらの IP アドレスまたは IP アドレス範囲は、ネットワーク管理者によって提供される必要があります。

## アクセス要件

この記事の手順を実行するには、以下を保有している必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>エンタープライズ</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p> <p><b>メモ</b>：まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## その他の許可リスト

ファイアウォールやメールサーバーが、特定のベンダーへのアクセスのみを許可するように設定されている場合は、特定の IP アドレスをその許可リストに追加する必要があります。これにより、環境と Adobe Workfront サーバー間の通信が開始されます。詳しくは、[ファイアウォールの許可リストの設定](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)を参照してください。

また、組織がエンタープライズプランを使用している場合は、Workfront メール許可リストを作成して、どのメールドメインが Workfront からのメールの受け入れを許可されるか、そしてユーザーが Workfront ユーザープロファイルで指定するメールアドレスにどのメールドメインを含めることができるかを制御できます。詳しくは、[メール許可リストの設定](../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md)を参照してください。

## IP アドレスをホワイトリストに追加

IP アドレスを Workfront 許可リストに追加すると、それらの IP アドレスのみが Workfront へのアクセスに使用できるようになります。ユーザーが別の IP アドレスから Workfront にアクセスしようとすると、IP アドレスがブロックされていることを示すエラーメッセージが表示されます。

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、「**設定**」![](assets/gear-icon-settings.png) をクリックします。

1. **システム**／**顧客情報**&#x200B;をクリックします。

1. **IP 許可リスト**&#x200B;セクションで、「**IP 許可リストを有効にする**」を選択します。

   このオプションはデフォルトでは無効になっています。

1. Workfront システムへのアクセスに現在使用している IP アドレスを指定します。

   または

   Workfront システムへのアクセスに現在使用している IP アドレスを含む IP アドレスの範囲を指定します。

   Workfront へのアクセスに使用している IP アドレスは、許可リストを有効にする前に許可リストに加える必要があります。

1. 「**IP 範囲の追加**」をクリックし、Workfront にアクセスできるようにする IP アドレスまたは IP アドレスの範囲を指定します。
1. （オプション）前の手順を繰り返して、追加の IP アドレスまたは IP アドレス範囲を追加します。

   最大 45 個のアドレスまたは範囲を追加できます。

1. 「**保存**」をクリックします。
