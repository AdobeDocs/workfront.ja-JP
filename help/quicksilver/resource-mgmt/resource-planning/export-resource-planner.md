---
product-area: resource-management
navigation-topic: resource-planning
title: リソースプランナーから情報を書き出す
description: リソースプランナーの任意のビューから、お使いのコンピューターに保存されている Excel （.xlsx）ファイルに情報を書き出すことができます。
author: Alina
feature: Resource Management
exl-id: 07acd28a-5dc0-45b4-bdf2-20abbd5e098c
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: ht
source-wordcount: '661'
ht-degree: 100%

---

# リソースプランナーから情報を書き出す

リソースプランナーの任意のビューから、お使いのコンピューターに保存されている Excel （.xlsx）ファイルに情報を書き出すことができます。

>[!IMPORTANT]
>
>表示する情報と、リソースプランナーから書き出すことのできる情報には、制限があります。これらの制限について詳しくは、[リソースプランナーの表示制限](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)を参照してください。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>Pro 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>レビュー以上 <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       (this seems to be the case in NWE only, not classic. Waiting on Vazgen's response for this)
      </MadCap:conditionalText>
     --></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクト、ユーザー、およびリソース管理に対する、表示以上のアクセス権</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対する、表示以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## リソースプランナーから情報を書き出す

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックします。

1. 「**リソース**」をクリックします。「**計画担当者**」がデフォルトで表示されます。

1. プランナーのビューを選択します。次のいずれかのオプションを選択できます。

   * ユーザー別に表示
   * プロジェクト別に表示
   * 役割別に表示

1. 「**書き出し**」をクリックします。

   エクスポートオプションダイアログボックスが表示されます。

   ![](assets/rp-export-options-box-350x421.png)

1. 次の情報を指定します。\
   **開始日**：書き出しの開始日。書き出したファイルには、ここで指定した日を含む週の最初の日から始まる、割り当てと空き時間に関する情報が含まれます。\
   **期間数**：ファイルに含める期間の数。デフォルトは 4 つの期間です。\
   **タイプ**：書き出したファイルに情報を表示する期間のタイプ（週、月または四半期）。\
   書き出すことのできる最大期間は次のとおりです。

   * 52 週間
   * 36 か月
   * 12 四半期

   **エクスポート対象を選択**：選択したビューに応じて、空き時間と予算計上の情報を書き出す対象として、画面に表示されるすべてのオブジェクトまたは特定のオブジェクトを選択できます。
次の情報の書き出しを選択できます。

   * プロジェクトビューでは、以下の書き出しを選択できます。

      * プロジェクト
      * プロジェクトと役割
      * すべて（これがデフォルトのオプションです）

   * ユーザービューでは、以下の書き出しを選択できます。

      * ユーザー
      * ユーザーとプロジェクト
      * すべて（これがデフォルトのオプションです）

   * 役割ビューで、書き出すアイテムを選択します。

      * 役割
      * 役割とプロジェクト
      * すべて（これがデフォルトのオプションです）

   **データフォーマット**：Excel ファイルの表示方法に応じて、次のいずれかのオプションを選択します。

   * **生**：これを選択すると、Excel ファイル内で属するオブジェクト別にグループ化されていない空き時間と配分情報が表示されます。（これはデフォルトのオプションです）
   * **グループ化**：これを選択すると、属するオブジェクト別にグループ化された空き時間および配分情報が表示されます。書き出された情報が、画面上の表示と同じように表示されます。

   書き出されたファイル内の情報がどのように表示されるかを示すサンプルが、エクスポートオプションダイアログボックスに表示されます。

1. 「**エクスポート**」をクリックして、リソースプランナーから情報を書き出します。\
   保存した情報のみが書き出されます。

1. （条件付き）役割ビューやプロジェクトビューに未保存の予算計上時間数がある場合は、「**保存して続行**」をクリックします。
お使いのコンピューターに Excel（.xlsx）ファイルがダウンロードされます。\
   ファイルのダウンロード準備中は、リソースプランナーからの書き出しは使用できません。\
   （条件付き）大量のデータを書き出すと、ファイルをダウンロードできるリンクが記載されたメールが届きます。\
   ![RP_eamil_with_exported_planner_attached.png](assets/rp-eamil-with-exported-planner-attached-350x116.png)

1. （条件付き）書き出したファイルが記載されたメールを受け取ったら、「**ダウンロード**」をクリックして、ファイルをダウンロードします。\
   これにより Workfront に戻り、ファイルをダウンロードできます。\
   ダウンロードを完了するには、Workfront にログインしている必要があります。\
   配信時にファイルをダウンロードしない場合、ダウンロードリンクは、書き出しを開始してから 7 日間有効です。
