---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: エラーメッセージ：無効なパラメーター：コンバージョン値
description: 既存のカスタムフォームでカスタムフィールドの形式を変更しようとすると、「無効なパラメーター：コンバージョン値'&lt;...&gt;」というエラーメッセージが表示されます
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4f7aac95-4afb-422d-877b-0fa49ef43883
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 84%

---

# エラーメッセージ：無効なパラメーター：コンバージョン値

## 問題

既存のカスタムフォームのカスタムフィールドの形式を変更しようとすると、次のエラーメッセージが表示されます。「無効なパラメーター: コンバージョン値 &quot;&lt;..>&quot;」\
![custom_field_format_invalid_parameter_error.png](assets/custom-field-format-invalid-parameter-error-350x148.png)

## 原因

このメッセージは、次のシナリオで発生します。

例えば、テキスト形式のカスタムフィールドがあるとします。次に、カスタムフィールドの形式を通貨に変更するとします。Adobe Workfront インスタンスのどこかで、このフィールドは既にオブジェクトに関連付けられており、その中で既に指定されている情報が含まれています。少なくとも 1 つのフィールドの既存の情報は、既にテキスト形式で書式設定されています。したがって、フィールドの形式を通貨に変更することはできません。

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
   <td> <p>次へのアクセスを編集：</p> 
    <ul> 
     <li> <p>レポート、ダッシュボードおよびカレンダーの作成</p> </li> 
     <li> <p>フィルター、ビュー、グループ化を作成</p> </li> 
    </ul>
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ソリューション

次の操作を実行します。

1. このフィールドがカスタムフォームに関連付けられている可能性のあるすべてのオブジェクトに関するレポートを作成します。\
   レポートの作成についての情報は、[カスタムレポートの作成](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)をご覧ください。

1. 編集しようとしているカスタムフィールドをレポートのビューに含めて、このフィールドにテキスト値が入力されているオブジェクトを確認できます。
1. テキスト形式で表示されるオブジェクトのカスタムフィールドの値を修正し、通貨形式の値を設定します。その後、カスタムフォームの書式フィールドを再度変更してみてください。\
   または\
   既にテキスト形式の情報が入力されているフィールド値が多すぎる場合は、新しいカスタムフィールドをカスタムフォームに追加して通貨形式にすることを検討してください。
