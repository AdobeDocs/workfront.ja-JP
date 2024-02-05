---
product-area: projects
navigation-topic: financials
title: プロジェクトレベルの請求レートの会社レベルの請求率での上書き
description: プロジェクトレベルの請求レートの会社レベルの請求率での上書き
author: Alina
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
source-git-commit: 72511f98e05c160e2ca69def8aa3a929ed62bb40
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 92%

---

# プロジェクトレベルの請求レートの会社レベルの請求率での上書き

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

プロジェクトレベルの請求料金の代わりに会社レベルの請求料金を使用するようにプロジェクトを設定できます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトおよび財務データへのアクセスを編集</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>財務を管理する権限を持つプロジェクトに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## 会社レベルの請求料金上書きオプションの有効化

会社がプロジェクトに関連付けられ、このオプションが有効になっている場合、会社レベルの請求料金を変更すると、プロジェクトで設定されている請求料金が上書きされます。

ユーザーがプロジェクトの財務を手動で再計算すると、会社レベルの請求料金に対する変更がすべて適用されます。収益計算の履歴も、請求済みとしてマークされていない限り上書きされます。

1. プロジェクトに移動します。
1. ヘッダーのプロジェクト名の横にある「**その他**」メニュー ![](assets/qs-more-icon-on-an-object.png) をクリックし、「**編集**」をクリックします。
1. 「**財務**」セクションで、「**会社レベルでの請求料金によるプロジェクトレベルの請求料金の上書きを許可**」を有効にします。

   >[!CAUTION]
   >
   >このオプションを有効にすると、請求済みとしてマークされていない限り、収益計算の履歴が上書きされます。請求記録を作成することで、収益計算の履歴を保持できます。詳しくは、[請求記録を作成](../../../manage-work/projects/project-finances/create-billing-records.md)の記事を参照してください。

1. 「**変更を保存**」をクリックします。

## 会社レベルの請求料金を更新してプロジェクトに適用

プロジェクトで会社レベルの請求料金上書きオプションを有効にした後、会社の請求料金に加えた変更は、財務が再計算されるたびにプロジェクトに適用されます。

>[!NOTE]
>
>会社レベルの請求料金を更新するには、ユーザーは自分のアクセスレベルで会社にアクセスできる必要があります。

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、「**設定**」をクリックします。
1. 「**会社**」をクリックします。
1. 会社レベルの請求料金の上書きを有効にしたプロジェクトに関連付けられている会社の名前をクリックします。
1. 左側のパネルで「**請求料金**」をクリックします。
1. を更新します。 **会社の請求率** 既存のジョブロールの開始日と終了日を入力し、Enter キーを押します。

   新しい日付有効な会社の請求率を追加するには、ジョブロールの請求率を選択し、 **編集**. 日付が有効な会社の請求料金について詳しくは、 [会社レベルでの担当業務請求料金の上書き](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md)を参照してください。

1. 1 つ以上のプロジェクトの会社の料金を更新するには、次のいずれかの操作を行います。

   * 複数のプロジェクト：

      1. プロジェクトのリストに移動します。
      1. 更新するプロジェクトに合わせてチェックボックスを選択します。
      1. 「**編集**」をクリックします。
      1. 「設定」セクションで、「**コストおよび収益の再計算**」オプションを有効にします。
      1. 「**変更を保存**」をクリックします。

   * 単一のプロジェクト：

      1. 会社レベルの請求料金の上書きを有効にしたプロジェクトに移動します。
      1. ヘッダーのプロジェクト名の横にある&#x200B;**その他** メニュー ![](assets/qs-more-icon-on-an-object.png) をクリックし、続いて「**財務を再計算**」をクリックします。
