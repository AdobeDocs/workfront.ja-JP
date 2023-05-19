---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 「計算済みカスタムフィールドの例：イシューの作成者の管理者をイシューのカスタムフォームに表示»
description: 計算済みのカスタムフィールドを使用すると、イシューに添付されたカスタムフォームに、イシューの作成者の管理者の名前を表示できます。 同じ文を使用して、プロジェクト、イシュー、その他のオブジェクトに類似した計算フィールドを作成できます。
author: Nolan
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 1%

---

# 計算済みカスタムフィールドの例：イシューの作成者の管理者をイシューのカスタムフォームに表示

計算済みのカスタムフィールドを使用すると、イシューに添付されたカスタムフォームに、イシューの作成者の管理者の名前を表示できます。 同じ文を使用して、プロジェクト、イシュー、その他のオブジェクトに類似した計算フィールドを作成できます。

<!--outdated link: 
>[!TIP]
>
>For information about additional custom text mode examples from other customers, follow the [Text Mode Reporting](https://one.workfront.com/s/topic/0TO0z000000cdHmGAI/text-mode-reporting?tabset-21363=3) topic on our Community site.
-->

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan*</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license*</p> </td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>アクセスレベル設定*</td> 
   <td> <p>カスタムフォームへの管理アクセス<br>アクセスレベルから管理アクセス権を付与する方法については、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定の領域に対する管理者アクセス権をユーザーに付与する</a>.</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>オブジェクト権限</p> </td> 
   <td> <p>カスタムフォームを編集するアクセス権を持つフォームが添付されたオブジェクトへのアクセス権を付与する</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## イシューの作成者の管理者をイシューのカスタムフォームに表示

次の手順は、イシューを作成したユーザーのマネージャーの名前を取り込む、イシューのカスタムフォームの計算フィールドの作成方法を示しています。 タスク、プロジェクト、ポートフォリオなどを作成したユーザーのマネージャ名を取り込む場合は、プロセスは同じです。

1. イシューのカスタムフォームを作成し、そのフォームに計算フィールドを追加します。

   カスタムフォームの作成と、カスタムフォームに計算フィールドを追加する方法について詳しくは、次の記事を参照してください。

   * [カスタムフォームの作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)
   * [計算データをカスタムフォームに追加する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)

1. 次のテキストモードコードを **計算** カスタムフォームのフィールド：

   ```
   {owner}.{manager}.{name}
   ```

   >[!TIP]
   >
   >カスタムフィールドの計算では、大文字と小文字が区別されます。

1. 「**完了**」をクリックし、「**保存して閉じる**」を選択します。

   イシューを作成したユーザーのマネージャーは、そのフィールドを含むフォームがイシューに添付されると、計算フィールドに表示されます。
