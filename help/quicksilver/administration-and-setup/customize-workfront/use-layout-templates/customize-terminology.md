---
title: レイアウトテンプレートを使用したユーザーインターフェイス用語のカスタマイズ
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Adobe Workfront 管理者は、レイアウトテンプレートを使用して、Workfront 全体に表示される一部のオブジェクトのラベルを組織で使用されている用語に合わせて変更できます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3ab3ca43-d8e9-4545-a862-e6bf9419ef16
source-git-commit: 76e32fa6b87583d2b8c296045da731afdb6d1f9a
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 91%

---

# レイアウトテンプレートを使用したユーザーインターフェイスの用語のカスタマイズ

Adobe Workfront 管理者は、レイアウトテンプレートを使用して、Workfront 全体に表示される一部のオブジェクトのラベルを組織で使用されている用語に合わせて変更できます。

用語を変更したレイアウトテンプレートを保存し、Workfront からログアウトしてから再度ログインすると、Workfront のほとんどのエリアでデフォルトのラベルの代わりに変更したラベルが表示されます。

* メインメニュー
* メインメニューからアクセス可能なすべてのエリア
* すべてのタブ
* すべてのメニュー
* Report Builder とレポート要素（ビュー、フィルターおよびグループ化）
* 「保存」ボタン
* 書き出されたファイル
* メール
* モバイルアプリ

>[!NOTE]
>
>* Outlook アドインエリアには、カスタマイズされたラベルは表示されません。
>* ラベルをカスタマイズすると、文法やその他の問題が発生する場合があります。例えば、「Issue」を「Request」に変更すると、UI 内の場所に「An request」という語句が表示される場合があります。詳しくは、[Adobe Workfront のオブジェクトについて](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)の記事の[オブジェクト名のカスタマイズの影響](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#implications-of-customizing-object-names)を参照してください。
>

レイアウトテンプレートについて詳しくは、[レイアウトテンプレートの作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)を参照してください。

グループのレイアウトテンプレートについて詳しくは、[グループのレイアウトテンプレートの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)を参照してください。

レイアウトテンプレートを設定した後、変更を他のユーザーに表示するために、ユーザーに割り当てる必要があります。レイアウトテンプレートのユーザーへの割り当てについて詳しくは、[ユーザーのレイアウトテンプレートへの割り当て](../use-layout-templates/assign-users-to-layout-template.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td><p>標準</p>
       <p>プラン</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td> <p>これらの手順をシステムレベルで実行するには、システム管理者のアクセスレベルが必要です。</p>
        <p>グループに対して実行するには、そのグループの管理者である必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ユーザーインターフェイスの用語のカスタマイズ

1. [レイアウトテンプレートの作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)で説明されるように、レイアウトテンプレート上での作業を開始します。
1. ページの右上隅付近にある「**用語の設定**」をクリックします。
1. 次のいずれかの操作を行います。

   * Workfrontが提供する別の用語を使用するには、ラベルの横の下向き矢印 ![&#x200B; 下向き矢印 &#x200B;](assets/dropdown-arrow.png) をクリックし、ドロップダウン リストで必要なラベルをクリックします。

     >[!NOTE]
     >
     >ドロップダウンリストで提供される代替ラベルは、英語以外の言語用にローカライズされた Workfront のバージョンでサポートされています。

   * オブジェクトに対して表示されるラベルに独自の代替オプションを指定するには、ラベルの右側にある「**カスタム名を設定**」をクリックし、カスタム用語の&#x200B;**単数形**&#x200B;および&#x200B;**複数形**&#x200B;の形式を入力します。変更する場合は、「**リセット**」をクリックしてください。

     次のオブジェクト名をカスタマイズできます。

     <table style="table-layout:auto">
      <col>
      <col>
      <col>
      <tbody>
       <tr>
        <td role="rowheader"><p>Workfront オブジェクト</p></td>
        <td>
          <p>ポートフォリオ</p>
          <p>プログラム</p>
          <p>プロジェクト</p>
          <p>タスク</p>
          <p>イシュー</p>
          <p>目標</p>
          <p>結果</p>
          <p>アクティビティ</p>
         </ul></td>
        <td><p>これらのオブジェクトについて詳しくは、<a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Adobe Workfront のオブジェクトについて</a>を参照してください。</p></td>
       </tr>
       <tr>
        <td role="rowheader"><p>Workfront Goals オブジェクト</p></td>
        <td>
         <ul>
          <p>目標</p>
          <p>結果</p>
          <p>アクティビティ</p>
         </ul></td>
        <td><p>これらのオブジェクトには追加のライセンスが必要です。詳しくは、<a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Adobe Workfront Goals の概要</a>を参照してください。</p></td>
       </tr>
       <tr data-mc-conditions="">
        <td role="rowheader"><p>Workfront シナリオプランナオブジェクト</p></td>
        <td>
         <ul>
          <p>イニシアチブ</p>
          <p>シナリオ</p>
          <p>プラン </p>
         </ul></td>
        <td><p>これらのオブジェクトには追加のライセンスが必要です。詳しくは、<a href="../../../scenario-planner/get-started-with-scenario-planning.md" class="MCXref xref">シナリオプランナの概要</a>を参照してください。</p></td>
       </tr>
      </tbody>
     </table>

1. 完了したら、「**完了**」をクリックします。

   >[!TIP]
   >
   >完了をクリックした後（レイアウトテンプレートを保存した後）で、いつでも用語の設定の設定に戻り、カスタム用語の横にあるリセットをクリックしてデフォルト設定に戻すことができます。

1. 引き続きレイアウトテンプレートをカスタマイズします。

   または

   カスタマイズが完了したら、**保存**&#x200B;をクリックします。

1. 用語の変更を確認するには、次の操作を行います。

   1. ログアウトして、Workfront に再度ログインします。
   1. Workfront 環境で開いているすべてのブラウザータブを閉じます。

   >[!IMPORTANT]
   >
   >用語の変更前にレイアウトテンプレートを使用していたユーザーも、この操作を行う必要があります。

レイアウトテンプレートについて詳しくは、[レイアウトテンプレートの作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)を参照してください。
