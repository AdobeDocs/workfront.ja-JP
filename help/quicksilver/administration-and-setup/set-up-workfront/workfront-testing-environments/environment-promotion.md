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
recommendations: noDisplay, noCatalog
exl-id: dd3c29df-4583-463a-b27a-bbfc4dda8184
source-git-commit: b44c83314a06592e21ab3c4316e2574b75e85715
workflow-type: tm+mt
source-wordcount: '1894'
ht-degree: 9%

---

# オブジェクトの移動間隔： [!DNL Workfront] 環境の使用 [!DNL Workfront] 環境プロモーション API

環境プロモーション機能は、設定関連のオブジェクトを環境間で移動する機能を提供することを目的としています。 この記事で説明するように、Workfront API を使用してこれらのオブジェクトを移動できます。

Workfrontアプリケーションを使用して環境間でオブジェクトを移動する手順については、以下を参照してください。

* [環境プロモーションパッケージの作成または編集](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
* [環境プロモーションパッケージのインストール](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] プラン</td> 
   <td> <p>Enterprise、Prime または Ultimate</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!DNL Workfront] ライセンス</p> </td> 
   <td> <p>[!UICONTROL Plan] </p> <p>[!DNL Workfront] の管理者になる必要があります。[!DNL Workfront] 管理者について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーへの完全な管理アクセス権の付与</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">オブジェクト権限</p> </td> 
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

プロモート可能なオブジェクトとそれに含まれるプロモート可能なサブオブジェクトのリストについては、 [環境の昇格でサポートされるオブジェクト](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#supported-objects-for-environment-promotion) 記事内 [Workfront環境間でのオブジェクトの移動の概要](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md).

## 認証

API はリクエストごとに認証を行い、リクエストされたオブジェクトを表示または変更するためのアクセス権をクライアントが持っていることを確認します。

認証は、セッション ID または API キーを渡すことで実行されます。このキーは、次の方法で指定できます。

### リクエストヘッダー認証

推奨される認証方法は、セッショントークンを含む SessionID という名前のリクエストヘッダーを渡すことです。[クロスサイトリクエストフォージェリー（CSRF）](https://en.wikipedia.org/wiki/Cross-site_request_forgery)攻撃に対して安全で、キャッシュ目的で URI に干渉することがありません。

リクエストヘッダーの例を次に示します。

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

## API エンドポイント

* [パッケージの作成](#create-a-package)
* [パッケージのリストの取得](#get-a-list-of-packages)
* [ID によるパッケージの取得](#get-a-package-by-id)
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
>各項目には、 `entities` コレクション。 これは、 `ID` フィールドに入力します。 オプションの `name` 何を知りやすくするための属性 `ID` は、を表します。
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
    "name": "Agency Onboarding - 2023-06-06",
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
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "ASSEMBLING",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d"
    }
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
            "createdAt": "2023-06-06T17:29:21.600Z",
            "deletedAt": null
},
        {...}
    ]
}
```

&lt;! — 上記の「ステータス」を確認します。 — 追加されたのですか？—>

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
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "DRAFT",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "packageEntities": {
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
1. status （値の検証を含む文字列）

使用可能なステータスについて詳しくは、 [環境の昇格ステータス](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#environment-promotion-statuses) 記事内 [Workfront環境間でのオブジェクトの移動の概要](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md).


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
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "ACTIVE",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "publishedAt": "2023-06-06T19:39:01.600Z",
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "packageEntities": {
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

>[!IMPORTANT]
>
>インストールを実行する前に、このプリランを実行する必要があります。 インストールの実行時に、この呼び出しから生成された ID を使用します。

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
   <td><p>対応するレコードがターゲット環境で見つかった場合、アクションは USEEXISTING に設定され、 <code>targetId</code> は、 <code>translationmap</code>.</p><p>このアクションが <code>translationmap</code> が <code>/install</code> エンドポイントの場合、インストールサービスはレコードを作成しません。 ただし、 <code>targetId</code> このレコードへの参照を持つ他のオブジェクトのマップエントリに含まれます。</p><p>例えば、パッケージのデプロイ先のターゲット環境に「デフォルトグループ」が存在する場合があります。 2 つの「Default Group」レコードを持つことはできないので、インストールサービスは、プロジェクト、フォーム、このグループに関連する他のエンティティなど、「Default Group」への参照を含む他のオブジェクト作成アクションで、既存のグループの GUID を使用します。</p><p><b>注意：</b> <ul><li><p>USEEXISTING アクションが割り当てられると、ターゲット環境の既存のレコードは変更されません。 </p><p>例えば、パッケージの構築元のサンドボックスで「デフォルトグループ」の説明が変更され、ターゲット環境で説明の値が異なる場合、このを使用したインストール後も、値は変更されません <code>translationmap</code>.</li></ul></td> 
  </tr> 
  <tr> 
   <td>上書き</td> 
   <td><p>このアクションは自動的には設定されません。</p><p>このアクションを使用すると、ターゲット環境に存在するオブジェクトを更新できます。 割り当てられた CREATE または USEEXISTING アクションを手動で上書きしてから、 <code>/install</code> を呼び出します。<ul><li>ユーザーは、テスト環境でオブジェクトを更新し、OVERWRITING アクションを使用して、ターゲット環境でそのオブジェクトを更新できます。</p></li><li><p>ユーザーが最初に 1 つのプロモーションパッケージをインストールし、将来新しい（または更新された）パッケージに初期パッケージ内のオブジェクトの変更が含まれる場合、OVERWRITING を使用して、以前にインストールしたオブジェクトを置き換え（上書き）できます。 </p></li><ul></td> 
  </tr> 
  <tr> 
   <td>無視</td> 
   <td><p>このアクションは自動的には設定されません。</p><p>割り当てられた CREATE または USEEXISTING アクションを手動で上書きしてから、 <code>/install</code> を呼び出します。</p><p><b>メモ： </b><ul><li><p>最初に CREATE に設定されたレコードが IGNORE に設定されている場合は、すべての子レコードも IGNORE に設定する必要があります。</p><p>例えば、テンプレートレコードが CREATE アクションにマッピングされ、インストールユーザーがそのレコードをデプロイメントから除外する場合、テンプレートのアクションを IGNORE に設定できます。</p><p>この場合、インストールユーザーがテンプレートタスク、テンプレートタスクの割り当て、テンプレートタスクの先行タスク、キュー定義、キュートピック、ルーティングルールなどを IGNORE に設定しないと、展開は失敗します。</p></li><li><p>最初に USEEXISTING に設定されたレコードが IGNORE に設定されている場合は、インストールプロセス中に何らかの悪影響が出る場合があります。</p><p>たとえば、グループレコードが USEEXISTING アクションにマッピングされ、インストールユーザーがグループを必要とするオブジェクト（グループが割り当てられていないプロジェクトは存在できない）のアクションを IGNORE に変更した場合、システムの既定のグループがそのプロジェクトに割り当てられます。</p></li><li><p>元々 USEEXISTING に設定されていたレコードが CREATE に設定されている場合、Workfrontエンティティの多くは一意の名前の制約を持つので、インストールプロセス中に悪影響が出る場合があります。</p><p>例えば、「Default Group」レコードが USEEXISTING アクションにマッピングされ、インストールユーザーがアクションを CREATE に変更した場合、「Default Group」が既に存在するので、インストールはすべての手順を完了できません。 グループ名は一意である必要があります。</p><p>一部のエンティティには、一意の名前の制約がありません。 これらのオブジェクトの場合、この変更を行うと、同じ名前の 2 つのレコードが作成されます。 例えば、テンプレート、プロジェクト、ビュー、フィルター、グループ、レポート、ダッシュボードには、一意の名前制約は必要ありません。 これらのレコードに一意の名前を付けることをお勧めしますが、適用されません。</p></li></ul></p></td> 
  </tr> 
  </tbody> 
</table>

現在、UPDATE はサポートされていません。 `action` （このサービスのアルファ機能）。 更新を許可するオプション `action` 我々が研究しているものです

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/:id/prepare-installation
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
{
    "environmentPromotionPackageId": "45f2ae94-76c0-4b13-8f3b-f688de83043d",
    "environmentPromotionPackageVersion": 1,
    "id": "c0bc79bd-c9c1-4b5b-b118-b1241392de0e",
    "userId": "5ba38da500b752fd66439d4f6a9999a1",
    "customerId": "5ba38d9d00b74f0c7a38b1b487fc9710",
    "status": "PREPARING",
    "environment": "mmi.my.workfront.com",
    "registeredAt": "2023-10-19T20:00:16.697Z",
    "updatedAt": "2023-10-19T20:00:16.701Z",
    "translationMap": {
        "CTGY": {
            "62d9c9a0000013aeeefe7242a0a5fdb2": {
                "name": "Example Document Form",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c9a0000013aeeefe7242a0a5fdb2"
            }
        },
        "PGRP": {
            "62d1eee4001c6618e6b9f9a588ba1598": {
                "name": "Asset Detail",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee4001c6618e6b9f9a588ba1598"
            }
        },
        "GROUP": {
            "5ba38da500b752b0f46d13186030b7ad": {
                "name": "Default Group",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "5ba38da500b752b0f46d13186030b7ad"
            }
        },
        "PARAM": {
            "62d1eee400f8578895166ee91a83f97a": {
                "name": "Asset Type",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee400f8578895166ee91a83f97a"
            },
            "62d1eee50001407c713514a8970b58e4": {
                "name": "Keywords",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee50001407c713514a8970b58e4"
            },
            "62d1eee5000333ac3981ea4f3df6d88e": {
                "name": "Permitted Uses",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee5000333ac3981ea4f3df6d88e"
            },
            "62d1eee5000b188e9ec8039a097fc7ab": {
                "name": "File Format",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee5000b188e9ec8039a097fc7ab"
            },
            "62d1eee500100c159fd5f838ce560507": {
                "name": "CTA",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee500100c159fd5f838ce560507"
            },
            "62d9c988001c1f23954dbb9d646335b5": {
                "name": "Other CTA",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c988001c1f23954dbb9d646335b5"
            },
            "62d9c9880070f546cf4c798ea6c3eaa4": {
                "name": "Other Audience",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c9880070f546cf4c798ea6c3eaa4"
            },
            "62d9c990006258baf1b40f2569c3eab7": {
                "name": "Target Audience",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c990006258baf1b40f2569c3eab7"
            }
        }
    }
}
```

>[!NOTE]
>
>インストールを実行する必要がある ID は、 `id` フィールドに入力します。 この例では、 `id` フィールドの先頭が 3 番目で、 `c0bc79bd`.

### インストールの実行

>[!IMPORTANT]
>
>インストールを実行する前に、事前に実行する必要があります。 インストールの実行時に、事前実行から生成された ID を使用します。
>
>事前実行の実行後に、宛先環境（パッケージのデプロイ先となる環境）に変更が加えられている場合は、再度事前実行を実行することをお勧めします。 再度プリランを実行しない場合は、実行が正しく完了しないか、インストールが失敗する可能性があります。
>
>事前実行の実行手順については、 [事前実行の実行](#execute-a-pre-run).

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /install</code></td> 
  </tr> 
  </tbody> 
</table>

この呼び出しにより、POSTURL で識別されるターゲット環境へのプロモーションパッケージのインストールが開始されます。

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations/{id}/install
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
202
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
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations?environmentPromotionPackageId={environmentPromotionPackageId}
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
        "status": "INSTALLED",
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
    "status": "INSTALLED",
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
