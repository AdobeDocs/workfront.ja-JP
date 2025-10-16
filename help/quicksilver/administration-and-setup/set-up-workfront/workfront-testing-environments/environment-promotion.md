---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: ある環境から別の環境にオブジェクトを移動する
description: 環境プロモーション機能は、設定関連のオブジェクトを環境間で移動する機能を提供することを目的としています。トランザクションオブジェクトを移動する機能はサポートしていません（限定的な例外はあります）。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: dd3c29df-4583-463a-b27a-bbfc4dda8184
source-git-commit: 7ca27795ec115a112acb55113bfade4a5fee15ad
workflow-type: tm+mt
source-wordcount: '2088'
ht-degree: 88%

---

# [!DNL Workfront] Environment Promotion API を使用して [!DNL Workfront] 環境間でオブジェクトを移動する

環境プロモーション機能を使用すると、設定関連のオブジェクトを環境間で移動できます。 この記事の説明に従って、Workfront API を使用してこれらのオブジェクトを移動できます。

Workfront アプリケーションを使用して環境間でオブジェクトを移動する手順については、以下を参照してください。

* [環境のプロモーションパッケージの作成または編集](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
* [環境のプロモーションパッケージのインストール](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)


## アクセス要件

以下が必要です。

<table>
  <tr>
   <td>Adobe Workfront パッケージ
   </td>
   <td> <p>PrimeまたはUltimate</p>
   </td>
  </tr>
  <tr>
   <td><strong>Workfront ライセンス </strong>
   </td>
   <td> <p>標準</p>&gt;
   </td>
  </tr>
   <tr>
   <td>アクセスレベル設定
   </td>
   <td><p>Workfront 管理者である必要があります。</p>
   </td>
  </tr>
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

## 前提条件

プロモーションパッケージを作成するエンドポイントは、既にソース環境が設定されていることを前提としています。この API 呼び出しでは、手動で [!DNL Workfront] objCodes のオブジェクトマップとオブジェクトの GUID を作成します。このマップの具体的な構造を以下に示します。

## 環境のプロモーションでサポートされるオブジェクト

環境プロモーション機能は、設定関連のオブジェクトを環境間で移動する機能を提供することを目的としています。トランザクションオブジェクトを移動する機能はサポートしていません（限定的な例外はあります）。

プロモーション可能なオブジェクトとこれに含まれるプロモーション可能なサブオブジェクトのリストについては、[Workfront 環境間でのオブジェクトの移動の概要](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md)の記事の[環境のプロモーションでサポートされているオブジェクト](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#supported-objects-for-environment-promotion)を参照してください。

## 認証

API はリクエストごとに認証を行い、リクエストされたオブジェクトを表示または変更するためのアクセス権をクライアントが持っていることを確認します。

認証は、次の方法で指定できるセッション ID または API キーを渡すことで実行されます。

### リクエストヘッダー認証

推奨される認証方法は、セッショントークンを含む SessionID という名前のリクエストヘッダーを渡すことです。[クロスサイトリクエストフォージェリー（CSRF）](https://ja.wikipedia.org/wiki/%E3%82%AF%E3%83%AD%E3%82%B9%E3%82%B5%E3%82%A4%E3%83%88%E3%83%AA%E3%82%AF%E3%82%A8%E3%82%B9%E3%83%88%E3%83%95%E3%82%A9%E3%83%BC%E3%82%B8%E3%82%A7%E3%83%AA)攻撃に対して安全で、キャッシュ目的で URI に干渉することがありません。

リクエストヘッダーの例を次に示します。

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

## API エンドポイント

* [パッケージを作成](#create-a-package)
* [パッケージのリストを取得](#get-a-list-of-packages)
* [ID でパッケージを取得](#get-a-package-by-id)
* [パッケージの特定のプロパティを更新](#update-specific-properties-of-a-package)
* [パッケージを削除](#delete-a-package)
* [事前実行を実行](#execute-a-pre-run)
* [インストールを実行](#execute-an-installation)
* [特定のパッケージのインストールのリストを取得](#get-a-list-of-installations-for-a-specific-package)
* [インストールのインストール詳細を取得](#get-the-installation-details-for-an-installation)

### パッケージを作成

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /packages</code></td> 
  </tr> 
  </tbody> 
</table>

この呼び出しでは、複数ステップのプロセスが実行されます。

最初のステップでは、「ASSEMBLING」ステータスの空のプロモーションパッケージが作成されます。

2 番目のステップでは、POST 本文で指定された `objectCollections` 配列を使用して、Workfront に要求されたレコードを組み立てます。要求されたレコードの数と Workfront の設定によっては、このステップが完了するまでに数分かかる場合があります。このプロセスの終わりに、空のプロモーションパッケージに `packageEntities` が反映され、ステータスが自動的に「DRAFT」に設定されます。


>[!NOTE]
>
>`objectCollections` 配列の構造をメモしておきます。
>
>配列内の各項目には、Workfront API エクスプローラーに記載されているオブジェクトコードに対応する `objCode` キーが含まれます。
>
>また、各項目には `entities` コレクションも含まれています。これは、`ID` フィールドを想定しています。また、`ID` で表されている内容がわかりやすくなるように、オプションの `name` 属性を指定することもできます。
>
>`objectCollections` リストで要求できるオブジェクトコードのリストについては、この記事の[環境プロモーションでサポートされているオブジェクト](#supported-objects-for-environment-promotion)の節を参照してください。

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

### パッケージのリストを取得

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages</code></td> 
  </tr> 
  </tbody> 
</table>

この呼び出しでは、顧客に属するプロモーションパッケージのフィルタリングされていないリストを返します。

応答には、顧客の Workfront のサンドボックス、プレビューインスタンス、実稼動インスタンスのいずれかから作成されたすべてのパッケージが含まれます。

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

&lt;!-- 前述の「ステータス」を確認します--追加しましたか？-->

### ID でパッケージを取得

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

この呼び出しでは、要求されたプロモーションパッケージの詳細を返します。

リクエストは、プロモーションパッケージの元のソースに関係なく、任意の環境を通じて行うことができます。

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

### パッケージの特定のプロパティを更新

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>PATCH /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

この呼び出しでは、PATCH 本体で提供されるプロモーションパッケージのコンテンツが更新されます。

編集可能な属性は次のとおりです。

1. name（文字列）
1. description（文字列）
1. status（値の検証を含む文字列）

利用可能なステータスについて詳しくは、[Workfront 環境間でのオブジェクトの移動の概要](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md)の記事の[環境のプロモーションでサポートされているオブジェクト](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#environment-promotion-statuses)を参照してください。


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

### パッケージを削除

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>DELETE /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

この呼び出しでは、プロモーションパッケージレコードが削除されます。このアクションは元に戻せません。

>[!NOTE]
>
>プロモーションパッケージを削除するのではなく、パッケージのステータスを DISABLED に変更することをお勧めします。これにより、パッケージを取得できるようになり、デプロイされた場所のインストール履歴が保持されます。

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

### 事前実行を実行

>[!IMPORTANT]
>
>インストールを実行する前に、この事前実行を実行する必要があります。インストールを実行する際に、この呼び出しから生成された ID を使用します。

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST  {customer-domain}/environment-promotion/api/v1/packages/{id}/prepare-installation</code></td> 
  </tr> 
  </tbody> 
</table>

この呼び出しでは、URL で識別されたパッケージ定義とターゲット環境の間の比較が行われます。

結果は、ターゲット環境でプロモーションオブジェクトが見つかったかどうかを識別する JSON 本文です。

プロモーションオブジェクトごとに、次の `actions` のいずれかが設定されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>作成</td> 
   <td><p>対応するレコードがターゲット環境で見つからない場合、アクションは CREATE に設定されます。</p><p>このアクションが <code>/install</code> エンドポイントに指定される <code>translationmap</code> に設定されている場合、インストールサービスではレコードを作成します。</p></td> 
  </tr> 
  <tr> 
   <td>USEEXISTING</td> 
   <td><p>対応するレコードがターゲット環境で見つかると、アクションが USEEXISTING に設定され、<code>targetId</code> も <code>translationmap</code> にキャプチャされます。</p><p>このアクションが <code>/install</code> エンドポイントに指定される <code>translationmap</code> に設定されている場合、インストールサービスではレコードを作成しません。ただし、このレコードへの参照を持つ可能性のある他のオブジェクトのマップエントリに含まれる <code>targetId</code> が使用されます。</p><p>例えば、パッケージをデプロイするターゲット環境で「デフォルトグループ」が見つかる場合があります。「デフォルトグループ」レコードを 2 つ持つことはできません。そのため、インストールサービスでは、このグループに関連するプロジェクト、フォームまたはその他のエンティティなど、「デフォルトグループ」への参照を含む他のオブジェクト作成アクションで既存のグループの GUID を使用します。</p><p><b>メモ：</b> <ul><li><p>USEEXISTING アクションを割り当てる場合、ターゲット環境内の既存のレコードは変更されません。 </p><p>例えば、パッケージの作成元のサンドボックスで「デフォルトグループ」の説明を変更し、ターゲット環境で説明の値が異なる場合、この <code>translationmap</code> をインストールした後も値は変更されません。</li></ul></td> 
  </tr> 
  <tr> 
   <td>OVERWRITING</td> 
   <td><p>このアクションは自動的に設定されません。</p><p>このアクションにより、ターゲット環境に存在するオブジェクトを更新できます。<code>/install</code> 呼び出しを実行する前に、割り当てられた CREATE または USEEXISTING アクションを手動で上書きする機能を提供します。<ul><li>ユーザーは、テスト環境でオブジェクトを更新し、OVERWRITING アクションを使用してターゲット環境でそのオブジェクトを更新できます。</p></li><li><p>ユーザーが最初に 1 つのプロモーションパッケージをインストールし、将来の新しい（または更新された）パッケージに初期パッケージ内のオブジェクトへの変更が含まれる場合、ユーザーは OVERWRITING を使用して、以前にインストールされたオブジェクトを置き換える（上書きする）ことができます。 </p><p>上書きの詳細については、この記事の [ 上書き ] （#overwriting）を参照してください。</li><ul></td> 
  </tr> 
  <tr> 
   <td>IGNORE</td> 
   <td><p>このアクションは自動的に設定されません。</p><p><code>/install</code> 呼び出しを実行する前に、割り当てられた CREATE または USEEXISTING アクションを手動で上書きする機能を提供します。</p><p><b>メモ： </b><ul><li><p>最初に CREATE に設定したレコードが IGNORE に設定されている場合は、子レコードも IGNORE に設定する必要があります。</p><p>例えば、テンプレートレコードが CREATE アクションでマッピングされ、インストールユーザーがデプロイメントから除外する場合、テンプレートのアクションを IGNORE に設定できます。</p><p>この場合、インストールユーザーがテンプレートタスク、テンプレートタスク割り当て、テンプレートタスク先行タスク、キュー定義、キュートピック、ルーティングルールなども IGNORE に設定しない場合、デプロイメントはインストール試行に失敗します。</p></li><li><p>最初に USEEXISTING に設定したレコードが IGNORE に設定されている場合は、インストールプロセス中に何らかの悪影響が生じる場合があります。</p><p>例えば、グループレコードが USEEXISTING アクションでマッピングされ、インストールユーザーがグループを必要とするオブジェクトのアクションを IGNORE に変更した場合（例：グループが割り当てられていないとプロジェクトは存在できません）、システムのデフォルトグループがそのプロジェクトに割り当てられます。</p></li><li><p>最初に USEEXISTING に設定したレコードが CREATE に設定された場合は、多くの Workfront エンティティには一意の名前制約があるので、インストールプロセス中に何らかの悪影響が生じる場合があります。</p><p>例えば、「デフォルトグループ」レコードが USEEXISTING アクションでマッピングされ、インストールユーザーがアクションを CREATE に変更した場合、「デフォルトグループ」が既に存在するので、インストール試行ではすべてのステップを完了できません。グループ名は一意にする必要があります。</p><p>一部のエンティティには、一意の名前制約がありません。これらのオブジェクトの場合、この変更を行うと、同じ名前の 2 つのレコードが作成されます。例えば、テンプレート、プロジェクト、ビュー、フィルター、グループ化、レポートおよびダッシュボードには、一意の名前制約は必要ありません。これらのレコードに対して、一意の名前を付けることがベストプラクティスですが、強制ではありません。</p></li></ul></p></td> 
  </tr> 
  </tbody> 
</table>

現在、このサービスのアルファ版機能では、UPDATE `action` はサポートされていません。UPDATE `action` を許可するオプションについては、現在調査中です。

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
>インストールを実行するために必要な ID は、`id` フィールドです。この例では、`id` フィールドは上から 3 番目にあり、`c0bc79bd` で始まる値を持ちます。

### インストールを実行

>[!IMPORTANT]
>
>インストールを実行する前に、事前実行を実行する必要があります。インストールを実行する際に、事前実行で生成された ID を使用します。
>
>事前実行の実行後に、宛先環境（パッケージのデプロイ先の環境）に変更を行った場合は、再度事前実行を実行することをお勧めします。事前実行を再度実行しない場合、実行が正確に完了しないか、インストールが失敗する場合があります。
>
>事前実行の実行手順について詳しくは、[事前実行の実行](#execute-a-pre-run)を参照してください。

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /install</code></td> 
  </tr> 
  </tbody> 
</table>

この呼び出しでは、POST URL で識別されたターゲット環境へのプロモーションパッケージのインストール試行が開始されます。

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

### 特定のパッケージのインストールのリストを取得

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /v1/installations?environmentPromotionPackageId={environmentPromotionPackageId}
</code></td> 
  </tr> 
  </tbody> 
</table>

結果には、パッケージがデプロイされた、すべての環境のインストールイベントが含まれます。リクエストされた環境へのインストールに限定されません。これにより、このパッケージを受け取った環境を識別できます。

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

### インストールのインストール詳細を取得

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /installations/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

この呼び出しは、特定のインストール用にインストールサービスで生成された最終的な `translationMap` を返します。

各レコードは、設定された `action` について、そして、そのアクションがが成功したかどうかを示します。

CREATE `action` を含むレコードの場合、`targetId` フィールドは、ターゲットシステムで新しく作成されたレコードの値で設定されます。また、`installationStatus` フィールドが INSTALLED に設定されます。

USEEXISTING `action` を含むレコードの場合、`targetId` フィールドも設定され、`installationStatus` フィールドが REGISTERED に設定されます。これは、マッピングプロセスが完了し、インストールサービスがレコードを評価して、何も操作が必要ないことを確認します。

レコードに CREATE `action` があるにもかかわらず、レコードが正常に作成されなかった場合、`installationStatus` は FAILED に設定され、失敗の理由も提示されます。

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

## 上書き

これは 3 段階のプロセスです。

1. 翻訳マップを作成します（「インストールの準備」フェーズに類似しています）。
1. 生成された翻訳マップを編集し、上書きするオブジェクトの `action` フィールドと `targetId` フィールドを設定します。 アクションは `OVERWRITING`、`targetId` は上書きするオブジェクトの uuid にしてください
1. インストールを実行します。

* [手順 1 – 翻訳マップの作成](#step-1---create-a-translation-map)
* [手順 2 – 翻訳マップの変更](#step-2---modify-the-translation-map)
* [手順 3 - インストール](#step-3---install)

### **手順 1 – 翻訳マップの作成**

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}/translation-map
```

#### 本文

なし

#### 応答

翻訳マップ（`202 - OK` ステータス）

```json
{
    {objcode}: {
        {object uuid}: {
            "targetId": {uuid of object in destination},
            "action": {installation action},
            "name": {name of the object},
            "isValid": true
        },
        {...more objects}
    },
    {...more objcodes}
}
```


#### 例

```json
{
    "UIVW": {
        "109f611680bb3a2b0c0a8c1f5ec63f6d": {
            "targetId": "6643a26b0001401ff797ccb318f97aa6",
            "action": "CREATE",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIGB": {
        "edb4c6c127d38910e4860eb25569a5cc": {
            "targetId": "6643a26b000178fb5cc27b74cc1e87ec",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIFT": {
        "f97b662e229fd09ee595d8d359ec88bd": {
            "targetId": "6643a26b00015cdd6727b76d6fda1d1d",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "PTLSEC": {
        "4bb80aa88a96420296a7f47bf866f162": {
            "targetId": "4bb80aa88a96420296a7f47bf866f162",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "EXTSEC": {
        "65f8637900015e4dceb6fe079bd5409d": {
            "targetId": "65f8637900015e4dceb6fe079bd5409d",
            "action": "USEEXISTING",
            "name": "Asnyc List",
            "isValid": true
        }
    },
    "PTLTAB": {
        "65f8638a00016422a83ddc3508852d0f": {
            "targetId": "65f8638a00016422a83ddc3508852d0f",
            "action": "CREATEWITHALTNAME",
            "name": "Cool 2.0 The Best",
            "isValid": true
        }
    }
}
```

### 手順 2 – 翻訳マップの変更

この手順にはエンドポイントがありません。

1. [&#x200B; 手順 1 – 翻訳マップの作成 &#x200B;](#step-1---create-a-translation-map) で返された翻訳マップで、インストールするオブジェクトのリストを調べます。
1. 各オブジェクトのアクションフィールドを目的のインストールアクションに更新します。
1. 各オブジェクトの `targetId` を検証します。 set アクションが `USEEXISTING` または `OVERWRITING` の場合、`targetId` は、ターゲット環境のターゲットオブジェクトの UUID に設定する必要があります。 その他のアクションの場合は、targetId を空の文字列にする必要があります。

   >[!NOTE]
   >
   >競合が検出された場合、`targetId` は既に入力されています。

### **手順 3 - インストール**

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}/install
```

#### 本文

これは、単一のフィールド `translationMap` を持つオブジェクトで、[&#x200B; 手順 2 – 翻訳マップの変更 &#x200B;](#step-2---modify-the-translation-map) で変更した翻訳マップと等しくなります。

```json
{
    "translationMap": {
        {objcode}: {
            {object uuid}: {
                "targetId": {uuid of object in destination},
                "action": {installation action},
                "name": {name of the object},
                "isValid": true
            },
            {...more objects}
        },
        {...more objcodes}
    }
}
```


#### 例

```json
{
    "translationMap": {
    "UIVW": {
        "109f611680bb3a2b0c0a8c1f5ec63f6d": {
            "targetId": "6643a26b0001401ff797ccb318f97aa6",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIGB": {
        "edb4c6c127d38910e4860eb25569a5cc": {
            "targetId": "6643a26b000178fb5cc27b74cc1e87ec",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIFT": {
        "f97b662e229fd09ee595d8d359ec88bd": {
            "targetId": "6643a26b00015cdd6727b76d6fda1d1d",
            "action": "OVERWRITING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "PTLSEC": {
        "4bb80aa88a96420296a7f47bf866f162": {
            "targetId": "4bb80aa88a96420296a7f47bf866f162",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "EXTSEC": {
        "65f8637900015e4dceb6fe079bd5409d": {
            "targetId": "65f8637900015e4dceb6fe079bd5409d",
            "action": "USEEXISTING",
            "name": "Asnyc List",
            "isValid": true
        }
    },
    "PTLTAB": {
        "65f8638a00016422a83ddc3508852d0f": {
            "targetId": "65f8638a00016422a83ddc3508852d0f",
            "action": "CREATEWITHALTNAME",
            "name": "Cool 2.0 The Best",
            "isValid": true
        }
    }
}
}
```

#### 応答

応答には、`{uuid of the created installation}` と `202 - ACCEPTED` ステータスが含まれます。

例：`b6aa0af8-3520-4b25-aca3-86793dff44a6`

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
