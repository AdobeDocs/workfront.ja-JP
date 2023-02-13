---
title: レイアウトテンプレートを使用したユーザインターフェイスの用語のカスタマイズ
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Adobe Workfront管理者は、レイアウトテンプレートを使用して、Workfront全体で表示される一部のオブジェクトのラベルを、組織で使用されている用語に合わせて変更できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3ab3ca43-d8e9-4545-a862-e6bf9419ef16
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 3%

---

# レイアウトテンプレートを使用したユーザインターフェイスの用語のカスタマイズ

Adobe Workfront管理者は、レイアウトテンプレートを使用して、Workfront全体で表示される一部のオブジェクトのラベルを、組織で使用されている用語に合わせて変更できます。

用語を変更したレイアウトテンプレートを保存し、Workfrontからログアウトしてから再度ログインすると、変更したラベルがWorkfrontのほとんどの領域でデフォルトのラベルが表示される場所に表示されます。

* メインメニュー
* メインメニューからアクセスするすべての領域
* すべてのタブ
* すべてのメニュー
* Report Builderおよびレポート要素（ビュー、フィルターおよびグループ化）
* 保存ボタン
* 書き出されたファイル
* メール
* モバイルアプリ

>[!NOTE]
>
>* Outlook アドイン領域には、カスタマイズされたラベルは表示されません。
>* ラベルをカスタマイズすると、文法やその他の問題が発生する場合があります。 例えば、「Issue」を「Request」に変更すると、UI 内に「An request」というフレーズが表示される場所が存在する場合があります。 詳しくは、 [オブジェクト名のカスタマイズの影響](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#implications-of-customizing-object-names) 記事内 [Adobe Workfrontのオブジェクトについて](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
>


グループのレイアウトテンプレートについて詳しくは、 [グループのレイアウトテンプレートの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>これらの手順をシステムレベルで実行するには、システム管理者のアクセスレベルが必要です。
グループに対して実行するには、そのグループの管理者である必要があります。</p> <p><b>注意</b>:まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## ユーザーインターフェイスの用語のカスタマイズ

1. レイアウトテンプレートの使用を開始する ( [レイアウトテンプレートの作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. クリック **用語を設定** ページの右上隅付近にあります。
1. 次のいずれかの操作を行います。

   * Workfrontが提供する別の用語を使用するには、下向き矢印をクリックします  ![](assets/dropdown-arrow.png) ラベルの横にある、ドロップダウンリストで必要な代替ラベルをクリックします。

      >[!NOTE]
      >
      >ドロップダウンリストで提供される代替ラベルは、英語以外の言語用にローカライズされたWorkfrontのバージョンでサポートされています。

   * オブジェクトに対して表示されるラベルに独自の代替オプションを指定するには、 **カスタム名を設定** ラベルの右側にを入力し、 **単数** および **複数** カスタム用語の形式。 次をクリックできます。 **リセット** もし気が変われば

      次のオブジェクト名をカスタマイズできます。

      <table style="table-layout:auto">
      <col>
      <col>
      <col>
      <tbody>
       <tr>
        <td role="rowheader"><p>Workfrontオブジェクト</p></td>
        <td>
          <p>ポートフォリオ</p>
          <p>プログラム</p>
          <p>プロジェクト</p>
          <p>タスク</p>
          <p>問題</p>
          <p>目標</p>
          <p>結果</p>
          <p>アクティビティ</p>
         </ul></td>
        <td><p>これらのオブジェクトの詳細については、 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Adobe Workfrontのオブジェクトについて</a>.</p></td>
       </tr>
       <tr>
        <td role="rowheader"><p>Workfront Goals オブジェクト</p></td>
        <td>
         <ul>
          <p>目標</p>
          <p>結果</p>
          <p>アクティビティ</p>
         </ul></td>
        <td><p>これらのオブジェクトには追加のライセンスが必要です。 詳しくは、 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Adobe Workfront目標の概要</a>.</p></td>
       </tr>
       <tr data-mc-conditions="">
        <td role="rowheader"><p>Workfront Scenario Planner オブジェクト</p></td>
        <td>
         <ul>
          <p>イニシアチブ</p>
          <p>シナリオ</p>
          <p>計画 </p>
         </ul></td>
        <td><p>これらのオブジェクトには追加のライセンスが必要です。 詳しくは、 <a href="../../../scenario-planner/get-started-with-scenario-planning.md" class="MCXref xref">シナリオプランナーの概要</a>.</p></td>
       </tr>
      </tbody>
     </table>

1. 完了したら、「 **完了**.

   >[!TIP]
   >
   >「完了」をクリックした後（レイアウトテンプレートを保存した後でも）、いつでも用語の設定設定に戻り、カスタム用語の横にある「リセット」をクリックして、デフォルトの状態に戻すことができます。

1. 引き続きレイアウトテンプレートをカスタマイズします。

   または

   カスタマイズが終了したら、 **保存**.

1. 用語の変更を確認するには、次の手順に従います。

   1. ログアウトして、Workfrontに再度ログインします。
   1. Workfront環境用に開いているすべてのブラウザータブを閉じます。

   >[!IMPORTANT]
   >
   >また、用語を変更する前にレイアウトテンプレートを使用したユーザーに対しても必要です。

レイアウトテンプレートについて詳しくは、 [レイアウトテンプレートの作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
