---
title: 財務データへのアクセス権の付与
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: Adobe Workfront 管理者は、Workfront の財務データへのユーザーのアクセス権を、ユーザーのアクセスレベルによって定義できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: bf4a37ee-9435-4c1c-b18c-a7338a548ab7
source-git-commit: 8dbb48e6aa2df874caa816468cf2e3ad408ebf7e
workflow-type: ht
source-wordcount: '799'
ht-degree: 100%

---

# 財務データへのアクセス権の付与

{{highlighted-preview}}

Adobe Workfront 管理者は、[アクセスレベルの概要](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)の説明に従って、ユーザーのアクセスレベルによって、以下の情報対するユーザーのアクセス権を定義できます。

* Workfront のプロジェクトに関する財務情報
* リソース計画ツールのリソース予算計上情報

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p> <p><b>メモ</b>：まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 財務データへのアクセス権を付与する際の考慮事項

Workfront の財務データへのアクセス権をユーザーに付与する場合は、以下の点を考慮してください。

* アクセスレベルで財務データへのアクセスが許可されていないユーザーからは、プロジェクトに対するリスクは引き起こされません。詳しくは、[プロジェクトのリスクを作成および編集](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)を参照してください。
* また、アクセスレベルを使用して、ユーザーがリソース割り当ての予算を設定したり表示したりするために、どのリソース管理アクティビティを採用できるかを決定することもできます。詳しくは、[リソース管理へのアクセス権を付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)を参照してください。

## カスタムアクセスレベルを使用して財務データへのユーザーアクセスを設定

1. [カスタムアクセスレベルを作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)の説明に従って、アクセスレベルの作成または編集を開始します。
1. 財務データの右にある「**表示**」ボタンまたは「**編集**」ボタンの歯車アイコン![](assets/gear-icon-settings.png)をクリックし、続いて「**設定を微調整**」で付与する機能を選択します。

   ![](assets/financial-data-fine-tune-nwe.png)

1. （オプション）**管理アクセスを許可**&#x200B;エリアで、以下のオプションを選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">為替レート</td> 
      <td> <p>Workfront に新しい通貨を追加します。</p> <p>このアクセス権がない場合、ユーザーは作成するプロジェクトに既存の通貨のみを追加できます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">費用</td> 
      <td> <p>Workfront のオブジェクトに関するすべての費用を表示します。</p> <p>この場合、ユーザーは新しい費用タイプを作成できません。</p> <p>このアクセス権がない場合、ユーザーは次の項目のみを表示できます。</p> 
       <ul> 
        <li>管理するプロジェクト、タスクまたはイシューに関する費用</li> 
        <li>自身の費用</li> 
        <li>部下の費用</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション）作業中のアクセスレベルの他のオブジェクトやエリアのアクセス権を設定するには、[タスクへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)などの、[Adobe Workfront へのアクセス権を設定](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)にある記事に従って、作業を続けます。
1. 完了したら「**保存**」をクリックします。

   作成したアクセスレベルは、ユーザーに割り当てることができます。詳しくは、[ユーザープロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。

## 共有された財務情報へのアクセス権

[オブジェクトに対する財務権限の共有](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md)にある説明に従って、他のユーザーに権限を付与することにより、プロジェクト、タスクやイシューに関する財務情報を他のユーザーと共有できます。

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

別のユーザーとオブジェクトを共有する場合、そのオブジェクトに対する受信者の権限は次の 2 つ項目の組み合わせによって決まります。

* オブジェクトについて受信者に付与する権限
* オブジェクトのタイプについての受信者のアクセスレベル設定

## ライセンスタイプ別の財務情報へのアクセス権

それぞれのアクセスレベルのユーザーが財務情報に対して実行できる操作について詳しくは、[それぞれのオブジェクトタイプで使用できる機能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)の記事にある[財務データ](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia)の節を参照してください。

## 設定別の財務情報へのアクセス権

以下の情報は、アクセスレベル設定を使用して財務データへのユーザーのアクセスを制御する方法を理解するのに役立ちます。

### アクセスなし

財務データへのアクセス権を持たないユーザーは、次の項目にアクセスできません。

* プロジェクトおよびタスクオブジェクトの下にある「財務」セクション
* ビジネスケース
* 請求レートおよび請求レコード
* <span class="preview">評価カード</span>
* ユーザーの環境設定での 1 時間当たりのコストと 1 時間当たりの請求

  上記の手順 4 の「表示」ボタンにある歯車アイコン ![](assets/gear-icon-settings.png) で設定できます。

* 担当業務に関する 1 時間当たりのコストと 1 時間当たりの請求

  上記の手順 4 の「表示」ボタンにある歯車アイコン ![](assets/gear-icon-settings.png) で設定できます。

### 表示アクセス権

財務データへの表示アクセス権を持つユーザーは、次の項目を表示（編集は不可）できます。

* プロジェクトおよびタスクオブジェクトの下にある「財務」セクション
* ビジネスケース
* 請求レートおよび請求レコード
* ユーザーの環境設定での 1 時間当たりのコストと 1 時間当たりの請求

  上記の手順 4 の「表示」ボタンにある歯車アイコン ![](assets/gear-icon-settings.png) で設定できます。

* 担当業務に関する 1 時間当たりのコストと 1 時間当たりの請求

  上記の手順 4 の「表示」ボタンにある歯車アイコン ![](assets/gear-icon-settings.png) で設定できます。

### 編集アクセス権

財務データに対する編集アクセス権を持つユーザーは、次の項目を表示および編集できます。

* プロジェクトおよびタスクオブジェクトの下にある「財務」セクション
* ビジネスケース
* 請求レートおよび請求レコード
* <span class="preview">評価カード</span>
* ユーザーの環境設定での 1 時間当たりのコストと 1 時間当たりの請求

  上記の手順 4 の「編集」ボタンにある歯車アイコン ![](assets/gear-icon-settings.png) で設定できます。

* 担当業務に関する 1 時間当たりのコストと 1 時間当たりの請求

  上記の手順 4 の「編集」ボタンにある歯車アイコン ![](assets/gear-icon-settings.png) で設定できます。
