---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 「エラーメッセージ：無効なパラメーター：コンバージョン値」
description: '「既存のカスタムフォームのカスタムフィールドの形式を変更しようとすると、次のエラーメッセージが表示されます。''無効なパラメーター : コンバージョン値 `<...>`''」'
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7aac95-4afb-422d-877b-0fa49ef43883
source-git-commit: 62d1b9563d83bd82b569e143f69e379e2f4ffbc2
workflow-type: ht
source-wordcount: '336'
ht-degree: 100%

---

# エラーメッセージ：無効なパラメーター：コンバージョン値

## 問題

既存のカスタムフォームのカスタムフィールドの形式を変更しようとすると、次のエラーメッセージが表示されます。「無効なパラメーター: コンバージョン値 &quot;&lt;..>&quot;」\
![custom_field_format_invalid_parameter_error.png](assets/custom-field-format-invalid-parameter-error-350x148.png)

## 原因

このメッセージは、次のシナリオで発生します。

例えば、テキスト形式のカスタムフィールドがあるとします。次に、カスタムフィールドの形式を通貨に変更するとします。Adobe Workfront インスタンスのどこかで、このフィールドは既にオブジェクトに関連付けられており、その中で既に指定されている情報が含まれています。少なくとも 1 つのフィールドの既存の情報は、既にテキスト形式で書式設定されています。したがって、フィールドの形式を通貨に変更することはできません。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><a href="https://www.workfront.com/plans" target="_blank">Workfront プラン</a>*</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">ライセンスの概要</a>*</p> </td> 
   <td>プラン</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>アクセスレベル*</strong> </td> 
   <td> <p>次へのアクセスを編集：</p> 
    <ul> 
     <li> <p>レポート、ダッシュボードおよびカレンダーの作成</p> </li> 
     <li> <p>フィルター、ビュー、グループ化を作成</p> </li> 
    </ul> <p><b>メモ</b>：まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## ソリューション

次の操作を実行します。

1. このフィールドがカスタムフォームに関連付けられている可能性のあるすべてのオブジェクトに関するレポートを作成します。\
   レポートの作成についての情報は、[カスタムレポートの作成](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)をご覧ください。

1. 編集しようとしているカスタムフィールドをレポートのビューに含めて、このフィールドにテキスト値が入力されているオブジェクトを確認できます。
1. テキスト形式で表示されるオブジェクトのカスタムフィールドの値を修正し、通貨形式の値を設定します。その後、カスタムフォームの書式フィールドを再度変更してみてください。\
   または\
   既にテキスト形式の情報が入力されているフィールド値が多すぎる場合は、新しいカスタムフィールドをカスタムフォームに追加して通貨形式にすることを検討してください。
