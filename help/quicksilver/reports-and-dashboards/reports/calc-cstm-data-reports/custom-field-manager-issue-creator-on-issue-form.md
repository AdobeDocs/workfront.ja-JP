---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 「計算済みカスタムフィールドの例：イシューのカスタムフォームにイシュー作成者の管理者を表示する」
description: 計算済みカスタムフィールドを使用すると、イシューに添付されたカスタムフォームにイシュー作成者の管理者の名前を表示できます。同じ文を使用して、プロジェクト、イシュー、その他のオブジェクトに類似した計算フィールドを作成できます。
author: Nolan
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: ht
source-wordcount: '413'
ht-degree: 100%

---

# 計算済みカスタムフィールドの例：イシューのカスタムフォームにイシュー作成者の管理者を表示する

計算済みカスタムフィールドを使用すると、イシューに添付されたカスタムフォームにイシュー作成者の管理者の名前を表示できます。同じ文を使用して、プロジェクト、イシュー、その他のオブジェクトに類似した計算フィールドを作成できます。

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
   <td> <p>Adobe Workfront プラン*</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront ライセンス*</p> </td> 
   <td> <p>プラン </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>アクセスレベル設定*</td> 
   <td> <p>カスタムフォームへの管理アクセス<br>アクセスレベルから管理アクセス権を付与する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定のエリアに対する管理者アクセス権をユーザーに付与する</a>を参照してください。</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>オブジェクト権限</p> </td> 
   <td> <p>カスタムフォームを編集するアクセス権を持つフォームが添付されたオブジェクトへのアクセス権を付与する</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## イシューのカスタムフォームにイシュー作成者の管理者を表示する

次の手順は、イシューのカスタムフォームの計算済みフィールドの作成方法を示しています。そこでは、イシューを作成したユーザーの管理者の名前を取り込むことができます。タスク、プロジェクト、ポートフォリオなどを作成したユーザーの管理者名を取り込む場合、プロセスは同じです。

1. イシューのカスタムフォームを作成し、計算済みフィールドをフォームに追加する。

   カスタムフォームの作成方法とカスタムフォームに計算済みフィールドを追加する方法について詳しくは、次の記事を参照してください。

   * [カスタムフォームの作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)
   * [計算済みデータをカスタムフォームに追加する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)

1. 次のテキストモードコードをカスタムフォームの&#x200B;**計算**&#x200B;フィールドにコピーして貼り付けます：

   ```
   {owner}.{manager}.{name}
   ```

   >[!TIP]
   >
   >カスタムフィールドの計算では大文字と小文字が区別されます。

1. 「**完了**」をクリックし、「**保存して閉じる**」を選択します。

   イシューを作成したユーザーの管理者は、そのフィールドを含むフォームがイシューに添付されると、計算済みフィールドに表示されます。
