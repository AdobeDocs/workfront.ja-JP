---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: ある環境から別の環境へのオブジェクトの移動
description: 環境プロモーション機能は、設定関連のオブジェクトを環境間で移動する機能を提供することを目的としています。 トランザクションオブジェクトを移動する機能はサポートしていません（例外は制限されています）。
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
source-git-commit: f886c67c80439e2e8158c4616479ffabaa53c3d3
workflow-type: tm+mt
source-wordcount: '2334'
ht-degree: 2%

---

# 1 つからのオブジェクトの移動 [!DNL Workfront] 別の環境

<!-- 
TO DO

Overview of value
Check for any code changes
Fix {}
Add to tocs
-->

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] 計画</td> 
   <td> <p>Enterprise、Prime または Ultimate</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!DNL Workfront] ライセンス</p> </td> 
   <td> <p>[!UICONTROL プラン ] </p> <p>次の条件を満たす必要があります。 [!DNL Workfront] 管理者。 詳しくは、 [!DNL Workfront] 管理者向け： <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">オブジェクトの権限</p> </td> 
   <td> <p>すべて</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">サポートパッケージ</td> 
   <td> <p>[!UICONTROL Plus]、[!UICONTROL Preferred]、または [!UICONTROL Enterprise]</p> <p>標準サポートパッケージは、カスタム更新サンドボックスにアクセスできませんが、プレビューサンドボックスにアクセスできます。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 前提条件

プロモーションパッケージを作成エンドポイントは、既にソース環境が設定されていることを前提としています。 この API 呼び出しでは、 [!DNL Workfront] objCodes とオブジェクトの GUID。 このマップの具体的な構造を以下に示します。

## 環境の昇格でサポートされるオブジェクト

環境プロモーション機能は、設定関連のオブジェクトを環境間で移動する機能を提供することを目的としています。 トランザクションオブジェクトを移動する機能はサポートしていません（例外は制限されています）。

* [作業オブジェクト](#work-objects)
* [レポートオブジェクト](#reporting-objects)
* [カスタムデータオブジェクト](#custom-data-objects)
* [組織オブジェクト](#organization-objects)
* [その他の設定オブジェクト](#other-configuration-objects)


### 作業オブジェクト

| 昇格可能なオブジェクト | 含まれるプロモート可能なサブオブジェクト |
| --- | --- |
| プロジェクト (PROJ) | プロジェクト<br>タスク<br>割り当て<br>前任者<br>会社情報<br>上書き率<br>グループ化<br>役割<br>チーム<br>承認プロセス<br>承認パス<br>承認ステップ<br>ステップ承認者<br>スケジュール<br>非稼働日<br>キューの定義<br>トピックグループをキュー<br>トピックをキュー<br>ルーティングルール<br>マイルストーンのパス<br>マイルストーン<br>時間タイプ<br>リソースプール<br>カテゴリ<br>カテゴリパラメーター<br>パラメーター<br>パラメータグループ<br>パラメーターオプション<br>カテゴリの表示ロジック |
| テンプレート (TMPL) | テンプレート<br>テンプレートタスク<br>テンプレートタスクの割り当て<br>テンプレートタスクの先行タスク<br>会社情報<br>上書き率<br>グループ化<br>役割<br>チーム<br>承認プロセス<br>承認パス<br>承認ステップ<br>ステップ承認者<br>スケジュール<br>非稼働日<br>キューの定義<br>トピックグループをキュー<br>トピックをキュー<br>ルーティングルール<br>マイルストーンのパス<br>マイルストーン<br>時間タイプ<br>リソースプール<br>カテゴリ<br>カテゴリパラメーター<br>パラメーター<br>パラメータグループ<br>パラメーターオプション<br>カテゴリの表示ロジック |

### レポートオブジェクト

| 昇格可能なオブジェクト | 含まれるプロモート可能なサブオブジェクト |
| --- | --- |
| レイアウトテンプレート (UITMPL) | レイアウトテンプレート<br>ダッシュボード<br>カレンダー<br>カレンダーセクション<br>外部ページ<br>レポート<br>フィルター<br>グループ化<br>表示<br>パラメーター |
| ダッシュボード (PTLTAB) | ダッシュボード<br>カレンダー<br>カレンダーセクション<br>外部ページ<br>レポート<br>フィルター<br>グループ化<br>表示<br>パラメーター |
| カレンダー (CALEND) | カレンダー<br>カレンダーセクション |
| 外部ページ (EXTSEC) | 外部ページ |
| レポート (PTLSEC) | レポート<br>フィルター<br>グループ化<br>表示<br>パラメーター |
| フィルター (UIFT) | フィルター<br>パラメーター |
| グループ化 (UIGB) | グループ化<br>パラメーター |
| 表示 (UIVW) | 表示<br>パラメーター |

### カスタムデータオブジェクト

| 昇格可能なオブジェクト | 含まれるプロモート可能なサブオブジェクト |
| --- | --- |
| カテゴリ (CTGY) | カテゴリ<br>カテゴリパラメーター<br>パラメーター<br>パラメータグループ<br>パラメーターオプション<br>カテゴリの表示ロジック<br>グループ化 |
| パラメータ (PARAM) | パラメーター<br>パラメーターオプション |
| パラメータグループ (PGRP) | パラメーター グループ |

### 組織オブジェクト

| 昇格可能なオブジェクト | 含まれるプロモート可能なサブオブジェクト |
| --- | --- |
| グループ (GROUP) | グループ化 <br>サブグループ（最大 5 レベル）<br>カテゴリ<br>カテゴリパラメーター<br>パラメーター<br>パラメータグループ<br>パラメーターオプション<br>カテゴリの表示ロジック |
| 役割（役割） | 役割 |
| チーム（チーム） | チーム<br>グループ化 |
| 会社 (CMPY) | 会社情報<br>上書き率<br>カテゴリ<br>カテゴリパラメーター<br>パラメーター<br>パラメータグループ<br>パラメーター <br>カテゴリの表示ロジック<br>グループ化 |
| Portfolio（ポート） | Portfolio<br>プログラム<br>グループ化<br>カテゴリ<br>カテゴリパラメーター<br>パラメーター<br>パラメータグループ<br>パラメーターオプション<br>カテゴリの表示ロジック |
| プログラム (PRGM) | プログラム<br>Portfolio<br>グループ化<br>カテゴリ<br>カテゴリパラメーター<br>パラメーター<br>パラメータグループ<br>パラメーターオプション<br>カテゴリの表示ロジック |

### その他の設定オブジェクト

| 昇格可能なオブジェクト | 含まれるプロモート可能なサブオブジェクト |
| --- | --- |
| 承認プロセス (ARVPRC) | 承認プロセス<br>承認パス<br>承認ステップ<br>ステップ承認者<br>役割<br>チーム<br>グループ化 |
| スケジュール (SCHED) | スケジュール<br>非稼働日<br>グループ化 |
| マイルストーンパス (MPATH) | マイルストーンのパス<br>マイルストーン |
| タイムシートプロファイル (TSPRO) | タイムシートプロファイル<br>時間タイプ |
| 時間のタイプ (HOURT) | 時間タイプ |
| 費用タイプ (EXPTYP) | 費用タイプ |
| リスクタイプ (RSKTYP) | 危険タイプ |
| リソースプール (RSPL) | リソース プール |

## 認証

API は、リクエストごとに認証をおこない、リクエストされたオブジェクトを表示または変更するためのアクセス権をクライアントが持つようにします。

認証は、セッション ID または API キーを渡すことで実行されます。このキーは、次の方法で指定できます。

### リクエストヘッダー認証

推奨される認証方法は、セッショントークンを含む SessionID という名前のリクエストヘッダーを渡すことです。 これは安全に対して有利である [クロスサイトリクエストフォージェリ (CSRF)](http://en.wikipedia.org/wiki/Cross-site_request_forgery) 攻撃を受け、キャッシュ目的で URI に干渉しない。

リクエストヘッダーの例を次に示します。

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

## API エンドポイント

* [パッケージの作成](#create-a-package)
* [パッケージのリストの取得](#get-a-list-of-packages)
* [ID によるパッケージの取得](#get-a-package-by-id)
* [パッケージの設定定義の取得](#get-a-packages-configuration-definition)
* [パッケージの詳細と定義を置き換える](#replace-package-details-and-definition)
* [パッケージの特定のプロパティを更新する](#update-specific-properties-of-a-package)
* [パッケージの削除](#delete-a-package)
* [事前実行の実行](#execute-a-pre-run)
* [インストールの実行](#execute-an-installation)
* [特定のパッケージのインストールのリストを取得する](#get-a-list-of-installations-for-a-specific-package)
* [インストールの詳細を取得する](#get-the-installation-details-for-an-installation)

### パッケージの作成

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /packages</code></td> 
  </tr> 
  </tbody> 
</table>

この呼び出しは、複数手順のプロセスを実行します。

最初のステップでは、「ASSEMBLING」ステータスで空のプロモーションパッケージが作成されます。

2 つ目の手順では、 `objectCollections` Workfrontから要求されたレコードをPOSTするためにアセンブリ本文で提供される配列。 リクエストされたレコードの数とWorkfrontの設定によっては、この手順の完了に数分かかる場合があります。 このプロセスの最後に、空のプロモーションパッケージが `packageEntities` ステータスは自動的に「ドラフト」に設定されます。


>[!NOTE]
>
>の構造をメモしておきます。 `objectCollections`  配列。
>
>配列内の各項目には、 `objCode` Workfront API Explorer で記述されたオブジェクトコードに対応するキー。
>
>各項目には、 `entities` コレクション。 これは、 `ID` および `name` 存在するキー。
>
>リクエストできるオブジェクトコードのリスト ( `objectCollections` リスト、「 [環境の昇格でサポートされるオブジェクト](#supported-objects-for-environment-promotion) 」の節を参照してください。

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages
```

#### ヘッダー

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

または

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### 本文

```json
{
    "packageName": "Agency Onboarding - 2023-06-06",
    "description": "This promotion package contains configuration to support the agency onboarding processes...",
    "source": "https://{domain}.{environment}.workfront.com",
    "objectCollections": [
        {
            "objCode": "PROJ",
            "entities": [
                {
                    "ID": "6419b8b9001151ee258921a4f7597ba1",
                    "name": "Agency Request"
                }
            ]
        },
        {
            "objCode": "TMPL",
            "entities": [
                {
                    "ID": "6419b8b9001151ee258921a4f7597bb2",
                    "name": "New Agency Onboarding"
                },
                {
                    "ID": "6419b8b9001151ee258921a4f7597bc3",
                    "name": "New Agency Offboarding"
                }
            ]
        },
        {
            "objCode": "PTLTAB",
            "entities": [
                {
                    "ID": "645e6435000b4aaebe4776f4a42ed5ad",
                    "name": "Agency Performance and Readiness"
                }
            ]
        }
    ]
}
```

#### 応答

```json
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "status": "ASSEMBLING",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d"
}
```

### パッケージのリストの取得

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages</code></td> 
  </tr> 
  </tbody> 
</table>

この呼び出しは、顧客に属するプロモーションパッケージのフィルターされていないリストを返します。

応答には、お客様のサンドボックス、プレビューまたはWorkfrontの実稼動インスタンスのいずれかから作成されたすべてのパッケージが含まれます。

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages
```

#### ヘッダー

```json
{
    "apikey": "**********"
}
```

または

```json
{
    "sessionID": "*****************"
}
```

#### 本文

_空_

#### 応答

```
200
```

```json
{
    "data": [
        {
            "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
            "name": "Agency Onboarding - 2023-06-06",
            "description": "This promotion package contains configuration to support the agency onboarding processes...",
            "status": "ASSEMBLING",
            "version": 1,
            "installationCounts": {},
            "createdAt": "2023-06-06T17:29:21.600Z",
            "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
            "publishedAt": null,
            "customerId": "61aa9d090005fa42152c1cb66659f38d"
        },
        {...}
    ]
}
```

### ID によるパッケージの取得

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

この呼び出しは、リクエストされたプロモーションパッケージの詳細を返します。

リクエストは、プロモーションパッケージの元のソースに関係なく、任意の環境を通じておこなうことができます。

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### ヘッダー

```json
{
    "apikey": "**********"
}
```

または

```json
{
    "sessionID": "*****************"
}
```

#### 本文

_空_

#### 応答

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "status": "DRAFT",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "displayEntities": {
            "GROUP": [
               {
                   "id": "52aa9d0e0005fcee8f212835bdaa2691",
                   "name": "Default Group",
                   "description": "null"
                   - or -
                   "description": "..."
               }
            ],
            "ROLE": [
               {...}
            ],
            ...
        }
   }
}
```

### パッケージの設定定義の取得

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages/{id}/definition</code></td> 
  </tr> 
  </tbody> 
</table>

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}/definition
```

#### ヘッダー

```json
{
    "apikey": "**********"
}
```

または

```json
{
    "sessionID": "*****************"
}
```

#### 本文

_空_

#### 応答

```
200
```

```json
{
    "packageEntities": {
        "GROUP": [
           {
               "id": "52aa9d0e0005fcee8f212835bdaa2691",
               "name": "Default Group",
               "businessLeaderID": "...",
               "categoryID": "...",
               "defaultInterface": 1,
               "description": "...",
               "extRefID": null,
               "isActive": true,
               "isGroupPublic": true,
               "isPublic": true,
               "parentID": null,
               "rootID": null,
               "rootName": null,
               "uiTemplateID": null
           }
        ],
        "ROLE": [
           {...}
        ],
        ...
    }
}
```

### パッケージの詳細と定義を置き換える

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>PUT /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

この呼び出しは、プロモーションパッケージのすべてのコンテンツを置き換えます。

リクエストでは、すべての編集可能なフィールドが提供される必要があります。

編集可能な属性は次のとおりです。

1. name（文字列）
1. description （文字列）
1. ソース（URL 検証を含む文字列）
1. status （値の検証を含む文字列）
1. バージョン（整数）
1. packageEntities （コレクション）

ステータスのオプションは次のとおりです。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>組み立て</td> 
   <td><p>このステータスは、オブジェクトのアセンブリ中に自動的に割り当てられます。</p><p>このステータスは、顧客が直接設定することはできません。</p></td> 
  </tr> 
  <tr> 
   <td>ドラフト</td> 
   <td><p>このステータスは、アセンブリプロセスの終了時、または空のプロモーションパッケージの作成時に割り当てられます。</p><p>顧客は、プロモーションパッケージをこのステータスに戻すことができます。</p><p>このステータスの場合、どの環境にもプロモーションパッケージをインストールすることはできません。</p></td> 
  </tr> 
  <tr> 
   <td>テスト</td> 
   <td><p>このステータスにより、任意のプレビューまたはカスタム更新サンドボックスにプロモーションパッケージをインストールできます。 このステータスの場合、パッケージを実稼動環境にインストールすることはできません。</p></td> 
  </tr> 
  <tr> 
   <td>アクティブ</td> 
   <td><p>このステータスにより、プロモーションパッケージを実稼動環境を含む任意の環境にインストールできます。</p><p>パッケージのステータスがアクティブに設定されている場合、 <code>publishedAt</code> 日付は、リクエストの現在のタイムスタンプに自動的に設定されます。</p></td> 
  </tr> 
  <tr> 
   <td>無効</td> 
   <td><p>このステータスは、以前使用したプロモーションパッケージを非表示にするために使用されます。このパッケージは、今後どの環境にもインストールされなくなります。</p><p>このステータスのパッケージは、どの環境にもインストールできません。</p><p>パッケージのステータスが DISABLED に設定されている場合、 <code>retiredAt</code> 日付は、リクエストの現在のタイムスタンプに自動的に設定されます。</p><p>このステータスの使用は、<code>DELETE /package</code> エンドポイントを設定する必要があります。このパッケージを使用して作成されたデプロイメントでは、このエンドポイントが取得可能で、インストール履歴が保持されるからです。</p></td> 
  </tr> 
  <tr> 
   <td>ASSEMBLING_FAILED</td> 
   <td><p>ASSEMBLING ステージに障害が発生すると、プロモーションパッケージは自動的にこのステータスに入ります。</p><p>パッケージを ASSEMBLING ステージに戻すには、抽出プロセスを再びトリガーする必要があります。</p></td> 
  </tr> 
  </tbody> 
</table>

#### URL

```
PUT https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### ヘッダー

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### 本文

```json
{
    "packageName": "Agency Onboarding - 2023-06-06",
    "description": "This promotion package contains configuration to support the agency onboarding processes... with a description change",
    "source": "https://{domain}.{environment}.workfront.com",
    "status": "TESTING",
    "version": 1,
    "metadata": {
        "displayOrder": ["GROUP","ROLE","TMPL","PROJ","PTLTAB"],
        "historyOrder": ["GROUP","ROLE","TMPL","TTSK","PROJ","PTLTAB"], 
        "installOrder": ["GROUP","ROLE","TMPL","TTSK","TPRED","TASSGN","PROJ","QUED","RRUL","QUET","UIFT","UIGB","UIVW","PTLTAB"], 
        "summaryOrder": ["GROUP","ROLE","TMPL"], 
        "shapeVersion": 2
    },
    "packageEntities": {
        "GROUP": [
           {
               "id": "52aa9d0e0005fcee8f212835bdaa2691",
               "name": "Default Group",
               "businessLeaderID": "...",
               "categoryID": "...",
               "defaultInterface": 1,
               "description": "...",
               "extRefID": null,
               "isActive": true,
               "isGroupPublic": true,
               "isPublic": true,
               "parentID": null,
               "rootID": null,
               "rootName": null,
               "uiTemplateID": null
           }
        ],
        "ROLE": [
           {...}
        ],
        ...
    }
}
```

#### 応答

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "status": "TESTING",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "displayEntities": {
            "GROUP": [
               {
                   "id": "52aa9d0e0005fcee8f212835bdaa2691",
                   "name": "Default Group",
                   "description": "..."
               }
            ],
            "ROLE": [
               {...}
            ],
            ...
        }
   }
}
```

### パッケージの特定のプロパティを更新する

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>PATCH /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

この呼び出しは、PATCH本文に提供されているプロモーションパッケージのコンテンツをすべて更新します。

編集可能な属性は次のとおりです。

1. name（文字列）
1. description （文字列）
1. ソース（URL 検証を含む文字列）
1. status （値の検証を含む文字列）
1. バージョン（整数）
1. packageEntities （コレクション）

   または

   objectCollections （配列）

次の項目を指定： `packageEntities` 指定された設定定義でプロモーションパッケージが更新されます。

次の項目を指定： `objectCollections` により、 `source` 環境がプロモーションパッケージに関連付けられています。 The `source` フィールドは、 `objectCollections` が指定されている。

#### URL

```
PATCH https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```


#### ヘッダー

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

または

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### 本文

```json
{
    "status": "ACTIVE"
}
```

#### 応答

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "status": "ACTIVE",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": "2023-06-06T19:39:01.600Z",
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "displayEntities": {
            "GROUP": [
               {
                   "id": "52aa9d0e0005fcee8f212835bdaa2691",
                   "name": "Default Group",
                   "description": "..."
               }
            ],
            "ROLE": [
               {...}
            ],
            ...
        }
   }
}
```

### パッケージの削除

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>DELETE /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

この呼び出しにより、プロモーションパッケージレコードが削除されます。 この操作は元に戻せません。

>[!NOTE]
>
>プロモーションパッケージを削除する場合とは異なり、パッケージのステータスを「無効」に変更することをお勧めします。 これにより、パッケージを取得し、パッケージがデプロイされた場所のインストール履歴を保持できます。

#### URL

```
DELETE https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### ヘッダー

```json
{
    "apikey": "**********"
}
```

または

```json
{
    "sessionID": "*****************"
}
```

#### 本文

_空_

#### 応答

```
200
```

```
Deleted
```

### 事前実行の実行

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST  {customer-domain}/environment-promotion/api/v1/packages/{id}/prepare-installation</code></td> 
  </tr> 
  </tbody> 
</table>

この呼び出しは、URL で識別されるターゲット環境とパッケージ定義の比較を実行します。

結果は、ターゲット環境でプロモーションオブジェクトが見つかったかどうかを識別する JSON 本文になります。

各プロモーションオブジェクトに対して、次のいずれかを実行します。 `actions`  が設定されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>作成</td> 
   <td><p>対応するレコードがターゲット環境で見つからない場合、アクションは CREATE に設定されます。</p><p>このアクションが <code>translationmap</code> が <code>/install</code> endpoint。インストールサービスはレコードを作成します。</p></td> 
  </tr> 
  <tr> 
   <td>既存を使用</td> 
   <td><p>対応するレコードがターゲット環境で見つかった場合、アクションは USEEXISTING に設定され、 <code>targetId</code> は、 <code>translationmap</code>.</p><p>このアクションが <code>translationmap</code> が <code>/install</code> エンドポイントの場合、インストールサービスはレコードを作成しません。 ただし、 <code>targetId</code> このレコードへの参照を持つ他のオブジェクトのマップエントリに含まれます。</p><p>例えば、パッケージのデプロイ先のターゲット環境に「デフォルトグループ」が存在する場合があります。 2 つの「Default Group」レコードを持つことはできないので、インストールサービスは、プロジェクト、フォーム、このグループに関連する他のエンティティなど、「Default Group」への参照を含む他のオブジェクト作成アクションで、既存のグループの GUID を使用します。</p><p><b>メモ:</b> <ul><li><p>USEEXISTING アクションが割り当てられると、ターゲット環境の既存のレコードは変更されません。 </p><p>例えば、パッケージの構築元のサンドボックスで「デフォルトグループ」の説明が変更され、ターゲット環境で説明の値が異なる場合、このを使用したインストール後も、値は変更されません <code>translationmap</code>.</li></ul></td> 
  </tr> 
  <tr> 
   <td>無視</td> 
   <td><p>このアクションは自動的には設定されません。</p><p>割り当てられた CREATE または USEEXISTING アクションを手動で上書きしてから、 <code>/install</code> を呼び出します。</p><p><b>メモ: </b><ul><li><p>最初に CREATE に設定されたレコードが IGNORE に設定されている場合は、すべての子レコードも IGNORE に設定する必要があります。</p><p>例えば、テンプレートレコードが CREATE アクションにマッピングされ、インストールユーザーがそのレコードをデプロイメントから除外する場合、テンプレートのアクションを IGNORE に設定できます。</p><p>この場合、インストールユーザーがテンプレートタスク、テンプレートタスクの割り当て、テンプレートタスクの先行タスク、キュー定義、キュートピック、ルーティングルールなどを IGNORE に設定しないと、展開は失敗します。</p></li><li><p>最初に USEEXISTING に設定されたレコードが IGNORE に設定されている場合は、インストールプロセス中に何らかの悪影響が出る場合があります。</p><p>たとえば、グループレコードが USEEXISTING アクションにマッピングされ、インストールユーザーがグループを必要とするオブジェクト（グループが割り当てられていないプロジェクトは存在できない）のアクションを IGNORE に変更した場合、システムの既定のグループがそのプロジェクトに割り当てられます。</p></li><li><p>元々 USEEXISTING に設定されていたレコードが CREATE に設定されている場合、Workfrontエンティティの多くは一意の名前の制約を持つので、インストールプロセス中に悪影響が出る場合があります。</p><p>例えば、「Default Group」レコードが USEEXISTING アクションにマッピングされ、インストールユーザーがアクションを CREATE に変更した場合、「Default Group」が既に存在するので、インストールはすべての手順を完了できません。 グループ名は一意である必要があります。</p><p>一部のエンティティには、一意の名前の制約がありません。 これらのオブジェクトの場合、この変更を行うと、同じ名前の 2 つのレコードが作成されます。 例えば、テンプレート、プロジェクト、ビュー、フィルター、グループ、レポート、ダッシュボードには、一意の名前制約は必要ありません。 これらのレコードに一意の名前を付けることをお勧めしますが、適用されません。</p></li></ul></p></td> 
  </tr> 
  </tbody> 
</table>

現在、UPDATE はサポートされていません。 `action` （このサービスのアルファ機能）。 更新を許可するオプション `action` 我々が研究しているものです

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/translationmap
```

#### ヘッダー

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

または

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### 本文

```json
{}
```

#### 応答

```
200
```

```json
{}
```

### インストールの実行

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /install</code></td> 
  </tr> 
  </tbody> 
</table>

この呼び出しにより、POSTURL で識別されるターゲット環境へのプロモーションパッケージのインストールが開始されます。

#### オプション

次の場合、 `translationmap` がPOST本文に指定されていない場合、プロセスは自動的に `/translationmap` を呼び出します。 The `translationmap` 返されるはそのまま使用され、レビューや調整をおこなう機会はありません。

次の場合、 `translationmap` がPOST本文に指定されている場合、インストールプロセスは提供されたマッピングを使用します。 これにより、インストールユーザーは、インストールを実行する前に、必要に応じて確認し、調整を行うことができます。

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/install
```

#### ヘッダー

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

または

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### 本文

```json
{
}
```

#### 応答

```
200
```


```json
{}
```

### 特定のパッケージのインストールのリストを取得する

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /v1/installations?environmentPromotionPackageId={environmentPromotionPackageId}
</code></td> 
  </tr> 
  </tbody> 
</table>

結果には、パッケージがデプロイされたすべての環境のインストールイベントが含まれます。 リクエストがおこなわれる環境のインストールに限定されるわけではありません。 これにより、このパッケージを受け取った環境を識別できます。

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1v1/installations?environmentPromotionPackageId={environmentPromotionPackageId}
```

#### ヘッダー

```json
{
    "apikey": "**********"
}
```

または

```json
{
    "sessionID": "*****************"
}
```

#### 本文

_空_

#### 応答

```
200
```

```json
[
    {
        "id": "2892b936-e09e-455a-935f-e1462ab9753c",
        "environmentPromotionPackageId": "4fae2b9d-d315-45f4-909f-a0c0d79fc65d",
        "environmentPromotionPackageVersion": 1,
        "userId": "8fbbc5bcf4f94a5b862483ee05573e73",
        "customerId": "54286d78b064451096752b99bf968481",
        "status": "COMPLETED",
        "environment": "https://{domain}.{environment}.workfront.com",
        "registeredAt": "2021-03-16T02:21:31.908Z",
        "updatedAt": null,
        "translationMap": {
            "ROLE": {
                "5f6d114f006883209828ddd9088e63b3": {
                    "name": "DAM Curator",
                    "action": "USEEXISTING",
                    "isValid": true,
                    "targetId": "600f4bed00028a718599f29575840053"
                },
                "ad535a9ebe647361e053a7656a0a1575": {
                    "name": "Copywriter",
                    "action": "USEEXISTING",
                    "isValid": true,
                    "targetId": "600f162700001ca051081c06667b14a4"
                },
                ...
            },
            "TMPL": {
                "5f9b317c00b3db5af69abcd1ed5f82aa": {
                    "name": "Digital Asset Production (Integrated)",
                    "action": "CREATE",
                    "isValid": true,
                    "targetId": "6054cda40000d5af63dc811d9c2b3a07"
                },
                ...
            },
            ...
        }
    },
    {...}
]
```

### インストールの詳細を取得する

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /installations/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

この呼び出しは、 `translationMap` 特定のインストール用にインストールサービスによって生成されます。

各レコードには、所定の `action` そしてその行動が成功したかどうかだった

CREATE を含むレコードの場合 `action` の `targetId` フィールドは、ターゲットシステムで新しく作成されたレコードの値で設定されます。 また、 `installationStatus` フィールドが INSTALLED に設定されます。

USEEXISTING を含むレコードの場合 `action` の `targetId` フィールドも設定され、 `installationStatus` フィールドが REGISTERED に設定されます。 これは、マッピングプロセスが完了し、インストールサービスがレコードを評価し、何も操作しないことを確認していることを示します。

レコードに CREATE `action` しかし、レコードを正常に作成できず、 `installationStatus` が「失敗」に設定され、失敗の理由も示されます。

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations/{id}
```

#### ヘッダー

```json
{
    "apikey": "**********"
}
```

または

```json
{
    "sessionID": "*****************"
}
```

#### 本文

_空_

#### 応答

```
200
```

```json
{
    "id": "2892b936-e09e-455a-935f-e1462ab9753c",
    "environmentPromotionPackageId": "4fae2b9d-d315-45f4-909f-a0c0d79fc65d",
    "environmentPromotionPackageVersion": 1,
    "userId": "8fbbc5bcf4f94a5b862483ee05573e73",
    "customerId": "54286d78b064451096752b99bf968481",
    "status": "COMPLETED",
    "environment": "https://{domain}.{environment}.workfront.com",
    "registeredAt": "2021-03-16T02:21:31.908Z",
    "updatedAt": null,
    "translationMap": {
        "ROLE": {
            "5f6d114f006883209828ddd9088e63b3": {
                "name": "DAM Curator",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "600f4bed00028a718599f29575840053"
            },
            ...
        },
        "TMPL": {
            "5f9b317c00b3db5af69abcd1ed5f82aa": {
                "name": "Digital Asset Production (Integrated)",
                "action": "CREATE",
                "isValid": true,
                "targetId": "6054cda40000d5af63dc811d9c2b3a07"
            },
            ...
        },
        ...
    }
}
```



<!--table templates

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /packages</code></td> 
  </tr> 
  </tbody> 
</table>

<table style="table-layout:fixed"> 
 <col> 
 <tbody> 
  <tr> 
   <td><b></b></td> 
  </tr> 
  <tr> 
   <td><pre></pre></td> 
  </tr> 
  </tbody> 
</table>
-->