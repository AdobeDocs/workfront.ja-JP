---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: SharePointモジュール
description: 内 [!DNL Adobe Workfront Fusion] シナリオの場合、SharePointを使用するワークフローを自動化し、それを複数のサードパーティのアプリケーションおよびサービスに接続できます。
author: Becky
feature: Workfront Fusion
exl-id: 16d49031-06d2-4c86-bac4-f58cd9b2f1f5
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1951'
ht-degree: 0%

---

# [!DNL SharePoint] モジュール

内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL SharePoint]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。

シナリオの作成手順については、 [でのシナリオの作成 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

モジュールについて詳しくは、 [のモジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

使用する [!DNL SharePoint] モジュールの場合、 [!DNL SharePoint] アカウント

## 接続 [!DNL SharePoint] から [!DNL Workfront Fusion] {#connect-sharepoint-to-workfront-fusion}

* [接続 [!DNL SharePoint] から [!DNL Workfront Fusion] の使用 [!DNL Microsoft] アカウント](#connect-sharepoint-to-workfront-fusion-using-a-microsoft-account)
* [接続 [!DNL SharePoint] から [!DNL Workfront Fusion] 詳細設定の使用](#connect-sharepoint-to-workfront-fusion-using-advanced-settings)

### 接続 [!DNL SharePoint] から [!DNL Workfront Fusion] の使用 [!DNL Microsoft] アカウント

次の項目を使用して、 [!DNL Microsoft] 接続を作成するアカウント [!DNL SharePoint]. 接続方法 [!DNL Sharepoint] アカウント [!DNL Workfront Fusion]を参照してください。 [への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順](../../workfront-fusion/connections/connect-to-fusion-general.md)

### 接続 [!DNL SharePoint] から [!DNL Workfront Fusion] 詳細設定の使用

接続するには [!DNL SharePoint] から [!DNL Workfront Fusion] 無しに [!DNL Microsoft] アカウントに割り当てるには、クライアント ID、クライアント秘密鍵、テナント ID が必要です。

1. クリック **[!UICONTROL 追加]** ～の頂上付近に **[!DNL SharePoint]** 開くボックス **[!UICONTROL 接続の作成]** ボックス

1. （オプション）デフォルトの **[!UICONTROL 接続名]**.
1. クリック **[!UICONTROL 詳細設定を表示]**.
1. 次を入力します。 [!DNL SharePoint] **[!UICONTROL クライアント ID]** および **[!UICONTROL クライアント秘密鍵]**.

1. クリック **[!UICONTROL 続行]**.
1. 表示されるログインウィンドウで、アプリにログインするための資格情報を入力します（まだ入力していない場合）。
1. （条件付き） **[!UICONTROL 許可]** ボタンが表示されたら、ボタンをクリックしてアプリを接続します [!DNL Workfront Fusion].

## [!DNL SharePoint] モジュールとそのフィールド

設定時に [!DNL SharePoint] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL SharePoint] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [アイテム](#item)
* [リスト](#list)
* [ページ（ベータ版）](#page-beta)
* [サイト](#site)
* [その他](#other)

### アイテム

* [[!UICONTROL ウォッチ項目]](#watch-items)
* [[!UICONTROL リスト項目]](#list-items)
* [[!UICONTROL 項目の取得]](#get-an-item)
* [[!UICONTROL 項目の作成]](#create-an-item)
* [[!UICONTROL 項目の更新]](#update-an-item)
* [[!UICONTROL 項目の削除]](#delete-an-item)

#### [!UICONTROL ウォッチ項目]

このトリガーモジュールは、項目が作成または変更されたときにシナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL SharePoint] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">接続 [!DNL SharePoint] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ウォッチリスト ]</td> 
   <td>作成時刻（新しい項目）または変更時刻（更新された項目）のどちらでリストを監視するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL サイトとリスト ID を入力 ]</td> 
   <td> <p>監視するサイトとリストを識別する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 手動で入力 ]</strong> </p> <p>を入力またはマッピングします。 <strong>[!UICONTROL サイト ID]</strong> および <strong>[!UICONTROL リスト ID]</strong> 表示されるフィールド内で、</p> </li> 
     <li> <p><strong>[!UICONTROL フォローしているリストから選択 ]</strong> </p> <p>監視するサイトを選択し、リストを選択します。 これらのドロップダウンは、後続のサイトのみを取得します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td> <p>各シナリオの実行サイクル中にモジュールが返す最大項目数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL リスト項目]

このアクションモジュールは、指定されたリスト内のすべての項目のリストを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL SharePoint] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">接続 [!DNL SharePoint] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リスト項目 ]</td> 
   <td> <p>項目を取得するリストを識別する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 手動で入力 ]</strong> </p> <p>を入力またはマッピングします。 <strong>[!UICONTROL サイト ID]</strong> および <strong>[!UICONTROL リスト ID]</strong> 表示されるフィールド内で、</p> </li> 
     <li> <p><strong>[!UICONTROL リストから選択 ]</strong> </p> <p>項目の取得元のリストが含まれるサイトを選択し、リストを選択します。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td> <p>各シナリオの実行サイクル中にモジュールが返す最大項目数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 項目の取得]

このアクションモジュールは、指定された項目のデータを返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL SharePoint] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">接続 [!DNL SharePoint] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 項目の取得 ]</td> 
   <td> <p>取得する項目を含むサイトとリストを識別する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 手動で入力 ]</strong> </p> <p>を入力またはマッピングします。 <strong>[!UICONTROL サイト ID]</strong>, <strong>[!UICONTROL リスト ID]</strong>、および <strong>[!UICONTROL Item ID]</strong> 表示されるフィールド内で、</p> </li> 
     <li> <p><strong>[!UICONTROL リストから選択 ]</strong> </p> <p>項目の取得元のリストが含まれるサイトを選択し、リストを選択して、項目を選択します。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 項目の作成]

このアクションモジュールは、SharePointリストに新しい項目を作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL SharePoint] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">接続 [!DNL SharePoint] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 項目の作成 ]</td> 
   <td> <p>サイトを識別する方法を選択し、項目を作成する場所をリストします。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 手動で入力 ]</strong> </p> <p>を入力またはマッピングします。 <strong>[!UICONTROL サイト ID]</strong> および <strong>[!UICONTROL リスト ID]</strong> 表示されるフィールド内で、</p> </li> 
     <li> <p><strong>[!UICONTROL リストから選択 ]</strong> </p> <p>項目を作成するリストが含まれるサイトを選択し、リストを選択します。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フィールド ]</td> 
   <td>新しい項目に設定する各フィールドに対して、フィールドのキー（フィールドを識別する）と、新しい項目にそのフィールドに設定する値を入力します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 項目の更新]

このアクションモジュールは、SharePointリスト内の既存の項目を更新します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL SharePoint] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">接続 [!DNL SharePoint] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 項目の更新 ]</td> 
   <td> <p>更新する項目を含むサイトとリストを識別する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 手動で入力 ]</strong> </p> <p>を入力またはマッピングします。 <strong>[!UICONTROL サイト ID]</strong>, <strong>[!UICONTROL リスト ID]</strong>、および <strong>[!UICONTROL Item ID]</strong> 表示されるフィールド内で、</p> </li> 
     <li> <p><strong>[!UICONTROL リストから選択 ]</strong> </p> <p>更新する項目が含まれるサイトを選択し、リストを選択して、項目を選択します。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フィールド ]</td> 
   <td>新しい項目に対して更新する各フィールドに対して、フィールドのキー（フィールドを識別する）と、そのフィールドに対して項目に含める新しい値を入力します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 項目の削除]

このアクションモジュールは、SharePointリスト内の既存の項目を削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL SharePoint] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">接続 [!DNL SharePoint] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 項目の更新 ]</td> 
   <td> <p>削除する項目を含むサイトとリストを識別する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 手動で入力 ]</strong> </p> <p>を入力またはマッピングします。 <strong>[!UICONTROL サイト ID]</strong>, <strong>[!UICONTROL リスト ID]</strong>、および <strong>[!UICONTROL Item ID]</strong> 表示されるフィールド内で、</p> </li> 
     <li> <p><strong>[!UICONTROL リストから選択 ]</strong> </p> <p>削除する項目が含まれるサイトを選択し、リストを選択して、項目を選択します。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### リスト

* [[!UICONTROL ウォッチリスト]](#watch-lists)
* [[!UICONTROL リストリスト]](#list-lists)
* [[!UICONTROL リストを取得]](#get-a-list)
* [[!UICONTROL リストの作成]](#create-a-list)

#### [!UICONTROL ウォッチリスト]

このトリガーモジュールは、リストの作成または変更時にシナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL SharePoint] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">接続 [!DNL SharePoint] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ウォッチリスト ]</td> 
   <td>作成時刻（新しい項目）または変更時刻（更新された項目）のどちらでリストを監視するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL サイトとリスト ID を入力 ]</td> 
   <td> <p>監視するサイトとリストを識別する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 手動で入力 ]</strong> </p> <p>を入力またはマッピングします。 <strong>[!UICONTROL サイト ID]</strong> 監視するリストがある場所。</p> </li> 
     <li> <p><strong>[!UICONTROL フォローしているリストから選択 ]</strong> </p> <p>監視するサイトを選択します。 ドロップダウンは、ユーザーがフォローしているサイトのみを取得します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td> <p>各シナリオの実行サイクル中にモジュールが返す最大リスト数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL リストリスト]

このアクションモジュールは、指定されたリスト内のすべての項目のリストを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL SharePoint] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">接続 [!DNL SharePoint] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リスト ]</td> 
   <td> <p>リストを取得するサイトを識別する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 手動で入力 ]</strong> </p> <p>を入力またはマッピングします。 <strong>[!UICONTROL サイト ID]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL リストから選択 ]</strong> </p> <p>取得するリストが含まれているサイトを選択します。 ドロップダウンは、従うサイトのみを取得します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td> <p>各シナリオの実行サイクル中にモジュールが返す最大リスト数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL リストを取得]

このアクションモジュールは、指定されたリストのデータを返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL SharePoint] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">接続 [!DNL SharePoint] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リストの取得 ]</td> 
   <td> <p>取得する項目を含むサイトとリストを識別する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 手動で入力 ]</strong> </p> <p>を入力またはマッピングします。 <strong>[!UICONTROL サイト ID]</strong> および <strong>リスト ID</strong> 表示されるフィールド内で、</p> </li> 
     <li> <p><strong>[!UICONTROL リストから選択 ]</strong> </p> <p>取得するリストが含まれるサイトを選択し、リストを選択します。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL リストの作成]

このアクションモジュールは、SharePointに新しいリストを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL SharePoint] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">接続 [!DNL SharePoint] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL サイト ID を入力 ]</td> 
   <td> <p>サイトを識別する方法を選択し、リストを作成する場所をリストします。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 手動で入力 ]</strong> </p> <p>を入力またはマッピングします。 <strong>[!UICONTROL サイト ID]</strong> リストを作成する場所です。</p> </li> 
     <li> <p><strong>[!UICONTROL リストから選択 ]</strong> </p> <p>リストを作成するサイトを選択します。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 表示名 ]</td> 
   <td>新しいリストの名前を入力またはマップします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 説明 ]</td> 
   <td>新しいリストの説明を入力またはマップします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 列を追加 ]</td> 
   <td>新しいリストに設定する各列に対して、 <strong>[!UICONTROL 名前 ]</strong> を選択し、 <strong>[!UICONTROL の種類 ]</strong> の値を指定します。</td> 
  </tr> 
 </tbody> 
</table>

### ページ（ベータ版）

>[!NOTE]
>
>の API `beta` バージョン [!DNL Microsoft Graph] は変更される場合があります。 実稼動アプリケーションでのこれらの API の使用はサポートされていません。

#### [!UICONTROL ページの取得]

このアクションモジュールは、指定されたページのデータを返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL SharePoint] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">接続 [!DNL SharePoint] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ページの取得 ]</td> 
   <td> <p>取得するページを識別する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 手動で入力 ]</strong> </p> <p>を入力またはマッピングします。 <strong>[!UICONTROL サイト ID]</strong>および <strong>[!UICONTROL Page ID]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL リストから選択 ]</strong> </p> <p>取得するページを含むサイトを選択し、ページを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### サイト

* [[!UICONTROL サイトを検索]](#search-sites)
* [[!UICONTROL サイトの取得]](#get-a-site)

#### [!UICONTROL サイトを検索]

このアクションモジュールは、指定したパラメーターでサイトを検索します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL SharePoint] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">接続 [!DNL SharePoint] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 表示名のキーワード ]</td> 
   <td> <p>サイトを検索する検索語句を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すサイトの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL サイトの取得]

このアクションモジュールは、指定されたサイトのデータを返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL SharePoint] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">接続 [!DNL SharePoint] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL サイトの取得 ]</td> 
   <td> <p>取得するページを識別する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 手動で入力 ]</strong> </p> <p>を入力またはマッピングします。 <strong>[!UICONTROL サイト ID]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL リストから選択 ]</strong> </p> <p>取得するサイトを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### その他

#### [!UICONTROL API 呼び出しを実行する]

このモジュールでは、カスタム API 呼び出しを実行できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL SharePoint] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">接続 [!DNL SharePoint] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>相対パスを入力 <code>https://graph.microsoft.com</code>. 例:<code> /beta/sites</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL メソッド ]</p> </td> 
   td&gt; <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。例： <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] によって、認証ヘッダーが追加されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL クエリ文字列 ]</td> 
   <td> <p> 標準の JSON オブジェクトの形式で、API 呼び出しのクエリを追加します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL の種類 ]</td> 
   <td>API 呼び出しで送信するデータのタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 本文 ]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文のコンテンツを追加します。</p> <p>メモ:  <p>条件文 ( <code>if</code> JSON で、条件文の外側に引用符を置きます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

