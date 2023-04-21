---
title: 各オブジェクトタイプの機能への設定可能なアクセス
description: この記事では、各アクセスレベルで、各オブジェクトタイプのAdobe Workfront管理者として許可する機能について説明します。 また、アクセスレベルの各タイプのデフォルト設定についても説明します。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 94e0b205-140c-41c9-bb5a-f89b4c3aaea0
source-git-commit: df73ba291f0a0ab6492e6fabfb6de578ba7e1f1b
workflow-type: tm+mt
source-wordcount: '3435'
ht-degree: 10%

---

# 各オブジェクトタイプの機能への設定可能なアクセス

この記事では、各アクセスレベルで、各オブジェクトタイプのAdobe Workfront管理者として許可する機能について説明します。 また、アクセスレベルの各タイプのデフォルト設定についても説明します。

各アクセスレベルのオブジェクトタイプで使用可能なすべての機能については、 [各オブジェクトタイプで使用できる機能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

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
     <li><p> <b>ビュー</b></p> <p>これを微調整するには、プロジェクトを共有する機能を設定します。 歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> 「表示」ボタンで、 <b>共有</b> オプション（デフォルトで有効）。</p> </li> 
     <li> <p><b>編集</b> （デフォルトの選択）:プロジェクトへの完全な編集アクセスを許可します。</p> <p>これを微調整するには、歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>編集</b> ボタンをクリックし、次のオプションを無効または有効にします。 これらはすべてデフォルトで有効になっています。</p> 
      <ul> 
       <li> <p>作成</p> </li> 
       <li> <p>コピー</p> </li> 
       <li> <p>削除</p> </li> 
       <li> <p>ビュー</p> </li> 
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
     <li><p> <b>ビュー</b></p> <p>これを微調整するには、プロジェクトを共有する機能を設定します。 歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> 「表示」ボタンで、 <b>共有</b> オプション（デフォルトで有効）。</p> </li> 
     <li> <p><b>編集</b> （デフォルトの選択）:プロジェクトに対する編集アクセスを制限します。 Planner のアクセスレベルと比較して、Worker のアクセスレベルで編集アクセスが制限される方法を確認するには（プロジェクトに対する完全な編集アクセスを許可する）、「 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#projects" class="MCXref xref">プロジェクト</a> 記事内 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md" class="MCXref xref">各オブジェクトタイプで使用できる機能</a>.</p> <p>これを微調整するには、プロジェクトを共有する機能を設定します。 歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> 「編集」ボタンで、 <b>共有</b> オプション（デフォルトで有効）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>レビュアー</td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li> <b>表示</b> （デフォルトの選択） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>要求者</td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li><p> <b>ビュー</b></p> （デフォルトの選択） <p>表示アクセスは制限されています。表示アクセスを微調整して、プロジェクトの共有を有効または無効にすることができません。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部ユーザー</td> 
   <td> <p>プロジェクトにアクセスできません。 外部ユーザーは、Workfrontを使用して、ドキュメントの確認とダウンロード、およびドキュメントと共有されているカレンダーの表示のみおこなうことができます。</p> </td> 
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
   <td>計画担当者 </td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li><p> <b>ビュー</b></p> <p>これを微調整するには、タスクを共有する機能を設定します。 歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> 「表示」ボタンで、 <b>共有</b> オプション（デフォルトで有効）。</p> </li> 
     <li> <p><b>編集</b> （デフォルトの選択）:タスクへの完全な編集アクセスを許可します。</p> <p>これを微調整するには、歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>編集</b> ボタンをクリックし、次のオプションを無効または有効にします。 これらはすべてデフォルトで有効になっています。</p> 
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
     <li><p> <b>ビュー</b></p> <p>これを微調整するには、タスクを共有する機能を設定します。 歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> 「表示」ボタンで、 <b>共有</b> オプション（デフォルトで有効）。</p> </li> 
     <li> <p><b>編集</b> （デフォルトの選択）:タスクへの完全な編集アクセスを許可します。</p> <p>これを微調整するには、歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>編集</b> ボタンをクリックし、次のオプションを無効または有効にします。 これらはすべてデフォルトで有効になっています。</p> 
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
     <li> <b>表示</b> （デフォルトの選択） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>要求者</td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li><p> <b>ビュー</b></p> （デフォルトの選択）<p>表示アクセスは制限されています。表示アクセスを微調整して、プロジェクトの共有を有効または無効にすることができません。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部ユーザー</td> 
   <td> <p>タスクにアクセスできません。 外部ユーザーは、Workfrontを使用して、ドキュメントの確認とダウンロード、およびドキュメントと共有されているカレンダーの表示のみおこなうことができます。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 問題

各アクセスレベルで、問題に関する次のオプションを設定できます。

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
   <td>計画担当者 </td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li> <p><b>ビュー</b></p><p>これを微調整するには、イシューを共有する機能を設定します。 歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> 「表示」ボタンで、 <b>共有</b> オプション（デフォルトで有効）。</p> </li> 
     <li> <p><b>編集</b> （デフォルトの選択）:問題に対する完全な編集アクセスを許可します。</p> <p>これを微調整するには、歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>編集</b> ボタンをクリックし、次のオプションを無効または有効にします。 これらはすべてデフォルトで有効になっています。</p> 
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
     <li><p> <b>ビュー</b></p> <p>これを微調整するには、イシューを共有する機能を設定します。 歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> 「表示」ボタンで、 <b>共有</b> オプション（デフォルトで有効）。</p> </li> 
     <li> <p><b>編集</b> （デフォルトの選択）:問題に対する完全な編集アクセスを許可します。</p> <p>これを微調整するには、歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>編集</b> ボタンをクリックし、次のオプションを無効または有効にします。 これらはすべてデフォルトで有効になっています。</p> 
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
     <li><p> <b>ビュー</b></p> <p>これを微調整するには、イシューを共有する機能を設定します。 歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> 「表示」ボタンで、 <b>共有</b> オプション（デフォルトで有効）。</p> </li> 
     <li> <p><b>編集</b> （デフォルトの選択）:問題に対する完全な編集アクセスを許可します。</p> <p>これを微調整するには、歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>編集</b> ボタンをクリックし、次のオプションを無効または有効にします。 これらはすべてデフォルトで有効になっています。</p> 
      <ul> 
       <li> <p>作成</p> </li> 
       <li> <p>削除</p> </li> 
       <li> <p>共有</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>要求者</td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li><p> <b>ビュー</b></p> <p>これを微調整するには、イシューを共有する機能を設定します。 歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> 「表示」ボタンで、 <b>共有</b> オプション（デフォルトで有効）。</p> </li> 
     <li> <p><b>編集</b> （デフォルトの選択）:問題に対する完全な編集アクセスを許可します。</p> <p>これを微調整するには、歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>編集</b> ボタンをクリックし、次のオプションを無効または有効にします。 これらはすべてデフォルトで有効になっています。</p> 
      <ul> 
       <li> <p>作成</p> </li> 
       <li> <p>削除</p> </li> 
       <li> <p>共有</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部ユーザー</td> 
   <td> <p>問題にアクセスできません。 外部ユーザーは、Workfrontを使用して、ドキュメントの確認とダウンロード、およびドキュメントと共有されているカレンダーの表示のみおこなうことができます。</p> </td> 
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
   <td>計画担当者 </td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li><p> <b>ビュー</b></p> <p>これを微調整するには、ポートフォリオを共有する機能を設定します。 歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> 「表示」ボタンで、 <b>共有</b> オプション（デフォルトで有効）。</p> </li> 
     <li> <p><b>編集</b> （デフォルトの選択）:ポートフォリオへの完全な編集アクセスを許可します。</p> <p>これを微調整するには、歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>編集</b> ボタンをクリックし、次のオプションを無効または有効にします。 これらはすべてデフォルトで有効になっています。</p> 
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
     <li> <b>表示</b> （デフォルトの選択） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>レビュアー</td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li> <b>表示</b> （デフォルトの選択）</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>要求者</td> 
   <td> <p>ポートフォリオにアクセスできません。</p> </td> 
  </tr> 
  <tr> 
   <td>外部ユーザー</td> 
   <td> <p>ポートフォリオにアクセスできません。 外部ユーザーは、Workfrontを使用して、ドキュメントの確認とダウンロード、およびドキュメントと共有されているカレンダーの表示のみおこなうことができます。</p> </td> 
  </tr> 
 </tbody> 
</table>

## プログラム

各アクセスレベルで、プログラムに対して次のオプションを設定できます。

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
   <td>計画担当者 </td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li><p> <b>ビュー</b></p> <p>これを微調整するには、プログラムを共有する機能を設定します。 歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> 「表示」ボタンで、 <b>共有</b> オプション（デフォルトで有効）。</p> </li> 
     <li> <p><b>編集</b> （デフォルトの選択）:プログラムへの完全な編集アクセスを許可します。</p> <p>これを微調整するには、歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>編集</b> ボタンをクリックし、次のオプションを無効または有効にします。 これらはすべてデフォルトで有効になっています。</p> 
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
     <li> <b>表示</b> （デフォルトの選択） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>レビュアー</td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li> <b>表示</b> （デフォルトの選択）</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>要求者</td> 
   <td> <p>プログラムにアクセスできません。</p> </td> 
  </tr> 
  <tr> 
   <td>外部ユーザー</td> 
   <td> <p>プログラムにアクセスできません。 外部ユーザーは、Workfrontを使用して、ドキュメントの確認とダウンロード、およびドキュメントと共有されているカレンダーの表示のみおこなうことができます。</p> </td> 
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
   <td>計画担当者 </td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li> <p><b>ビュー</b></p><p>これを微調整するには、歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>編集</b> ボタン ) をクリックし、次のいずれかのアクションを無効または有効にします。 これらはどちらも、デフォルトで有効になっています。</p> 
      <ul> 
       <li> <p>組み込み報告書の表示</p> </li> 
       <li> <p>共有</p> </li> 
      </ul> </li> 
     <li> <p><b>編集</b> （デフォルトの選択）:レポート、ダッシュボード、カレンダーに対する完全な編集アクセスを許可します。</p> <p>これを微調整するには、歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>編集</b> ボタンをクリックし、次のオプションを無効または有効にします。 これらはすべて、を除き、デフォルトで有効になっています。 <b>組み込みレポートの表示</b>, <b>レポートを公開する</b>、および <b>システム全体で共有</b>.</p> 
      <ul> 
       <li> <p>作成</p> </li> 
       <li> <p>削除</p> </li> 
       <li> <p>組み込み報告書の表示</p> </li> 
       <li> <p>共有</p> </li> 
       <li> <p>公開（外部）でのレポートの共有</p> </li> 
       <li> <p>システム全体で共有</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>作業者 </td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li><p> <b>ビュー</b></p> （デフォルトの選択）<p>これを微調整するには、歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>編集</b> ボタンをクリックし、次のいずれかのアクションを無効または有効にします。 これらはどちらも、デフォルトで有効になっています。</p> 
      <ul> 
       <li> <p>組み込み報告書の表示</p> </li> 
       <li> <p>共有</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>レビュアー</td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li> <p><b>表示</b> （デフォルトの選択）<p>これを微調整するには、歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>編集</b> ボタンをクリックし、次のいずれかのアクションを無効または有効にします。 デフォルトでは、「共有」オプションのみが有効になっています。</p> 
      <ul> 
       <li> <p>組み込み報告書の表示</p> </li> 
       <li> <p>共有</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>要求者</td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li> <p><b>表示</b> （デフォルトの選択）:共有されているレポート、ダッシュボード、カレンダーに対して、表示のみのアクセスを許可します。</p> <p>これを微調整するには、組み込みのレポートを表示する機能を設定します。 歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>表示</b> ボタン、次に無効または有効 <b>組み込みの表示</b>（デフォルトでは無効）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部ユーザー</td> 
   <td> <p>レポート、ダッシュボード、カレンダーにアクセスすることはできません。 外部ユーザーは、Workfrontを使用して、ドキュメントの確認とダウンロード、およびドキュメントと共有されているカレンダーの表示のみおこなうことができます。</p> </td> 
  </tr> 
 </tbody> 
</table>

## フィルター、ビュー、グループ化

各アクセスレベルで、フィルター、ビューおよびグループに対して次のオプションを設定できます。

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
   <td>計画担当者 </td> 
   <td> 
    <ul> 
     <li> <p><b>ビュー</b></p><p>これを微調整するには、フィルター、ビューおよびグループを共有する機能を設定します。 歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> 「表示」ボタンで、 <b>共有</b> オプション（デフォルトで有効）。</p> </li> 
     <li> <p><b>編集</b> （デフォルトの選択）:フィルター、ビュー、グループに対する完全な編集アクセスを許可します。</p> <p>これを微調整するには、歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>編集</b> ボタンをクリックし、次のオプションを無効または有効にします。 これらはすべてデフォルトで有効になっています。</p> 
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
     <li> <p><b>ビュー</b></p><p>これを微調整するには、フィルター、ビューおよびグループを共有する機能を設定します。 歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> 「表示」ボタンで、 <b>共有</b> オプション（デフォルトで有効）。</p> </li> 
     <li> <p><b>編集</b> （デフォルトの選択）:フィルター、ビュー、グループに対する完全な編集アクセスを許可します。</p> <p>これを微調整するには、歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>編集</b> ボタンをクリックし、次のオプションを無効または有効にします。 これらはすべてデフォルトで有効になっています。</p> 
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
     <li><p> <b>ビュー</b></p> <p>これを微調整するには、フィルター、ビューおよびグループを共有する機能を設定します。 歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> 「表示」ボタンで、 <b>共有</b> オプション（デフォルトで有効）。</p> </li> 
     <li> <p><b>編集</b> （デフォルトの選択）:フィルター、ビュー、グループに対する完全な編集アクセスを許可します。</p> <p>これを微調整するには、歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>編集</b> ボタンをクリックし、次のオプションを無効または有効にします。 これらはすべてデフォルトで有効になっています。</p> 
      <ul> 
       <li> <p>作成</p> </li> 
       <li> <p>削除</p> </li> 
       <li> <p>共有</p> </li> 
       <li> <p>システム全体で共有</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>要求者</td> 
   <td> 
    <ul> 
     <li> <p><b>ビュー</b>:</p> <p>これを微調整するには、フィルター、ビューおよびグループを共有する機能を設定します。 歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> 「表示」ボタンで、 <b>共有</b> オプション（デフォルトで有効）。</p> </li> 
     <li> <p><b>編集</b> （デフォルトの選択）:フィルター、ビュー、グループに対する完全な編集アクセスを許可します。</p> <p>これを微調整するには、歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>編集</b> ボタンをクリックし、次のオプションを無効または有効にします。 これらはすべてデフォルトで有効になっています。</p> 
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
   <td> <p>フィルター、ビューおよびグループにアクセスすることはできません。 外部ユーザーは、Workfrontを使用して、ドキュメントの確認とダウンロード、およびドキュメントと共有されているカレンダーの表示のみおこなうことができます。</p> </td> 
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
   <td>計画担当者 </td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li><p> <b>ビュー</b></p> <p>これを微調整するには、ドキュメントを共有する機能を設定します。 歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> 「表示」ボタンで、 <b>共有</b> オプション（デフォルトで有効）。</p> </li> 
     <li> <p><b>編集</b> （デフォルトの選択）:ドキュメントへの完全な編集アクセスを許可します。</p> <p>これを微調整するには、歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>編集</b> ボタンをクリックし、次のオプションを無効または有効にします。 これらはすべて、を除き、デフォルトで有効になっています。 <b>ドキュメントを公に共有</b> および <b>システム全体で共有</b>.</p> 
      <ul> 
       <li> <p>作成</p> </li> 
       <li> <p>削除</p> </li> 
       <li> <p>共有</p> </li> 
       <li> <p>公開（外部）でのドキュメントの共有</p> </li> 
       <li> <p>システム全体で共有</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>作業者 </td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li> <p><b>ビュー</b></p><p>これを微調整するには、ドキュメントを共有する機能を設定します。 歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> 「表示」ボタンで、 <b>共有</b> オプション（デフォルトで有効）。</p> </li> 
     <li> <p><b>編集</b> （デフォルトの選択）:ドキュメントへの完全な編集アクセスを許可します。</p> <p>これを微調整するには、歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>編集</b> ボタンをクリックし、次のオプションを無効または有効にします。 これらはすべて、を除き、デフォルトで有効になっています。 <b>ドキュメントを公に共有</b> および <b>システム全体で共有</b>.</p> 
      <ul> 
       <li> <p>作成</p> </li> 
       <li> <p>削除</p> </li> 
       <li> <p>共有</p> </li> 
       <li> <p>公開（外部）でのドキュメントの共有</p> </li> 
       <li> <p>システム全体で共有</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>レビュアー</td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li><p> <b>ビュー</b></p> <p>これを微調整するには、ドキュメントを共有する機能を設定します。 歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> 「表示」ボタンで、 <b>共有</b> オプション（デフォルトで有効）。</p> </li> 
     <li> <p><b>編集</b> （デフォルトの選択）:ドキュメントへの完全な編集アクセスを許可します。</p> <p>これを微調整するには、歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>編集</b> ボタンをクリックし、次のいずれかのアクションを無効または有効にします。 これらはすべて、最後の 2 つを除き、デフォルトで有効になっています。 <b>ドキュメントを公に共有</b> および <b>システム全体で共有</b>.</p> 
      <ul> 
       <li> <p>作成</p> </li> 
       <li> <p>削除</p> </li> 
       <li> <p>共有</p> </li> 
       <li> <p>公開（外部）でのドキュメントの共有</p> </li> 
       <li> <p>システム全体で共有</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>要求者</td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li> <p><b>ビュー</b></p><p>これを微調整するには、ドキュメントを共有する機能を設定します。 歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> 「表示」ボタンで、 <b>共有</b> オプション（デフォルトで有効）。</p> </li> 
     <li> <p><b>編集</b> （デフォルトの選択）:ドキュメントへの完全な編集アクセスを許可します。</p> <p>これを微調整するには、歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>編集</b> ボタンをクリックし、次のオプションを無効または有効にします。 これらはすべてデフォルトで有効になっています。</p> 
      <ul> 
       <li> <p>作成</p> </li> 
       <li> <p>削除</p> </li> 
       <li> <p>共有</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部ユーザー</td> 
   <td> <p>このアクセスレベルでは、ドキュメントへのアクセスは設定できません。 ただし、外部ユーザーはWorkfrontを使用して、ドキュメントの表示、確認、ダウンロードをおこなうことができます。</p> </td> 
  </tr> 
 </tbody> 
</table>

## ユーザー

各アクセスレベルで、ユーザーに対して次のオプションを設定できます。

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
   <td>計画担当者 </td> 
   <td> 
    <ul> 
     <li> <p><b>ビュー</b></p><p>これを微調整するには、ユーザーの連絡先情報を表示する機能を設定します。 歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>表示</b> ボタンをクリックし、無効または有効にします。 <b>連絡先情報の表示</b> オプション（デフォルトで有効）。</p> </li> 
     <li> <p><b>編集</b> （デフォルトの選択）:ユーザーに対して完全な編集アクセスを許可します。</p> <p>これを微調整するには、歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>編集</b> ボタンをクリックし、次のいずれかのアクションを無効または有効にします。 最初の 2 つのオプションのみ <b>作成</b> および <b>削除</b>に設定され、デフォルトで有効になっています。</p> 
      <ul> 
       <li> <p>作成</p> </li> 
       <li> <p>削除</p> </li> 
       <li>ユーザー管理者 (すべてのユーザー)</li> 
       <li> <p>ユーザー管理者 (グループ ユーザー)</p> </li> 
      </ul> <p>2 つのユーザー管理オプションについて詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">カスタムアクセスレベルを使用してユーザーのアクセスを設定し、ユーザーを編集します</a> 記事内 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>作業者 </td> 
   <td> 
    <ul> 
     <li><p> <b>表示</b> （使用可能なオプションのみ）</p><p>これを微調整するには、ユーザーの連絡先情報を表示する機能を設定します。 歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>表示</b> ボタンをクリックし、無効または有効にします。 <b>連絡先情報の表示</b> オプション（デフォルトで有効）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>レビュアー</td> 
   <td> 
    <ul> 
     <li><p> <b>表示</b> （使用可能なオプションのみ）</p> <p>これを微調整するには、ユーザーの連絡先情報を表示する機能を設定します。 歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>表示</b> ボタンをクリックし、有効または無効にします。 <b>連絡先情報の表示</b> オプション（デフォルトでは無効）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>要求者</td> 
   <td> 
    <ul> 
     <li> <p><b>表示</b> （使用可能なオプションのみ）</p><p>これを微調整するには、ユーザーの連絡先情報を表示する機能を設定します。 歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>表示</b> ボタンをクリックし、有効または無効にします。 <b>連絡先情報の表示</b> オプション（デフォルトでは無効）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部ユーザー</td> 
   <td> <p>ユーザーにアクセスできません。 外部ユーザーは、Workfrontを使用して、ドキュメントの確認とダウンロード、およびドキュメントと共有されているカレンダーの表示のみおこなうことができます。</p> </td> 
  </tr> 
 </tbody> 
</table>

## チーム

各アクセスレベルで、チームに対して次のオプションを設定できます。

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
   <td>計画担当者 </td> 
   <td> 
    <ul> 
     <li><b>ビュー</b> <p>これを微調整するには、歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>表示</b> ボタンをクリックし、次のオプションを無効または有効にします*。 両方とも、デフォルトでは無効になっています。</p> 
      <ul> 
       <li>すべてのチームを表示</li> 
       <li> <p>自分のグループと関連付けられたチームを確認する</p> </li> 
      </ul> </li> 
     <li> <p><b>編集</b> （デフォルトの選択）:チームに対して完全な編集アクセスを許可します。</p> <p>これを微調整するには、歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>表示</b> ボタンをクリックし、次のオプションを無効または有効にします*。 これらはすべて、デフォルトで有効になっています ( ただし、 <b>自分の所属するチームを編集</b>.</p> 
      <ul> 
       <li>作成</li> 
       <li>削除</li> 
       <li> <p>所属チームを編集</p> </li> 
       <li> <p>自分が管理するグループのチームを編集する (グループ管理者のみ)</p> </li> 
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
      <p>これを微調整するには、歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>表示</b> ボタンをクリックし、次のオプションを無効または有効にします*。 両方とも、デフォルトで有効になっています。</p> 
      <ul> 
       <li>すべてのチームを表示</li> 
       <li> <p>自分のグループと関連付けられたチームを確認する</p> </li> 
      </ul> </li> 
     <li> <p><b>編集</b> （デフォルトの選択）:チームに対して完全な編集アクセスを許可します。</p> <p>これを微調整するには、歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>表示</b> ボタンをクリックし、次のオプションを無効または有効にします*。 最初のオプションのみ <b>自分の所属するチームを編集</b>に設定され、デフォルトでは無効になっています。</p> 
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
     <li> <p><b>表示</b> （使用可能なオプションのみ）</p> <p>これを微調整するには、歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>表示</b> ボタンをクリックし、次のオプションを無効または有効にします*。 両方とも、デフォルトで有効になっています。</p> 
      <ul> 
       <li> <p>すべてのチームを表示</p> </li> 
       <li>自分のグループと関連付けられたチームを確認する</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>要求者</td> 
   <td> 
    <ul> 
     <li> <p><b>表示</b> （使用可能なオプションのみ）</p> <p>これを微調整するには、歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>表示</b> ボタンをクリックし、次のオプションを無効または有効にします*。 両方とも、デフォルトで有効になっています。</p> 
      <ul> 
       <li> <p>すべてのチームを表示</p> </li> 
       <li>自分のグループと関連付けられたチームを確認する</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部ユーザー</td> 
   <td> <p>チームへのアクセスは利用できません。 外部ユーザーは、Workfrontを使用して、ドキュメントの確認とダウンロード、およびドキュメントと共有されているカレンダーの表示のみおこなうことができます。</p> </td> 
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
   <td>計画担当者 </td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li><p> <b>ビュー</b></p> <p>これを微調整するには、テンプレートを共有する機能を設定します。 歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> 「表示」ボタンで、 <b>共有</b> オプション（デフォルトで有効）。</p> </li> 
     <li> <p><b>編集</b> （デフォルトの選択）:テンプレートへの完全な編集アクセスを許可します。</p> <p>これを微調整するには、歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>編集</b> ボタンをクリックし、次のオプションを無効または有効にします。 これらはすべてデフォルトで有効になっています。</p> 
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
     <li> <p><b>アクセスなし</b> （使用可能なオプションのみ）</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>レビュアー</td> 
   <td> 
    <ul> 
     <li> <p><b>アクセスなし</b> （使用可能なオプションのみ）</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>要求者</td> 
   <td> 
    <ul> 
     <li> <p><b>アクセスなし</b> （使用可能なオプションのみ）</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部ユーザー</td> 
   <td> <p>テンプレートにアクセスできません。 外部ユーザーは、Workfrontを使用して、ドキュメントの確認とダウンロード、およびドキュメントと共有されているカレンダーの表示のみおこなうことができます。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 財務データ

各アクセス・レベルで、財務データに対して次のオプションを構成できます。

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
   <td>計画担当者 </td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li> <p><b>ビュー</b>:</p> <p>これを微調整するには、歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>表示</b> ボタンをクリックし、次のオプションを無効または有効にします*。 両方とも、デフォルトで有効になっています。</p> 
      <ul> 
       <li>役割請求率と役割コスト率を表示</li> 
       <li> <p>ユーザー請求率とユーザーコスト率を表示</p> </li> 
      </ul> </li> 
     <li> <p><b>編集</b> （デフォルトの選択）:財務データへの完全な編集アクセスを許可します。</p> <p>これを微調整するには、歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>表示</b> ボタンをクリックし、次のオプションを無効または有効にします*。 最後の 2 つのオプションのみ <b>ロールの請求とコスト率の表示</b> および <b>ユーザーの請求とコスト率の表示</b>に設定され、デフォルトで有効になっています。</p> 
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
     <li> <p><b>アクセスなし</b> （デフォルトの選択）</p> </li> 
     <li> <b>ビュー</b> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>レビュアー</td> 
   <td> 
    <ul> 
     <li> <p><b>アクセスなし</b> （デフォルトの選択）</p> </li> 
     <li><b>ビュー</b> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>要求者</td> 
   <td> 
    <ul> 
     <li> <p><b>アクセスなし</b> （使用可能なオプションのみ）</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部ユーザー</td> 
   <td> <p>財務データにアクセスできません。 外部ユーザーは、Workfrontを使用して、ドキュメントの確認とダウンロード、およびドキュメントと共有されているカレンダーの表示のみおこなうことができます。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; これらのオプションについて詳しくは、 [請求と売上高の概要](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

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
   <td>計画担当者 </td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li> <b>ビュー</b> </li> 
     <li> <p><b>編集</b> （デフォルトの選択）:リソース管理への完全な編集アクセスを許可します。</p> <p>これを微調整するには、歯車アイコンをクリックします。 <img src="assets/gear-icon-in-access-levels.png"> の <b>編集</b> ボタンをクリックし、次のオプションを無効または有効にします。 最初のオプションのみ <b>プランナーの優先度と予算時間を編集</b>：デフォルトで有効になっています。</p> 
      <ul> 
       <li> <p> プランナー内の優先度と予算計上時間数を編集します</p> </li> 
       <li> <p>リソース プールの管理</p> <p><b>注意</b>:リソースプールを管理するには、財務データに対する追加のアクセス権と、財務をプロジェクトする権限が必要です。 財務データにアクセスできないプランナ・ユーザーに資源管理アクセス権を付与した場合、ユーザーは「資源プランナ」で時間別割当を表示できますが、「原価」ビューに切り替えたり、ビジネス・ケースを表示することはできません。 詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">財務データへのアクセス権の付与</a> および <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">オブジェクトに対する財務権限の共有</a>.</p> </li> 
       <li> <p>ワークロード バランサーの予定時間数を更新する</p> <p><b>注意</b>:ワークロードバランサーで予定時間を更新するには、[ 詳細設定 ] で [ 割り当てを行う ] を有効にして、オブジェクトに貢献する権限が必要です。 詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">オブジェクトに対する共有権限の概要</a>.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>作業者 </td> 
   <td> 
    <ul> 
     <li><b>アクセスなし</b> </li> 
     <li> <b>表示</b> （デフォルトの選択） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>レビュアー</td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> </li> 
     <li> <b>表示</b> （デフォルトの選択）</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>要求者</td> 
   <td> 
    <ul> 
     <li> <b>アクセスなし</b> （使用可能なオプションのみ） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部ユーザー</td> 
   <td> <p>アクセスできません。 外部ユーザーは、Workfrontを使用して、ドキュメントの確認とダウンロード、およびドキュメントと共有されているカレンダーの表示のみおこなうことができます。</p> </td> 
  </tr> 
 </tbody> 
</table>

## シナリオプランナー領域

すべてのアクセスレベルのデフォルト設定は、[ アクセスなし ] です。 Workfront管理者は、任意のプランナー、ワーカー、レビュー担当者のアクセスレベルに対して、これを「表示」または「編集」アクセス権に変更できます。

<!--
DRAFTED IN FLARE:
Alina says: This will change overtime for some of the access levels, but right now once they get Edit access, they can do everything

-->

>[!NOTE]
>
>プランへのリンクが共有されている場合にのみ、別のユーザーが作成したプランを表示できます。

## Workfront Goals 領域

デフォルトの 6 つのアクセスレベル（および 4 つのライセンスタイプのすべて）すべてで、Workfront目標を編集および表示できます。

デフォルトのオプションは「編集」です。
