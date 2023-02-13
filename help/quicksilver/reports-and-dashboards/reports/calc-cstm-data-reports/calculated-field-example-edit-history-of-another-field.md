---
content-type: reference
product-area: reporting
keywords: 監査，トレール，カスタム，フィールド
navigation-topic: calculate-custom-data-reports
title: 「計算済みカスタムフィールドの例：フィールドの編集履歴を表示»
description: ユーザーが定期的にカスタムフィールドを更新し、フィールドに加えられたすべての変更のログと変更が発生した日付を取り込む場合、この情報を計算カスタムフィールドに取り込むことができます。
author: Nolan
feature: Reports and Dashboards
exl-id: e233ef28-c95a-42a1-b2eb-448dad5feddb
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '666'
ht-degree: 0%

---

# 計算済みカスタムフィールドの例：フィールドの編集履歴を表示する

ユーザーが定期的にカスタムフィールドを更新し、フィールドに加えられたすべての変更のログと変更が発生した日付を取り込む場合、この情報を計算カスタムフィールドに取り込むことができます。

次の例は、 *手順の編集履歴* 1 行のテキストフィールド ( *説明*.

>[!TIP]
>
>この例は、1 行のテキストフィールドだけでなく、すべての種類のカスタムフィールドに対して使用できます。

これにより、次のことがおこなわれます。 

* 制限 *手順の編集履歴* フィールドに最新の 2,000 文字を入力して、Workfrontデータベースの制限内に収めます。
* 現在の *説明* フィールドは *手順の編集履歴* 値；空白であると仮定し、空でない場合は、次の処理を行います。 

   * 一致する場合は、 *手順の編集履歴* そのまま
   * 一致しない場合は、 *手順の編集履歴* が *説明* フィールドに続いて、括弧で囲まれた現在の日付、縦棒、前の日付が表示されます。 *手順の編集履歴*：入力された前の値と日付が保持されます。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <caption style="text-align: left;"> 
  <p>*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。</p> 
 </caption> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan*</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td> <p>Workfront license*</p> </td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td><strong>アクセスレベル設定*</strong> </td> 
   <td> <p>Custom Formsへの管理アクセス</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>オブジェクト権限</strong> </p> </td> 
   <td> <p>カスタムフォームに対する権限の管理 </p> <p>詳しくは、 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">カスタムフォームの共有</a>.<br></p> </td> 
  </tr> 
 </tbody> 
</table>

## 前提条件

フィールドの編集履歴を表示する計算フィールドをカスタムフォームに追加するには、まず次の操作を行う必要があります。

* カスタムフォームの作成
* 履歴を取得するフィールドをカスタムフォームに追加します

## フィールドの編集履歴を表示する

1. 計算フィールドを追加するカスタムフォームに移動します。

1. 例えば、1 行のテキストカスタムフィールドを作成するには、次の手順を実行します。

   1. クリック **1 行のテキストフィールド**.
   1. を指定します。 **ラベル** カスタムフィールドの場合： *説明*.
   1. クリック **アプリ**.

1. 選択 **フィールドを追加**&#x200B;を選択し、「 **計算済み** をクリックして、計算済みカスタムフィールドをフォームに追加します。
1. を指定します。 **ラベル** 計算されたカスタムフィールド（例： ） *手順の編集履歴*.

   これは、最初に作成したフィールド (*説明*) をクリックします。

1. クリック **保存して閉じる**.
1. 2 つのフィールドを追加したフォームの名前をクリックして、再度開きます。
1. 計算済みカスタムフィールドをクリックします。 *手順の編集履歴，* 次に、「計算」ボックスに次の内容をコピーして貼り付けます。
1. 内 **計算** フィールドで、カスタムフィールドに対して次の計算を指定します。

   ```
   LEFT(IF(LEFT({DE:Instructions Edit History},LEN(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})))={DE:Instructions},{DE:Instructions Edit History},CONCAT(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})," (",$$NOW,") | ",{DE:Instructions Edit History})),2000)
   ```

1. （推奨）同じ計算を **説明** フィールドを指定します。
1. 必ず  **テキスト** が **形式** 計算カスタムフィールドをテキスト形式で表すフィールド。

   これがデフォルトです。

1. クリック **保存して閉じる**.

   これで、カスタムフォームをオブジェクトに添付した後で、別のユーザーが *説明* 「*Instructions Edit History」フィールドには、最新の値が表示され、その後に括弧で囲まれた現在の日付と縦棒が表示されます。 さらに変更を加えると、同じ方法でこの情報に追加されます。

   上記の計算では、 *説明* 履歴を追跡する 1 行のテキストフィールドの名前と *手順の編集履歴* 計算フィールドの名前と完全に一致する
