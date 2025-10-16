---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 計算済みカスタムフィールドの例：イシューのカスタムフォームにイシュー作成者の管理者を表示する
description: 計算済みカスタムフィールドを使用すると、イシューに添付されたカスタムフォームにイシュー作成者の管理者の名前を表示できます。同じ文を使用して、プロジェクト、イシュー、その他のオブジェクトに類似した計算フィールドを作成できます。
author: Jenny
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
source-git-commit: a1ead6d0c1c85bfbe6d7302506743db8d8b3e205
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 92%

---

# 計算済みカスタムフィールドの例：イシューのカスタムフォームにイシュー作成者の管理者を表示する

計算済みカスタムフィールドを使用すると、イシューに添付されたカスタムフォームにイシュー作成者の管理者の名前を表示できます。同じ文を使用して、プロジェクト、イシュー、その他のオブジェクトに類似した計算フィールドを作成できます。

<!--outdated link: 
>[!TIP]
>
>For information about additional custom text mode examples from other customers, follow the [Text Mode Reporting](https://one.workfront.com/s/topic/0TO0z000000cdHmGAI/text-mode-reporting?tabset-21363=3) topic on our Community site.
-->

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront パッケージ</p> </td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront プラン</p> </td> 
   <td>
      <p>標準</p>
      <p>プラン</p></td>
  </tr> 
  <tr> 
   <td><p>アクセスレベル設定</p></td> 
   <td> <p>カスタムフォームへの管理アクセス</p> </td> 
  </tr> 
  <tr> 
   <td> <p>オブジェクト権限</p> </td> 
   <td> <p>カスタムフォームを編集するアクセス権を持つフォームが添付されたオブジェクトへのアクセス権を付与する</p></td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## イシューのカスタムフォームにイシュー作成者の管理者を表示する

次の手順は、イシューのカスタムフォームの計算済みフィールドの作成方法を示しています。そこでは、イシューを作成したユーザーの管理者の名前を取り込むことができます。タスク、プロジェクト、ポートフォリオなどを作成したユーザーの管理者名を取り込む場合、プロセスは同じです。

1. イシューのカスタムフォームを作成し、計算済みフィールドをフォームに追加する。

   カスタムフォームの作成方法とカスタムフォームに計算済みフィールドを追加する方法について詳しくは、次の記事を参照してください。

   * [カスタムフォームを作成](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)
   * [計算フィールドをフォームに追加する](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)

1. 次のテキストモードコードをカスタムフォームの&#x200B;**計算**&#x200B;フィールドにコピーして貼り付けます：

   ```
   {owner}.{manager}.{name}
   ```

   >[!TIP]
   >
   >カスタムフィールドの計算では大文字と小文字が区別されます。

1. 「**完了**」をクリックし、「**保存して閉じる**」を選択します。

   イシューを作成したユーザーの管理者は、そのフィールドを含むフォームがイシューに添付されると、計算済みフィールドに表示されます。
