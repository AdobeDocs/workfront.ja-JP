---
product-area: projects
navigation-topic: financials
title: プロジェクト・レベルの請求率を会社レベルの請求率で上書き
description: プロジェクト・レベルの請求率を会社レベルの請求率で上書き
author: Alina
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# プロジェクト・レベルの請求率を会社レベルの請求率で上書き

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

プロジェクトレベルの請求率の代わりに会社レベルの請求率を使用するようにプロジェクトを設定できます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトおよび財務データへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>財務を管理する権限を持つプロジェクトに対する権限を管理します</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 「会社レベルの請求率の上書き」オプションを有効にします

会社がプロジェクトに関連付けられ、このオプションが有効になっている場合、会社レベルの請求率を変更すると、プロジェクトで設定された請求率が上書きされます。

ユーザーがプロジェクト上の財務を手動で再計算すると、会社レベルの請求率に対する変更が適用されます。 過去の売上高の計算も、請求としてマークされない限り上書きされます。

1. プロジェクトに移動します。
1. 次をクリック： **詳細** メニュー ![](assets/qs-more-icon-on-an-object.png) ヘッダーのプロジェクト名の横にあるをクリックし、 **編集**.
1. 内 **金融** セクションで、 **会社レベルの請求率でプロジェクトレベルの請求率を上書きすることを許可**.

   >[!CAUTION]
   >
   >このオプションを有効にすると、請求済みとしてマークされていない限り、過去の売上高の計算が上書きされます。 請求レコードを作成することで、売上高の履歴計算を保持できます。 詳しくは、 [請求レコードの作成](../../../manage-work/projects/project-finances/create-billing-records.md)

1. クリック **変更を保存**.

## 会社レベルの請求率を更新し、プロジェクトに適用する

プロジェクトで会社レベルの請求率上書きオプションを有効にした後、会社の請求率に加えた変更は、財務が再計算されるたびにプロジェクトに適用されます。

>[!NOTE]
>
>会社レベルの請求率を更新するには、ユーザーはアクセスレベルで会社にアクセスできる必要があります。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定**.
1. クリック **会社**.
1. 会社レベルの請求率の上書きを有効にしたプロジェクトに関連付けられている会社名をクリックします。
1. クリック **請求率** をクリックします。
1. 既存のジョブロールの新しい請求率を **会社の請求率** 「 」フィールドで、Enter キーを押します。
1. 1 つ以上のプロジェクトの会社レートを更新するには、次のいずれかを実行します。

   * 複数のプロジェクト：
   1. プロジェクトのリストに移動します。
   1. 更新するプロジェクトに合わせてチェックボックスを選択します。
   1. クリック **編集**.
   1. 「設定」セクションで、 **コストと売上高を再計算** オプション。
   1. クリック **変更を保存**.
   * 単一のプロジェクト：

      1. 会社レベルの請求率の上書きを有効にしたプロジェクトに移動します。
      1. 次をクリック： **詳細** メニュー ![](assets/qs-more-icon-on-an-object.png) ヘッダーのプロジェクト名の横にあるをクリックし、 **財務の再計算**.
