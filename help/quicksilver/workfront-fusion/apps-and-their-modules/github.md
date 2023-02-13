---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: GitHub モジュール
description: 内 [!DNL Adobe Workfront Fusion] シナリオを使用すると、GitHub を使用するワークフローを自動化でき、また、それを複数のサードパーティのアプリケーションやサービスに接続することができます。
author: Becky
feature: Workfront Fusion
exl-id: 5e520aab-8307-4a52-96b6-13b284f9cb53
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1796'
ht-degree: 0%

---

# [!DNL GitHub] モジュール

内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!UICONTROL GitHub]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画*</td>
  <td> <p>[!UICONTROL Pro] 以降</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td>
   <td> <p>[!UICONTROL プラン ]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 前提条件

使用する [!DNL GitHub] モジュール、 [!DNL GitHub] アカウント

## 接続 [!DNL GitHub] から [!DNL Workfront Fusion]

接続方法 [!DNL GitHub] アカウント [!UICONTROL Workfront Fusion]を参照してください。 [への接続の作成 [!UICONTROL Adobe Workfront Fusion]  — 基本手順](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL GitHub] モジュールとそのフィールド。

設定時に [!DNL GitHub] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL GitHub] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [トリガー](#triggers)
* [アクション](#actions)

### トリガー

* [[!UICONTROL 問題を見る]](#watch-issues)
* [[!UICONTROL 監視リポジトリ]](#watch-repositories)
* [[!UICONTROL 監視フォーク]](#watch-forks)
* [[!UICONTROL コメントを見る]](#watch-comments)
* [[!UICONTROL プル要求の監視]](#watch-pull-requests)

#### [!UICONTROL 問題を見る]

このモジュールは、新しいイシューが追加されたり、既存のイシューが変更されたりするとトリガーします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL GitHub] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 視聴する</td> 
   <td>すべてのリポジトリを監視するか、1 つのリポジトリのみを監視するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リポジトリ ]</td> 
   <td>1 つのリポジトリのみの問題の監視を選択した場合は、監視するリポジトリを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 返された問題の最大数 ]</td> 
   <td>結果の最大数を設定 [!DNL Workfront Fusion] は、1 サイクルの間にと連携します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ウォッチ ]</td> 
   <td>新しい問題のみを監視するか、新しい問題とすべての変更を監視するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フィルター ]</td> 
   <td> <p>監視する問題を、その問題との関連付けによってフィルタリングできます。</p> 
    <ul> 
     <li>[!UICONTROL すべての問題 ]</li> 
     <li>[!UICONTROL 自分に割り当てられた問題のみ ]</li> 
     <li>[!UICONTROL 自分が作成した問題のみ ]</li> 
     <li>[!UICONTROL 私に関する問題のみ ]</li> 
     <li>[!UICONTROL アップデートを購読している問題のみ ]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 状態 ]</td> 
   <td>未完了の問題のみを表示するか、未完了の問題のみを表示するかを選択します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ラベル ]</td> 
   <td>タグを追加します。 モジュールは、このタグの問題を監視します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 監視リポジトリ]

このモジュールは、リポジトリーの作成または変更時にトリガーします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL GitHub] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 返されるリポジトリの最大数 ]</td> 
   <td>結果の最大数を設定 [!DNL Workfront Fusion] は、1 サイクルの間にと連携します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ウォッチ ]</td> 
   <td>新しいリポジトリとすべての変更を監視するか、新しいリポジトリのみを監視するかを選択します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 監視フォーク]

このモジュールは、新しい分岐が作成されたときにトリガーします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL GitHub] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リポジトリ ]</td> 
   <td>分岐を監視するリポジトリを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 返されるフォークの最大数 ]</td> 
   <td>結果の最大数を設定 [!DNL Workfront Fusion] は、1 サイクルの間にと連携します。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL コメントを見る]

このモジュールは、新しいコメントが追加されたり、既存のコメントが変更されたりする際にトリガーします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL GitHub] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リポジトリ ]</td> 
   <td>監視するリポジトリを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 問題番号 ]</td> 
   <td>特定の問題に対して行われた新しいコメントのみを検索して検索を制限する場合は、問題番号を入力します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 返された問題の最大数 ]</td> 
   <td>結果の最大数を設定 [!DNL Workfront Fusion] は、1 サイクルの間にと連携します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ウォッチ ]</td> 
   <td>新しいコメントのみを監視するか、コメントとすべての変更を監視するかを選択します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL プル要求の監視]

このモジュールは、新しいプル要求が追加されたとき、または既存のプル要求が変更されたときにトリガーします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL GitHub] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リポジトリ ]</td> 
   <td>監視するリポジトリを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 返されたプル要求の最大数 ]</td> 
   <td>結果の最大数を設定 [!DNL Workfront Fusion] は、1 サイクルの間にと連携します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 状態 ]</td> 
   <td>[!UICONTROL はプルリクエストのみを開く ]、[!UICONTROL はプルリクエストのみを閉じる ]、またはすべてのプルリクエストを監視するかを選択します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ウォッチ ]</td> 
   <td>新規のプル要求のみを監視するか、新規のプル要求とすべての変更を監視するかを選択します。</td> 
  </tr> 
 </tbody> 
</table>

### アクション

* [[!UICONTROL 問題を検索]](#search-for-an-issue)
* [[!UICONTROL 問題を作成]](#create-an-issue)
* [[!UICONTROL 問題の更新]](#update-an-issue)
* [[!UICONTROL 問題を取得]](#get-an-issue)
* [[!UICONTROL 担当者を追加]](#add-assignees)
* [[!UICONTROL 担当者を削除]](#remove-assignees)
* [[!UICONTROL イシューにラベルを追加する]](#add-labels-to-an-issue)
* [[!UICONTROL 問題からラベルを削除する]](#remove-a-label-from-an-issue)
* [[!UICONTROL コメントの作成]](#create-a-comment)
* [[!UICONTROL コメントをリスト]](#list-comments)

#### [!UICONTROL 問題を検索]

このモジュールでは、検索条件に一致する問題を検索します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL GitHub] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 返された問題の最大数 ]</td> 
   <td>結果の最大数を設定 [!DNL Workfront Fusion] は、1 サイクル（シナリオ実行あたりの繰り返し数）で機能します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 並べ替え基準 ]</td> 
   <td> <p>検索結果の並べ替え方法を選択します。</p> 
    <ul> 
     <li> <p>[!UICONTROL 最適一致 ] </p> </li> 
     <li>[!UICONTROL 作成日 ]</li> 
     <li>[!UICONTROL 更新日 ]</li> 
     <li>[!UICONTROL コメント数 ]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 並べ替え方向 ]</td> 
   <td> <p>昇順または降順を選択します。 </p> <p>日付の場合、選択 <strong>[!UICONTROL 降順 ]</strong> は最も新しい日付を最初に返します。 </p> <p>[!UICONTROL コメント数 ] の場合、選択 <strong>[!UICONTROL 降順 ]</strong> が最も多くのコメントを先に持つ問題を返します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL クエリ ]</td> 
   <td>検索クエリを入力またはマッピングします。 検索オプションについて詳しくは、 <a href="https://docs.github.com/en/github/searching-for-information-on-github/searching-issues-and-pull-requests">問題の検索とプル要求</a> の [!DNL GitHub] ヘルプサイト。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 問題を作成]

このモジュールは、選択したリポジトリに新しいイシューを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL GitHub] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リポジトリ ]</td> 
   <td>イシューを作成するリポジトリを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 担当者 ]</td> 
   <td>問題に割り当てる担当者を選択します。 使用可能な担当者には、リポジトリへの書き込み権限を持つすべてのユーザーと、リポジトリへの読み取り権限を持つ組織のメンバーが含まれます。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL マイルストーン ]</td> 
   <td>新しいイシューに関連付けるマイルストーンを選択します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ラベル ]</td> 
   <td>新しい問題に適用するラベルを選択します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL タイトル ]</td> 
   <td>新しいイシューのタイトルを入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 本文 ]</td> 
   <td>説明や追加情報など、問題の本文を入力またはマッピングする</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 問題の更新]

このモジュールは、既存の [!DNL GitHub] 問題。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL GitHub] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リポジトリ ]</td> 
   <td>イシューを更新するリポジトリを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 担当者 ]</td> 
   <td>問題に割り当てる担当者を選択します。 使用可能な担当者には、リポジトリへの書き込み権限を持つユーザーや、リポジトリへの読み取り権限を持つ組織のメンバーが含まれます。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL マイルストーン ]</td> 
   <td>問題に関連付けるマイルストーンを選択します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ラベル ]</td> 
   <td>問題に適用するラベルを選択します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 数値 ]</td> 
   <td>更新する問題の問題番号を入力またはマッピングします。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 状態 ]</td> 
   <td>問題の更新先の状態を選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL タイトル ]</td> 
   <td>イシューのタイトルを入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 本文 ]</td> 
   <td>説明や追加情報など、問題の本文を入力またはマッピングする</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 問題を取得]

このモジュールは、指定された問題に関する詳細を取得します

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL GitHub] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リポジトリ ]</td> 
   <td>詳細を取得するイシューを含むリポジトリを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 数値 ]</td> 
   <td>詳細を取得する問題の問題番号を入力またはマッピングします。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 担当者を追加]

このモジュールは、指定された問題に割り当て先を追加します

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL GitHub] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リポジトリ ]</td> 
   <td>割り当て先を追加するイシューを含むリポジトリを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 担当者 ]</td> 
   <td>問題に割り当てる担当者を選択します。 使用可能な担当者には、リポジトリへの書き込み権限を持つユーザーや、リポジトリへの読み取り権限を持つ組織のメンバーが含まれます。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 数値 ]</td> 
   <td>担当者を追加する問題の問題番号を入力またはマッピングします。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 担当者を削除]

このモジュールは、指定されたイシューから担当者を削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL GitHub] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リポジトリ ]</td> 
   <td>担当者を削除する問題を含むリポジトリを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 担当者 ]</td> 
   <td>問題から削除する人を選択します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 数値 ]</td> 
   <td>担当者を削除する問題の問題番号を入力またはマッピングします。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL イシューにラベルを追加する]

このモジュールは、問題にラベルを追加します。 ラベルはリポジトリレベルで定義され、リポジトリへの書き込みアクセス権を持つユーザーのみが作成できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL GitHub] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リポジトリ ]</td> 
   <td>ラベルを追加するイシューを含むリポジトリを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ラベル ]</td> 
   <td>イシューに追加するラベルを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 数値 ]</td> 
   <td>ラベルを追加する問題の問題番号を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 問題からラベルを削除する]

このモジュールは、1 つのラベルをイシューから削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL GitHub] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リポジトリ ]</td> 
   <td>ラベルを削除する問題を含むリポジトリを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ラベル ]</td> 
   <td>問題から削除するラベルを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 数値 ]</td> 
   <td>ラベルを削除する問題の問題番号を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL コメントの作成]

このモジュールは、指定された問題に対するコメントを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL GitHub] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リポジトリ ]</td> 
   <td>コメントを作成するイシューを含むリポジトリを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 数値 ]</td> 
   <td>コメントを作成するイシューのイシュー番号を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 本文 ]</td> 
   <td>コメントの内容を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL コメントをリスト]

このモジュールは、指定された問題に関するすべてのコメントを一覧表示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL GitHub] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リポジトリ ]</td> 
   <td>コメントのリストを表示するイシューを含むリポジトリを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 数値 ]</td> 
   <td>コメントのリストを表示するイシューのイシュー番号を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Since]</td> 
   <td>モジュールは、この日付以降に作成されたコメントを返します。 サポートされる日付形式のリストについては、 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">強制入力 [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 返されたコメントの最大数 ]</td> 
   <td>結果の最大数を設定 [!DNL Workfront Fusion] は、1 サイクルの間にと連携します。 </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Troubleshooting</h2>
-->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Module does not receive any events</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">If a module does not receive any events, check the webhook settings in Github and make sure that:</p>
-->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You have set the correct type of event that the chosen module should receive</p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You have entered the correct Payload URL</p>
  -->
