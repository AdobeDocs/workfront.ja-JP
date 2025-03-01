---
title: 各オブジェクトタイプの機能への設定可能なアクセス
description: この記事では、各アクセスレベルで、各オブジェクトタイプの Adobe Workfront 管理者として何が可能かについて説明します。また、アクセスレベルの各タイプのデフォルト設定についても説明します。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 94e0b205-140c-41c9-bb5a-f89b4c3aaea0
source-git-commit: 5d924e510ad94098b9f417494f9fc6e8696c90d6
workflow-type: tm+mt
source-wordcount: '3485'
ht-degree: 97%

---

# オブジェクトの種類ごとに機能へのアクセスを設定します。

組織のアクセスレベルを設定する際に、アクセスレベルで使用できる特定のアクションを決定できます。

この記事では、Adobe Workfront管理者がオブジェクトタイプごとに、各アクセスレベルで選択できるオプションについて説明します。 また、アクセスレベルの各タイプのデフォルト設定についても説明します。

例えば、Workfront管理者が特定のアクセスレベルのプロジェクトに対して「表示」を選択した場合、そのアクセスレベルを持つユーザーは、プロジェクトを表示できますが、編集することはできません。

各アクセスレベルのオブジェクトタイプで使用可能なすべての機能について詳しくは、[各オブジェクトタイプで使用できる機能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)を参照してください。

## プロジェクト

各アクセスレベルで、プロジェクトに対して次のオプションを設定できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>アクセスレベル</th> 
   <th>オプション</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>プランナー（プランライセンスタイプ）</td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li><p> <b>ビュー</b></p> <p>これを微調整するには、プロジェクトを共有する機能を設定します。「表示」ボタンで、歯車アイコン<img src="assets/gear-icon-in-access-levels.png"> をクリックし、「<b>共有</b>」オプションを無効または有効にします（デフォルトで有効）。</p> </li> 
     <li> <p><b>編集</b>（デフォルト選択）：プロジェクトへの完全な編集アクセスを許可します。</p> <p>これを微調整するには、「<b>編集</b>」ボタンで歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、次のオプションを無効または有効にします。これらはすべてデフォルトで有効になっています。</p> 
      <ul> 
       <li> <p>作成</p> </li> 
       <li> <p>コピー</p> </li> 
       <li> <p>削除</p> </li> 
       <li> <p>表示</p> </li> 
       <li> <p>共有</p> </li> 
       <li> <p>システム全体で共有</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>作業者 </td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li><p> <b>ビュー</b></p> <p>これを微調整するには、プロジェクトを共有する機能を設定します。「表示」ボタンで、歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、「<b>共有</b>」オプションを無効または有効にします（デフォルトで有効）。</p> </li> 
     <li> <p><b>編集</b>（デフォルト選択）：プロジェクトに対する完全な編集アクセスを許可します。Planner のアクセスレベルと比較して、Worker のアクセスレベルで編集アクセスが制限される方法を確認するには（プロジェクトに対する完全な編集アクセスを許可する）、<a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md" class="MCXref xref">各オブジェクトタイプで使用できる機能</a>の記事の<a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#projects" class="MCXref xref">プロジェクト</a>の節を参照してください。</p> <p>これを微調整するには、プロジェクトを共有する機能を設定します。「表示」ボタンで、歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、「<b>共有</b>」オプションを無効または有効にします（デフォルトで有効）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>レビュアー</td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li> <b>表示</b>（デフォルトの選択） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>依頼者</td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li><p> <b>ビュー</b></p> （デフォルトの選択） <p>プロジェクト共有を有効または無効にするために微調整できないので、表示アクセスは制限されています。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部ユーザー</td> 
   <td> <p>プロジェクトにアクセスできません。外部ユーザーは、Workfront を使用して、ドキュメントの確認とダウンロード、およびドキュメントと共有されているカレンダーの表示のみ行うことができます。</p> </td> 
  </tr> 
 </tbody> 
</table>

## タスク

各アクセスレベルで、タスクに対して次のオプションを設定できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>アクセスレベル</th> 
   <th>オプション</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>プランナー </td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li><p> <b>ビュー</b></p> <p>これを微調整するには、タスクを共有する機能を設定できます。「表示」ボタンで、歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、「<b>共有</b>」オプションを無効または有効にします（デフォルトで有効）。</p> </li> 
     <li> <p><b>編集</b>（デフォルト選択）：タスクへの完全な編集アクセスを許可します。</p> <p>これを微調整するには、「<b>編集</b>」ボタンで歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、次のオプションを無効または有効にします。これらはすべてデフォルトで有効になっています。</p> 
      <ul> 
       <li> <p>作成</p> </li> 
       <li> <p>削除</p> </li> 
       <li> <p>共有</p> </li> 
       <li> <p>システム全体で共有</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>作業者 </td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li><p> <b>ビュー</b></p> <p>これを微調整するには、タスクを共有する機能を設定できます。「表示」ボタンで、歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、「<b>共有</b>」オプションを無効または有効にします（デフォルトで有効）。</p> </li> 
     <li> <p><b>編集</b>（デフォルト選択）：タスクへの完全な編集アクセスを許可します。</p> <p>これを微調整するには、「<b>編集</b>」ボタンで歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、次のオプションを無効または有効にします。これらはすべてデフォルトで有効になっています。</p> 
      <ul> 
       <li> <p>作成</p> </li> 
       <li> <p>削除</p> </li> 
       <li> <p>共有</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>レビュアー</td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li> <b>表示</b>（デフォルトの選択） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>依頼者</td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li><p> <b>ビュー</b></p> （デフォルトの選択）<p>プロジェクト共有を有効または無効にするために微調整できないので、表示アクセスは制限されています。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部ユーザー</td> 
   <td> <p>タスクにアクセスできません。外部ユーザーは、Workfront を使用して、ドキュメントの確認とダウンロード、およびドキュメントと共有されているカレンダーの表示のみ行うことができます。</p> </td> 
  </tr> 
 </tbody> 
</table>

## イシュー

各アクセスレベルで、イシューに対して次のオプションを設定できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>アクセスレベル</th> 
   <th>オプション</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>プランナー </td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li> <p><b>表示</b></p><p>これを微調整するには、イシューを共有する機能を設定します。「表示」ボタンで、歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、「<b>共有</b>」オプションを無効または有効にします（デフォルトで有効）。</p> </li> 
     <li> <p><b>編集</b>（デフォルト選択）：イシューへの完全な編集アクセスを許可します。</p> <p>これを微調整するには、「<b>編集</b>」ボタンで歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、次のオプションのいずれかを無効または有効にします。これらはすべてデフォルトで有効になっています。</p> 
      <ul> 
       <li> <p>作成</p> </li> 
       <li> <p>削除</p> </li> 
       <li> <p>共有</p> </li> 
       <li> <p>システム全体で共有</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>作業者 </td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li><p> <b>ビュー</b></p> <p>これを微調整するには、イシューを共有する機能を設定します。「表示」ボタンで、歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、「<b>共有</b>」オプションを無効または有効にします（デフォルトで有効）。</p> </li> 
     <li> <p><b>編集</b>（デフォルト選択）：イシューへの完全な編集アクセスを許可します。</p> <p>これを微調整するには、「<b>編集</b>」ボタンで歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、次のオプションのいずれかを無効または有効にします。これらはすべてデフォルトで有効になっています。</p> 
      <ul> 
       <li> <p>作成</p> </li> 
       <li> <p>削除</p> </li> 
       <li> <p>共有</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>レビュアー</td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li><p> <b>ビュー</b></p> <p>これを微調整するには、イシューを共有する機能を設定します。「表示」ボタンで、歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、「<b>共有</b>」オプションを無効または有効にします（デフォルトで有効）。</p> </li> 
     <li> <p><b>編集</b>（デフォルト選択）：イシューへの完全な編集アクセスを許可します。</p> <p>これを微調整するには、「<b>編集</b>」ボタンで歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、次のオプションのいずれかを無効または有効にします。これらはすべてデフォルトで有効になっています。</p> 
      <ul> 
       <li> <p>作成</p> </li> 
       <li> <p>削除</p> </li> 
       <li> <p>共有</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>依頼者</td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li><p> <b>ビュー</b></p> <p>これを微調整するには、イシューを共有する機能を設定します。「表示」ボタンで、歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、「<b>共有</b>」オプションを無効または有効にします（デフォルトで有効）。</p> </li> 
     <li> <p><b>編集</b>（デフォルト選択）：イシューへの完全な編集アクセスを許可します。</p> <p>これを微調整するには、「<b>編集</b>」ボタンで歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、次のオプションのいずれかを無効または有効にします。これらはすべてデフォルトで有効になっています。</p> 
      <ul> 
       <li> <p>作成</p> </li> 
       <li> <p>削除</p> </li> 
       <li> <p>共有</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部ユーザー</td> 
   <td> <p>イシューにアクセスできません。外部ユーザーは、Workfront を使用して、ドキュメントの確認とダウンロード、およびドキュメントと共有されているカレンダーの表示のみ行うことができます。</p> </td> 
  </tr> 
 </tbody> 
</table>

## ポートフォリオ

各アクセスレベルで、ポートフォリオ用に次のオプションを設定できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>アクセスレベル</th> 
   <th>オプション</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>プランナー </td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li><p> <b>ビュー</b></p> <p>これを微調整するには、ポートフォリオを共有する機能を設定します。「表示」ボタンで、歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、「<b>共有</b>」オプションを無効または有効にします（デフォルトで有効）。</p> </li> 
     <li> <p><b>編集</b>（デフォルト選択）：ポートフォリオへの完全な編集アクセスを許可します。</p> <p>これを微調整するには、「<b>編集</b>」ボタンで歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、次のオプションのいずれかを無効または有効にします。これらはすべてデフォルトで有効になっています。</p> 
      <ul> 
       <li> <p>作成</p> </li> 
       <li> <p>削除</p> </li> 
       <li> <p>共有</p> </li> 
       <li> <p>システム全体で共有</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>作業者 </td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li> <b>表示</b>（デフォルトの選択） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>レビュアー</td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li> <b>表示</b>（デフォルトの選択）</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>依頼者</td> 
   <td> <p>ポートフォリオにアクセスできません。</p> </td> 
  </tr> 
  <tr> 
   <td>外部ユーザー</td> 
   <td> <p>ポートフォリオにアクセスできません。外部ユーザーは、Workfront を使用して、ドキュメントの確認とダウンロード、およびドキュメントと共有されているカレンダーの表示のみ行うことができます。</p> </td> 
  </tr> 
 </tbody> 
</table>

## プログラム

各アクセスレベルで、プロジェクトに対して次のオプションを設定できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>アクセスレベル</th> 
   <th>オプション</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>プランナー </td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li><p> <b>ビュー</b></p> <p>これを微調整するには、プログラムを共有する機能を設定します。「表示」ボタンで、歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、「<b>共有</b>」オプションを無効または有効にします（デフォルトで有効）。</p> </li> 
     <li> <p><b>編集</b>（デフォルト選択）：プログラムへの完全な編集アクセスを許可します。</p> <p>これを微調整するには、「<b>編集</b>」ボタンで歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、次のオプションのいずれかを無効または有効にします。これらはすべてデフォルトで有効になっています。</p> 
      <ul> 
       <li> <p>作成</p> </li> 
       <li> <p>削除</p> </li> 
       <li> <p>共有</p> </li> 
       <li> <p>システム全体で共有</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>作業者 </td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li> <b>表示</b>（デフォルトの選択） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>レビュアー</td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li> <b>表示</b>（デフォルトの選択）</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>依頼者</td> 
   <td> <p>プログラムにアクセスできません。</p> </td> 
  </tr> 
  <tr> 
   <td>外部ユーザー</td> 
   <td> <p>プログラムにアクセスできません。外部ユーザーは、Workfront を使用して、ドキュメントの確認とダウンロード、およびドキュメントと共有されているカレンダーの表示のみ行うことができます。</p> </td> 
  </tr> 
 </tbody> 
</table>

## レポート、ダッシュボード、カレンダー

各アクセスレベルで、レポート、ダッシュボードおよびカレンダーに対して次のオプションを設定できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>アクセスレベル</th> 
   <th>オプション</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>プランナー </td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li> <p><b>表示</b></p><p>これを微調整するには、「<b>編集</b>」ボタンで歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、次のアクションを無効または有効にします。どちらも、デフォルトで有効になっています。</p> 
      <ul> 
       <li> <p>組み込みレポートの表示</p> </li> 
       <li> <p>共有</p> </li> 
      </ul> </li> 
     <li> <p><b>編集</b>（デフォルトの選択）：レポート、ダッシュボード、カレンダーに対する完全な編集アクセスを許可します。</p> <p>これを微調整するには、「<b>編集</b>」ボタンの歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、次のオプションのいずれかを無効または有効にします。「<b>組み込みレポートの表示</b>」、「<b>レポートの公開共有</b>」、「<b>システム全体で共有</b>」を除き、これらはすべてデフォルトで有効になっています。</p> 
      <ul> 
       <li> <p>作成</p> </li> 
       <li> <p>削除</p> </li> 
       <li> <p>組み込みレポートの表示</p> </li> 
       <li> <p>共有</p> </li> 
       <li> <p>レポートの公開（外部）共有</p> </li> 
       <li> <p>システム全体で共有</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>作業者 </td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li><p> <b>ビュー</b></p> （デフォルトの選択）<p>これを微調整するには、「<b>編集</b>」ボタンの歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、次のアクションのいずれかを無効または有効にします。どちらも、デフォルトで有効になっています。</p> 
      <ul> 
       <li> <p>組み込みレポートの表示</p> </li> 
       <li> <p>共有</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>レビュアー</td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li> <p><b>表示</b>（デフォルトの選択）<p>これを微調整するには、「<b>編集</b>」ボタンの歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、次のアクションのいずれかを無効または有効にします。デフォルトでは、「共有」オプションのみが有効になっています。</p> 
      <ul> 
       <li> <p>組み込みレポートの表示</p> </li> 
       <li> <p>共有</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>依頼者</td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li> <p><b>表示</b>（デフォルトの選択）：共有されているレポート、ダッシュボードおよびカレンダーに対して、表示のみのアクセスを許可します。</p> <p>これを微調整するには、組み込みのレポートを表示する機能を設定します。「<b>表示</b>」ボタンの歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、<b>組み込みを表示</b>（デフォルトで無効）を無効または有効にします。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部ユーザー</td> 
   <td> <p>レポート、ダッシュボード、カレンダーにはアクセスできません。外部ユーザーは、Workfront を使用して、ドキュメントの確認とダウンロード、およびドキュメントと共有されているカレンダーの表示のみ行うことができます。</p> </td> 
  </tr> 
 </tbody> 
</table>

## フィルター、ビュー、グループ化

各アクセスレベルで、フィルター、ビュー、グループに対して次のオプションを設定できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>アクセスレベル</th> 
   <th>オプション</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>プランナー </td> 
   <td> 
    <ul> 
     <li> <p><b>表示</b></p><p>これを微調整するには、フィルター、ビュー、グループを共有する機能を設定します。「表示」ボタンの歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、「<b>共有</b>」オプション（デフォルトで有効）を無効または有効にします。</p> </li> 
     <li> <p><b>編集</b>（デフォルトの選択）：フィルター、ビュー、グループに対して完全な編集アクセスを許可します。</p> <p>これを微調整するには、「<b>編集</b>」ボタンの歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、次のオプションのいずれかを無効または有効にします。これらはすべてデフォルトで有効になっています。</p> 
      <ul> 
       <li> <p>作成</p> </li> 
       <li> <p>削除</p> </li> 
       <li> <p>共有</p> </li> 
       <li> <p>システム全体で共有</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>作業者 </td> 
   <td> 
    <ul> 
     <li> <p><b>表示</b></p><p>これを微調整するには、フィルター、ビュー、グループを共有する機能を設定します。「表示」ボタンの歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、「<b>共有</b>」オプション（デフォルトで有効）を無効または有効にします。</p> </li> 
     <li> <p><b>編集</b>（デフォルトの選択）：フィルター、ビュー、グループに対して完全な編集アクセスを許可します。</p> <p>これを微調整するには、「<b>編集</b>」ボタンの歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、次のオプションのいずれかを無効または有効にします。これらはすべてデフォルトで有効になっています。</p> 
      <ul> 
       <li> <p>作成</p> </li> 
       <li> <p>削除</p> </li> 
       <li> <p>共有</p> </li> 
       <li> <p>システム全体で共有</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>レビュアー</td> 
   <td> 
    <ul> 
     <li><p> <b>ビュー</b></p> <p>これを微調整するには、フィルター、ビュー、グループを共有する機能を設定します。「表示」ボタンの歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、「<b>共有</b>」オプション（デフォルトで有効）を無効または有効にします。</p> </li> 
     <li> <p><b>編集</b>（デフォルトの選択）：フィルター、ビュー、グループに対して完全な編集アクセスを許可します。</p> <p>これを微調整するには、「<b>編集</b>」ボタンの歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、次のオプションのいずれかを無効または有効にします。これらはすべてデフォルトで有効になっています。</p> 
      <ul> 
       <li> <p>作成</p> </li> 
       <li> <p>削除</p> </li> 
       <li> <p>共有</p> </li> 
       <li> <p>システム全体で共有</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>依頼者</td> 
   <td> 
    <ul> 
     <li> <p><b>ビュー</b>:</p> <p>これを微調整するには、フィルター、ビュー、グループを共有する機能を設定します。「表示」ボタンの歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、「<b>共有</b>」オプション（デフォルトで有効）を無効または有効にします。</p> </li> 
     <li> <p><b>編集</b>（デフォルトの選択）：フィルター、ビュー、グループに対して完全な編集アクセスを許可します。</p> <p>これを微調整するには、「<b>編集</b>」ボタンの歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、次のオプションのいずれかを無効または有効にします。これらはすべてデフォルトで有効になっています。</p> 
      <ul> 
       <li> <p>作成</p> </li> 
       <li> <p>削除</p> </li> 
       <li> <p>共有</p> </li> 
       <li> <p>システム全体で共有</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部ユーザー</td> 
   <td> <p>フィルター、ビュー、グループにはアクセスできません。外部ユーザーは、Workfront を使用して、ドキュメントの確認とダウンロード、およびドキュメントと共有されているカレンダーの表示のみ行うことができます。</p> </td> 
  </tr> 
 </tbody> 
</table>

## ドキュメント

各アクセスレベルで、ドキュメントに対して次のオプションを設定できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>アクセスレベル</th> 
   <th>オプション</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>プランナー </td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li><p> <b>ビュー</b></p> <p>これを微調整するには、ドキュメントを共有する機能を設定します。「表示」ボタンの歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、「<b>共有</b>」オプション（デフォルトで有効）を無効または有効にします。</p> </li> 
     <li> <p><b>編集</b>（デフォルトの選択）：ドキュメントへの完全な編集アクセスを許可します。</p> <p>これを微調整するには、「<b>編集</b>」ボタンで歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、次のオプションのいずれかを無効または有効にします。これらはすべてデフォルトで有効になっています（「<b>ドキュメントをパブリックにして共有</b>」および「<b>システム全体で共有</b>」を除く）。</p> 
      <ul> 
       <li> <p>作成</p> </li> 
       <li> <p>削除</p> </li> 
       <li> <p>共有</p> </li> 
       <li> <p>ドキュメントをパブリックにして共有（外部）</p> </li> 
       <li> <p>システム全体で共有</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>作業者 </td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li> <p><b>表示</b></p><p>これを微調整するには、ドキュメントを共有する機能を設定します。「表示」ボタンの歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、「<b>共有</b>」オプション（デフォルトで有効）を無効または有効にします。</p> </li> 
     <li> <p><b>編集</b>（デフォルトの選択）：ドキュメントへの完全な編集アクセスを許可します。</p> <p>これを微調整するには、「<b>編集</b>」ボタンで歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、次のオプションのいずれかを無効または有効にします。これらはすべてデフォルトで有効になっています（「<b>ドキュメントをパブリックにして共有</b>」および「<b>システム全体で共有</b>」を除く）。</p> 
      <ul> 
       <li> <p>作成</p> </li> 
       <li> <p>削除</p> </li> 
       <li> <p>共有</p> </li> 
       <li> <p>ドキュメントをパブリックにして共有（外部）</p> </li> 
       <li> <p>システム全体で共有</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>レビュアー</td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li><p> <b>ビュー</b></p> <p>これを微調整するには、ドキュメントを共有する機能を設定します。「表示」ボタンの歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、「<b>共有</b>」オプション（デフォルトで有効）を無効または有効にします。</p> </li> 
     <li> <p><b>編集</b>（デフォルトの選択）：ドキュメントへの完全な編集アクセスを許可します。</p> <p>これを微調整するには、「<b>編集</b>」ボタンで歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、次のアクションのいずれかを無効または有効にします。これらはすべてデフォルトで有効になっています（「<b>ドキュメントをパブリックにして共有</b>」および「<b>システム全体で共有</b>」を除く）。</p> 
      <ul> 
       <li> <p>作成</p> </li> 
       <li> <p>削除</p> </li> 
       <li> <p>共有</p> </li> 
       <li> <p>ドキュメントをパブリックにして共有（外部）</p> </li> 
       <li> <p>システム全体で共有</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>依頼者</td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li> <p><b>表示</b></p><p>これを微調整するには、ドキュメントを共有する機能を設定します。「表示」ボタンの歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、「<b>共有</b>」オプション（デフォルトで有効）を無効または有効にします。</p> </li> 
     <li> <p><b>編集</b>（デフォルトの選択）：ドキュメントへの完全な編集アクセスを許可します。</p> <p>これを微調整するには、「<b>編集</b>」ボタンで歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、次のオプションのいずれかを無効または有効にします。これらはすべてデフォルトで有効になっています。</p> 
      <ul> 
       <li> <p>作成</p> </li> 
       <li> <p>削除</p> </li> 
       <li> <p>共有</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部ユーザー</td> 
   <td> <p>このアクセスレベルでは、ドキュメントへのアクセスは設定できません。ただし、外部ユーザーは Workfront を使用して、ドキュメントの表示、レビュー、ダウンロードを行うことができます。</p> </td> 
  </tr> 
 </tbody> 
</table>

## ユーザー

各アクセスレベルで、ユーザーに次のオプションを設定できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>アクセスレベル</th> 
   <th>オプション</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>プランナー </td> 
   <td> 
    <ul> 
     <li> <p><b>ビュー</b></p><p>これを微調整するには、ユーザーの連絡先情報を表示する機能を設定します。「<b>表示</b>」ボタンで、歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、「<b>連作先情報を表示</b>」オプションを無効または有効にします（デフォルトで有効）。</p> </li> 
     <li> <p><b>編集</b>（デフォルト選択）：ユーザーに完全な編集アクセスを許可します。</p> <p>これを微調整するには、「<b>編集</b>」ボタンで歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、次のアクションのいずれかを無効または有効にします。最初の 2 つのオプション、「<b>作成</b>」および「<b>削除</b>」のみデフォルトで有効になっています。</p> 
      <ul> 
       <li> <p>作成</p> </li> 
       <li> <p>削除</p> </li> 
       <li>ユーザー管理者（すべてのユーザー）</li> 
       <li> <p>ユーザー管理者（グループユーザー）</p> </li> 
      </ul> <p>2 つのユーザー管理オプションについて詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>記事内の、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">カスタムアクセスレベルを使用してユーザーのアクセスを設定し、ユーザーを編集する</a>の節を参照してください。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>作業者 </td> 
   <td> 
    <ul> 
     <li><p> <b>表示</b>（使用可能なオプションのみ）</p><p>これを微調整するには、ユーザーの連絡先情報を表示する機能を設定します。「<b>表示</b>」ボタンで、歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、「<b>連絡先情報を表示</b>」オプションを無効または有効にします（デフォルトで有効）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>レビュアー</td> 
   <td> 
    <ul> 
     <li><p> <b>表示</b>（使用可能なオプションのみ）</p> <p>これを微調整するには、ユーザーの連絡先情報を表示する機能を設定します。「<b>表示</b>」ボタンで、歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、「<b>連絡先情報を表示</b>」オプションを無効または有効にします（デフォルトで無効）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>依頼者</td> 
   <td> 
    <ul> 
     <li> <p><b>表示</b>（使用可能なオプションのみ）</p><p>これを微調整するには、ユーザーの連絡先情報を表示する機能を設定します。「<b>表示</b>」ボタンで、歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、「<b>連絡先情報を表示</b>」オプションを無効または有効にします（デフォルトで無効）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部ユーザー</td> 
   <td> <p>ユーザーにアクセスできません。外部ユーザーは、Workfront を使用して、ドキュメントの確認とダウンロード、およびドキュメントと共有されているカレンダーの表示のみ行うことができます。</p> </td> 
  </tr> 
 </tbody> 
</table>

## チーム

各アクセスレベルで、チームの次のオプションを設定できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>アクセスレベル</th> 
   <th>オプション</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>プランナー </td> 
   <td> 
    <ul> 
     <li><b>ビュー</b> <p>これを微調整するには、「<b>表示</b>」ボタンで歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、次のオプションのいずれかを無効または有効にします。両方とも、デフォルトでは無効になっています。</p> 
      <ul> 
       <li>すべてのチームを表示</li> 
       <li> <p>自分のグループと関連付けられたチームを確認する</p> </li> 
      </ul> </li> 
     <li> <p><b>編集</b>（デフォルト選択）：チームに完全な編集アクセスを許可します。</p> <p>これを微調整するには、「<b>表示</b>」ボタンで歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、次のオプションのいずれかを無効または有効にします。これらはすべて、デフォルトで有効になっています（「<b>所属チームを編集</b>」を除く）。</p> 
      <ul> 
       <li>作成</li> 
       <li>削除</li> 
       <li> <p>所属チームを編集</p> </li> 
       <li> <p>自分が管理するグループのチームを編集する（グループ管理者のみ）</p> </li> 
       <li> <p>すべてのチームを表示</p> </li> 
       <li> <p>自分のグループと関連付けられたチームを確認する</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>作業者 </td> 
   <td> 
    <ul> 
     <li> <b>ビュー</b>
      <p>これを微調整するには、「<b>表示</b>」ボタンで歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、次のオプションのいずれかを無効または有効にします。両方とも、デフォルトで有効になっています。</p> 
      <ul> 
       <li>すべてのチームを表示</li> 
       <li> <p>自分のグループと関連付けられたチームを確認する</p> </li> 
      </ul> </li> 
     <li> <p><b>編集</b>（デフォルト選択）：チームに完全な編集アクセスを許可します。</p> <p>これを微調整するには、「<b>表示</b>」ボタンで歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、次のオプションのいずれかを無効または有効にします*。最初のオプションである「<b>所属するチームを編集</b>」のみが、デフォルトで無効になっています。</p> 
      <ul> 
       <li> <p>所属チームを編集</p> </li> 
       <li> <p>すべてのチームを表示</p> </li> 
       <li> <p>自分のグループと関連付けられたチームを確認する</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>レビュアー</td> 
   <td> 
    <ul> 
     <li> <p><b>表示</b>（使用可能なオプションのみ）</p> <p>これを微調整するには、「<b>表示</b>」ボタンで歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、次のオプションのいずれかを無効または有効にします*。両方とも、デフォルトで有効になっています。</p> 
      <ul> 
       <li> <p>すべてのチームを表示</p> </li> 
       <li>自分のグループと関連付けられたチームを確認する</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>依頼者</td> 
   <td> 
    <ul> 
     <li> <p><b>表示</b>（使用可能なオプションのみ）</p> <p>これを微調整するには、「<b>表示</b>」ボタンで歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、次のオプションのいずれかを無効または有効にします*。両方とも、デフォルトで有効になっています。</p> 
      <ul> 
       <li> <p>すべてのチームを表示</p> </li> 
       <li>自分のグループと関連付けられたチームを確認する</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部ユーザー</td> 
   <td> <p>チームにアクセスできません。外部ユーザーは、Workfront を使用して、ドキュメントの確認とダウンロード、およびドキュメントと共有されているカレンダーの表示のみ行うことができます。</p> </td> 
  </tr> 
 </tbody> 
</table>


## テンプレート

各アクセスレベルで、テンプレートに対して次のオプションを設定できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>アクセスレベル</th> 
   <th>オプション</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>プランナー </td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li><p> <b>ビュー</b></p> <p>これを微調整するには、テンプレートを共有する機能を設定します。「表示」ボタンの歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、「<b>共有</b>」オプション（デフォルトで有効）を無効または有効にします。</p> </li> 
     <li> <p><b>編集</b>（デフォルト選択）：テンプレートに対する完全な編集アクセスを許可します。</p> <p>これを微調整するには、「<b>編集</b>」ボタンで歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、次のオプションを無効または有効にします。これらはすべてデフォルトで有効になっています。</p> 
      <ul> 
       <li> <p>作成</p> </li> 
       <li> <p>削除</p> </li> 
       <li> <p>共有</p> </li> 
       <li> <p>システム全体で共有</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>作業者 </td> 
   <td> 
    <ul> 
     <li> <p><b>アクセスなし</b>（使用可能なオプションのみ）</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>レビュアー</td> 
   <td> 
    <ul> 
     <li> <p><b>アクセスなし</b>（使用可能なオプションのみ）</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>依頼者</td> 
   <td> 
    <ul> 
     <li> <p><b>アクセスなし</b>（使用可能なオプションのみ）</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部ユーザー</td> 
   <td> <p>テンプレートにアクセスできません。外部ユーザーは、Workfront を使用して、ドキュメントの確認とダウンロード、およびドキュメントと共有されているカレンダーの表示のみ行うことができます。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 財務データ

各アクセスレベルで、財務データに対して次のオプションを設定できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>アクセスレベル</th> 
   <th>オプション</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>プランナー </td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li> <p><b>ビュー</b>：</p> <p>これを微調整するには、「<b>表示</b>」ボタンで歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、次のオプションのいずれかを無効または有効にします*。両方とも、デフォルトで有効になっています。</p> 
      <ul> 
       <li>役割請求率と役割コスト率を表示</li> 
       <li> <p>ユーザー請求率とユーザーコスト率を表示</p> </li> 
      </ul> </li> 
     <li> <p><b>編集</b>（デフォルトの選択）：財務データに対する完全な編集アクセスを許可します。</p> <p>これを微調整するには、「<b>表示</b>」ボタンで歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、次のオプションのいずれかを無効または有効にします*。最後の 2 つのオプション、<b>ロールの請求とコスト率を表示</b>と<b>ユーザーの請求とコスト率を表示</b>のみがデフォルトで有効になっています。</p> 
      <ul> 
       <li>役割請求率と役割コスト率を編集</li> 
       <li> <p>ユーザー請求率とユーザーコスト率を編集</p> </li> 
       <li>役割請求率と役割コスト率を表示</li> 
       <li> <p>ユーザー請求率とユーザーコスト率を表示</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>作業者 </td> 
   <td> 
    <ul> 
     <li> <p><b>アクセスなし</b>（デフォルトの選択）</p> </li> 
     <li> <b>ビュー</b> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>レビュアー</td> 
   <td> 
    <ul> 
     <li> <p><b>アクセスなし</b>（デフォルトの選択）</p> </li> 
     <li><b>ビュー</b> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>依頼者</td> 
   <td> 
    <ul> 
     <li> <p><b>アクセスなし</b>（使用可能なオプションのみ）</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部ユーザー</td> 
   <td> <p>財務データにアクセスできません。外部ユーザーは、Workfront を使用して、ドキュメントの確認とダウンロード、およびドキュメントと共有されているカレンダーの表示のみ行うことができます。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;これらのオプションについて詳しくは、[請求と収益の概要](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md)を参照してください。

## リソース管理

各アクセスレベルで、リソース管理に対して次のオプションを設定できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>アクセスレベル</th> 
   <th>オプション</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>プランナー </td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li> <b>ビュー</b> </li> 
     <li> <p><b>編集</b>（デフォルトの選択）：リソース管理に対する完全な編集アクセスを許可します。</p> <p>これを微調整するには、「<b>編集</b>」ボタンの歯車アイコン <img src="assets/gear-icon-in-access-levels.png"> をクリックし、次のオプションのいずれかを無効または有効にします。最初のオプションである「<b>プランナーの優先度と予算計上時間を編集</b>」のみが、デフォルトで有効になっています。</p> 
      <ul> 
       <li> <p> プランナー内の優先度と予算計上時間数を編集します</p> </li> 
       <li> <p>リソースプールの管理</p> <p><b>メモ</b>：リソースプールを管理するには、財務データへの追加のアクセス権と、プロジェクトの財務の権限が必要です。財務データへのアクセス権を持たないプランナーユーザーにリソース管理アクセス権を付与した場合、ユーザーはリソースプランナーで時間別配分を表示できますが、原価ビューに切り替えたり、ビジネスケースを表示することはできません。詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">財務データへのアクセスの許可</a>および<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">オブジェクトに対する財務権限の共有</a>を参照してください。</p> </li> 
       <li> <p>ワークロードバランサーの予定時間数を更新する</p> <p><b>メモ</b>：ワークロードバランサーで予定時間をアップデートするには、ユーザーがオブジェクトに貢献する権限を持つ必要があります。詳細設定で「割り当ての作成」を有効にします。詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">オブジェクトに対する共有権限の概要</a>を参照してください。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>作業者 </td> 
   <td> 
    <ul> 
     <li><b>アクセスなし</b> </li> 
     <li> <b>表示</b>（デフォルトの選択） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>レビュアー</td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li> <b>表示</b>（デフォルトの選択）</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>依頼者</td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b>（使用可能なオプションのみ） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部ユーザー</td> 
   <td> <p>アクセスできません。外部ユーザーは、Workfront を使用して、ドキュメントの確認とダウンロード、およびドキュメントと共有されているカレンダーの表示のみ行うことができます。</p> </td> 
  </tr> 
 </tbody> 
</table>

## シナリオプランナーのエリア

すべてのアクセスレベルのデフォルト設定は、アクセスなしです。Workfront 管理者は、任意のプランナー、作業者、レビュアーのアクセスレベルに対して、これを表示アクセスまたは編集アクセスに変更できます。

<!--
DRAFTED IN FLARE:
Alina says: This will change overtime for some of the access levels, but right now once they get Edit access, they can do everything

-->

>[!NOTE]
>
>プランへのリンクが共有されている場合にのみ、別のユーザーが作成したプランを表示できます。

## Workfront Goals のエリア

デフォルトの 6 つのアクセスレベルのすべて（および 4 つのライセンスタイプのすべて）で、Workfront Goals を編集および表示できます。

編集がデフォルトのオプションです。
