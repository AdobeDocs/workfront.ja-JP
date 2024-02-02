---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: リンクされたフォルダとドキュメントの移行
description: API を使用して、リンクされたフォルダーとドキュメントを Adobe Experience Manager Assets に移行できます。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 586ab0a8-52ee-4aba-9298-af5a304acb02
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: ht
source-wordcount: '925'
ht-degree: 100%

---

# リンクされたフォルダとドキュメントの移行

API を使用して、リンクされたフォルダーとドキュメントを Adobe Experience Manager Assets に移行できます。

## 手順

1. 以前の外部ドキュメントストレージプロバイダーにリンクされているすべてのドキュメントとフォルダーを特定し、それらの Workfront 内部ドキュメントまたはフォルダーの ID と、含まれているフォルダーのフォルダー ID をメモします。

   >[!NOTE]
   >
   > 特定したすべてのフォルダーまたはドキュメントについて、新しいプロバイダーとのリンクがまだ作成されていないことを確認する必要があります。

1. 新しいリポジトリ内のドキュメントとフォルダーをパスで探し、外部システムでその ID を検索します。

1. 内部の Workfront ID と、新しい外部ストアの ID とのマッピングを作成します。この手順は、次の手順で新しいリンクを作成するために必要です。

1. Workfront で新しいドキュメントまたはドキュメントフォルダーのリンクを作成し、新しい外部 ID を介して新しい場所のリソースを指すようにします。

   1. **ドキュメント**：既存のドキュメントの新しいバージョンを、新しい外部ドキュメントプロバイダーで追加します。
   1. **フォルダー**：同じ場所に、同じ名前の新しいフィルダーを作成します。

>[!CAUTION]
>
>   既存のリンクされたフォルダーを削除しないでください。削除した結果、データが失われる可能性があります。Workfront アプリケーションから古いフォルダーリンクを削除するには、設定エリアでカスタムドキュメント統合を無効にします。


## リンクの移行プロセスの例

![simplified-link-flow](assets/links-flow-simplified.png)

## API 情報

この節の Workfront API について詳しくは、[開発者ドキュメント：ドキュメント](https://developer.workfront.com/documents.html)を参照してください。

### すべてのドキュメントを検索

**providerType** の&#x200B;**ドキュメントプロバイダー**&#x200B;に **documentProviderID** でリンクされた&#x200B;**ドキュメント（DOCU）**&#x200B;をすべて検索します。

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/document/search?fields=currentVersion:*&currentVersion:externalIntegrationType={providerType}
```

[API ドキュメントリファレンス](https://developer.workfront.com/documents.html#get-/docu/search)

### すべてのフォルダーを検索

**providerType** のドキュメントプロバイダーに **documentProviderID** でリンクされた&#x200B;**ドキュメントフォルダー（DOCFDR）**&#x200B;をすべて検索します。

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/documentFolder/search?fields=*,linkedFolder:*&linkedFolder:externalIntegrationType={providerType}
```

API ドキュメント：（ドキュメントフォルダーのエンドポイントは、現在 developer.workfront.com では扱われていません）

### ドキュメントをリンク

**providerType** の&#x200B;**外部ドキュメントプロバイダー**&#x200B;の&#x200B;**ドキュメント（DOCU）**&#x200B;を **documentProviderID** でリンクします。

>[!IMPORTANT]
>
>ドキュメントは一時的に保存されます。つまり、ドキュメントのすべてのバージョンにアクセスできます。リンクを作成する際に、既存のドキュメント ID を指定できるので、そのドキュメントに新しいバージョンを書き込むだけで、そのデータは外部の新しいプロバイダーでホストされます。このドキュメント ID は、置き換えるドキュメントリンクで見つかったドキュメント ID と同じです。これは同じ概念ドキュメントです。この新しいバージョンのバイトが別のプロバイダーで保存されていることを示します。

```
Http Method: POST
 
Endpoint: {host}/internal/documents/linkExternalObjects
 
Http Body:
refObjCode=DOCU&refObjID={documentId}&providerType={providerType}&documentProviderID={documentProviderID}
```

API ドキュメント：（内部リンクエンドポイントは、現在 developer.workfront.com では扱われていません）

### フォルダーのリンク

**providerType** の&#x200B;**外部ドキュメントプロバイダー**&#x200B;の&#x200B;**ドキュメントフォルダー（DOCFDR）**&#x200B;を **documentProviderID** でリンクします。

>[!IMPORTANT]
>
>フォルダーのリンクには、ドキュメントのリンクの場合とは異なり、新しいリンクを配置する Workfront のフォルダーの「documentFolderId」が必要です。コピーするリンク先のフォルダーとして最も考えられるのは、同じ親フォルダーです。

>[!CAUTION]
>
>フォルダーの一時保存はありません。古いフォルダーは削除しないでください。設定エリアでカスタムドキュメントの統合を無効にして、古いフォルダーを削除します。


```
Http Method: POST
 
Endpoint: {host}/internal/document/version/linkExternal
 
Http Body:
providerType={providerType}&documentProviderID={documentProviderID}&breadcrumb=[]&linkAction=LINKEXTERNAL&refObjCode={USER|PROJECT_TASK|TEMPLATE_TASK|securityRootObjectCode}&refObjID={userID|taskID|templateTaskID|securityRootId}&destFolderID={parentFolderId}
```

API ドキュメント：（内部リンクエンドポイントは、現在 developer.workfront.com では扱われていません）

## 重要な用語

* **ドキュメント**：Workfront 内のデジタルアセット

* **ドキュメントフォルダー**：Workfront 内のデジタルアセットのコンテナ

* **ドキュメント ID**：デジタルアセットの Workfront 内部 ID

* **ドキュメントフォルダー ID**：デジタルアセットフォルダーの Workfront 内部 ID

* **ドキュメントプロバイダー ID**：特定のドキュメントプロバイダーに関連付けられた ID

>[!IMPORTANT]
>
> 任意のドキュメントプロバイダータイプに対して、1 人の顧客が複数のインスタンスを接続している場合があります。例えば、複数の AEM リポジトリがリンクされている場合があります。または、複数の Google Drive インスタンスがリンクされている場合があります。ドキュメントプロバイダー ID は、置き換え先または切り替え先の接続タイプの特定のインスタンスを示しています。

* **ドキュメントストレージプロバイダータイプ（「外部統合タイプ」とも呼ばれます）**：Workfront でサポートしているドキュメントストレージプロバイダー統合のタイプ。専用の統合または「カスタム統合」を使用します。

* **現在のドキュメントストレージプロバイダータイプ（providerType）**：

  ```
  ATTASK
  BOX
  GOOGLE
  SHAREPOINT
  WEBDAM
  WORKFRONTDAM
  INFERNO
  WIDEN
  DROPBOX
  DROPBOX_BUSINESS
  ONEDRIVE
  QUIP
  WEBHOOKS
  AEM
  MOCK
  ```

* **リンクされたドキュメント**：外部のドキュメントストレージプロバイダーでホストされているデジタルアセット。Workfront では、アセットの内部「ドキュメント ID」を独自に保持していますが、バイトデータは外部に保存されます。これを容易にするために、Workfront では、リモートリポジトリまたはストア内にある外部参照リソースの特定に役立つ「外部ドキュメント ID」も保存します。

* **リンクされたドキュメントフォルダー**：外部のドキュメントストレージプロバイダーでホストされているデジタルアセットのコンテナ。Workfront では、アセットの内部「ドキュメントフォルダー ID」を独自に保持していますが、バイトデータは外部に保存されます。これを容易にするために、Workfront では、リモートリポジトリまたはストア内にある外部参照リソースの特定に役立つ「外部ドキュメント ID」も保存します。

* **外部ドキュメント ID**：アセットを Workfront の外部に保存する際に割り当てられる ID。Workfront では、この「外部ドキュメント識別子」フィールドを使用して、Workfront の内部識別子を、外部システム内のアセットを見つけるための識別子にマッピングします。したがって、新しい外部ストアからドキュメントまたはフォルダーをリンクする場合は、外部ドキュメントプロバイダーが新しいリポジトリまたはストア内のドキュメントを識別できるように、適切な形式で新しい外部ドキュメント識別子を作成する必要があります。

  >[!NOTE]
  >
  > Workfront には、外部ドキュメント識別子の標準がまだありません。AEM ID には新しい仕様が使用されつつありますが、他の ID の場合、外部ドキュメント ID は、プロバイダータイプに応じて異なる形式を取る可能性があります。


* **オブジェクトタイプ**：このドキュメントの目的でのみ使用される API 専用の用語です。これは、操作する Workfront 内の汎用オブジェクトの一種です。この場合、「DOCU」と「DOCFDR」のタイプをそれぞれ持つドキュメントとフォルダーを操作します。

* **オブジェクト ID**：操作する汎用オブジェクトの内部 Workfront 識別子。ドキュメントやフォルダーを操作する際に、これがそれぞれドキュメント ID またはドキュメントフォルダー ID になります。
