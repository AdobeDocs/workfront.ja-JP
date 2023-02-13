---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'エラーメッセージ：無効なパラメータ：コンバージョン値'
description: 「既存のカスタムフォームのカスタムフィールドの形式を変更しようとすると、次のエラーメッセージが表示されます。'無効なパラメータ：コンバージョン値'&lt;...&gt;""
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7aac95-4afb-422d-877b-0fa49ef43883
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 1%

---

# エラーメッセージ：無効なパラメータ：コンバージョン値

## 問題

既存のカスタムフォームでカスタムフィールドの形式を変更しようとすると、次のエラーメッセージが表示されます。&quot;無効なパラメータ：コンバージョン値&quot;&lt;...>&quot;&quot;\
![custom_field_format_invalid_parameter_error.png](assets/custom-field-format-invalid-parameter-error-350x148.png)

## 原因

このメッセージは、次のシナリオで発生します。

例えば、テキスト形式のカスタムフィールドがあるとします。  次に、カスタムフィールドの形式を通貨に変更します。 任意の場所に [!DNL Adobe Workfront] インスタンス、このフィールドは既にオブジェクトにアタッチされており、既にオブジェクトに指定されている情報を持ちます。 少なくとも 1 つのフィールドの既存の情報は、既にテキスト形式で書式設定されています。 したがって、フィールドの形式を通貨に変更することはできません。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><a href="https://www.workfront.com/plans" target="_blank">[!DNL Workfront] 計画</a>*</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] ライセンスの概要</a>*</p> </td> 
   <td>計画</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>アクセスレベル*</strong> </td> 
   <td> <p>次へのアクセスを編集：</p> 
    <ul> 
     <li> <p>レポート、ダッシュボードおよびカレンダーの作成</p> </li> 
     <li> <p>フィルター、ビュー、グループの作成</p> </li> 
    </ul> <p><b>注意</b>:まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者は、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 解決策

次の操作を実行します。

1. このフィールドがカスタムFormsに関連付けられている可能性のあるすべてのオブジェクトのレポートを作成します。\
   レポートの作成について詳しくは、 [カスタムレポートの作成](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 編集しようとしているカスタムフィールドをレポートのビューに含めて、このフィールドにテキスト値が入力されているオブジェクトを確認できます。
1. テキスト形式で表示されるオブジェクトのカスタムフィールド値を修正し、通貨形式の値を指定します。次に、カスタムフォームの「形式」フィールドをもう一度変更しようとします。\
   または\
   既にテキスト形式の情報が入力されているフィールド値が多すぎる場合は、新しいカスタムフィールドをカスタムフォームに追加して通貨形式にすることを検討してください。
