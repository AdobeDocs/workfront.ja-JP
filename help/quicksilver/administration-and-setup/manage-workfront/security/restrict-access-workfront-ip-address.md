---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: IP アドレスでAdobe Workfrontへのアクセスを制限する
description: Workfrontへのアクセスを指定した 45 個の IP アド許可リストレスまたは IP アドレスの範囲に制限するAdobe Workfront IP アドレスを設定できます。 これにより、Workfrontアプリケーションのセキュリティレイヤーがさらに強化されます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: aed65b42-d534-453a-885d-f922114987bc
source-git-commit: 7bd3d2252b124a07a112aaa2b7798063087e7cab
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# IP アドレスでAdobe Workfrontへのアクセスを制限する

Workfrontへのアクセスを指定した 45 個の IP アド許可リストレスまたは IP アドレスの範囲に制限するAdobe Workfront IP アドレスを設定できます。 これにより、Workfrontアプリケーションのセキュリティレイヤーがさらに強化されます。

これらの IP アドレスまたは IP アドレスの範囲は、ネットワーク管理者が提供する必要があります。

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td> <p>エンタープライズ</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront管理者である。</p> <p><b>注意</b>:まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## その他の許可リスト

ファイアウォールまたはメールサーバーが特定のベンダーへのアクセスのみを許可するように設定されている場合は、特定の IP アドレスをそのに追加する必要があ許可リストります。 これにより、環境とAdobe Workfrontサーバー間の通信が開始されます。 詳しくは、 [ファイアウォールの設定を許可リスト行う](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

また、Enterprise プランを使用している場合は、Workfront電子メールドメインを設定して、Workfrontからの電子メールを受け入れる許可を受け入れる電子メールドメイン許可リストと、Workfrontユーザープロファイルでユーザーが指定した電子メールアドレスに含める電子メールドメインを制御できます。 詳しくは、 [電子メールの設定を許可リスト行う](../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).

## IP アドレスのへの許可リスト追加

Workfrontに IP アドレスを追加した後許可リストは、Workfrontへのアクセスに使用できるのは、それらの IP アドレスのみです。 別の IP アドレスからWorkfrontにアクセスしようとするユーザーには、IP アドレスがブロックされていることを示すエラーメッセージが表示されます。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **システム** > **顧客情報。**

1. 内 **IP の許可リスト** セクション、選択 **IP の有効化を許可リスト行います。**

   このオプションはデフォルトでは無効になっています。

1. Workfrontシステムへのアクセスに現在使用している IP アドレスを指定します。

   または

   Workfrontシステムへのアクセスに現在使用している IP アドレスを含む IP アドレスの範囲を指定します。

   Workfrontにアクセスするために使用している IP アドレスは、アドレスが有効になる前許可リストに、に追加する必要がありま許可リストす。

1. クリック **IP 範囲を追加** 次に、Workfrontにアクセスする IP アドレスまたは IP アドレスの範囲を指定します。
1. （オプション）前の手順を繰り返して、IP アドレスまたは IP アドレス範囲を追加します。

   最大 45 個のアドレスまたは範囲を追加できます。

1. クリック **保存します。**
