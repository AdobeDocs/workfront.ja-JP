---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Workfront Fusionを使用して、Adobe Experience Manager ワークフローを含むWorkfront プロジェクトを作成する
description: Workfront Fusionを使用してプロジェクトを作成し、プロジェクトにAdobe Experience Manager ワークフローを含める場合は、この記事で説明する特定のFusion モジュール設定を使用する必要があります。
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps, Workfront Fusion
exl-id: b8132d5e-234d-47f6-a09c-ca46018a2d77
TQID: https://experienceleague.adobe.com/Hegf4kJc65Le5-PttBh6pLzyR8zvydUbbjidxrK0se0
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 9f74d7a567a77128b5d6d6cfa1d4a8d559998a0f
workflow-type: tm+mt
source-wordcount: 1040
ht-degree: 19%

---

# Workfront Fusion を使用して、Workfront イシューを Adobe Experience Manager のワークフローを含むプロジェクトに変換

Workfront Fusionを使用してプロジェクトを作成し、プロジェクトにAdobe Experience Manager ワークフローを含める場合は、この記事で説明する特定のFusion モジュール設定を使用する必要があります。

>[!NOTE]
>
>ワークフローを使用できるのは Adobe Experience Manager as a Cloud Service 統合のみで、 Adobe Experience Manager Assets Essentials との統合では使用できません。この機能は、新規ドキュメント領域では使用できません。


## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table>
  <tr>
    <td><strong>Adobe Workfront パッケージ</strong></td>
   <td> <p>任意の Adobe Workfront Workflow パッケージと任意の Adobe Workfront Automation および Integration パッケージ</p><p>Workfront Ultimate</p><p>Workfront Fusion を追加購入した Workfront Prime および Select パッケージ。</p> </td> 
  </tr>
  <tr>
   <td><strong>Adobe Workfront ライセンス</strong></td>
   <td><p>コントリビューター以上</p><p>リクエスト以上</p></td>
  </tr>
  <tr>
   <td><strong>製品</strong></td>
   <td>
     <p><b>Adobe Experience Manager:</b></p>
     <ul>
       <li>
         <p>Experience Manager Assets as a Cloud Service または Assets Essentials を使用するには、Admin Console に製品にユーザーとして追加されていることが必要です。</p>
       </li>
       <li>
        <p>Adobe Experience Manager のリポジトリへの書き込みアクセス権が必要です。</p>
       </li>
     </ul>
     <p><b>Workfront Fusion:</b></p>
     <ul>
       <li>
        <p>組織が Workfront Automation および Integration を含まない Select またはPrime Workfront パッケージを持っている場合は、Adobe Workfront Fusion を購入する必要があります。</li></ul>
       </li>
     </ul>
   </td>
  </tr>
  <tr>
   <td><strong>アクセスレベル設定</strong>
   </td>
   <td><p>ドキュメントへのアクセスを編集</p>
   </td>
  </tr>
</table>

+++

## 前提条件

開始する前に、

* Workfront 管理者は、Adobe Experience Manager 統合でワークフローを設定する必要があります。 詳しくは、[Experience Manager Assets as a Cloud Service 統合の設定](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional)を参照してください。
* Adobe Experience Manager統合リンクされたフォルダーワークフローで設定されたプロジェクトテンプレートが必要です。
* このモジュールの接続を設定するには、WorkfrontでOAuth アプリケーションを作成している必要があります。

  手順については、この記事の「[OAuth アプリケーションの作成](#create-an-oauth-application)」を参照してください。

## モジュール設定

Workfront Fusionで、Adobe Experience Manager ワークフローを含むプロジェクトを作成する場合は、Workfront/その他のアクションモジュールを使用する必要があります。

1. シナリオに&#x200B;**Workfront** > **Misc Action** モジュールを追加します。
1. 「**Connection**」フィールドで、このモジュールが使用するアカウントに接続するWorkfront接続を選択します。

   接続の作成手順については、Workfront モジュールの「[Connect [!DNL Workfront] to [!DNL Workfront Fusion]](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-modules#connect-workfront-to-workfront-fusion)」を参照してください。

   接続を作成する必要があるクライアント IDとクライアントシークレットの作成手順については、この記事の「[OAuth アプリケーションの作成](#create-an-oauth-application)」を参照してください。

1. **レコードタイプ** フィールドで、`Issue`を選択します。
1. **アクション** フィールドで、`convertToProject`を選択します。
1. 「**ID**」フィールドに、プロジェクトに変換するイシューのIDを入力するか、マッピングします。
1. **詳細設定を表示**&#x200B;を有効にします。
1. モジュールの一番下までスクロールして、**プロジェクト（詳細コレクション）** フィールドを見つけます。
1. 次のテキストを&#x200B;**プロジェクト（詳細コレクション）** フィールドに貼り付けます。

   ```
   {
       "aemNativeFolderTreeIDs": ["Folder Tree ID here"],
       "aemNativeFolderWorkflowEnabled": "true",
       "name": "New project name here",
       "templateID": "Template ID here"
   }
   ```

1. `Folder tree ID here`をフォルダーIDに置き換えます。

   フォルダーツリーIDを見つけるには、この記事の「[ フォルダーツリーIDを見つける](#locate-folder-tree-ids)」を参照してください。

   複数のフォルダーツリーを使用するには、IDをコンマで区切ります。

   `"aemNativeFolderTreeIDs": ["Folder tree ID here","Second folder tree ID here"],`
1. `New project name here`を、新しいプロジェクトの名前に置き換えます。
1. `Template ID here`を、新しいプロジェクトに使用するテンプレートのIDに置き換えます。

   以前のモジュール（Workfront/検索モジュールなど）からテンプレート IDをマッピングしたり、WorkfrontのテンプレートのページのURLにテンプレート IDを配置したりできます。

1. モジュール設定を保存するには、**OK**&#x200B;をクリックします。

## フォルダーツリーIDの検索

フォルダーツリーのIDを見つけるには：

>[!NOTE]
>
>これらの手順では、Chrome ブラウザーを使用します。

1. Workfrontで、このプロジェクトに使用するテンプレートを開きます。 このテンプレートには、プロジェクトに使用するAdobe Experience Manager設定が含まれている必要があります。
1. お使いのブラウザーの開発者用ツールを開きます。
1. 開発者ツールで「**ネットワーク**」タブを開きます。
1. 「**フィルター**」ボックスに「`object-workflow`」と入力します。
1. 「名前」列で、表示される英数字IDをクリックします。

   ![ フォルダーID 1](assets/finding-folder-id-1.png)を検索しています

1. 英数字IDの右側にある「**プレビュー**」タブをクリックします。
1. 次の折りたたまれたセクションを開きます。
   1. `data`
   1. `objectWorkflow`
   1. `workflows`
   1. `enhancedLinkedFolderCreationWorkflow`
   1. `enhancedLinkedFolderCreationWorkflowConfigurations`

   各フォルダーツリーは数字で表されます。 0 （ゼロ）はリストの最初のフォルダーを表し、1は2番目のフォルダーを表します。 テンプレートにフォルダーツリーが1つだけ含まれている場合は、番号0になります。

1. 新しいプロジェクトに使用するフォルダーツリーを開きます。 `_id` フィールド値をメモします。 複数のフォルダーツリーを使用する場合は、使用するフォルダーツリーのすべての`_id` フィールド値をメモします。

   ![ フォルダーID 2](assets/finding-folder-id-2.png)を検索しています

   これらは、**Workfront** > **その他のアクション** Fusion モジュールの&#x200B;**プロジェクト（詳細コレクション）** フィールドに入力する`aemNativeFolderTreeIDs`値です。

## OAuth アプリケーションの作成

このモジュールの接続用にWorkfrontでOAuth アプリケーションを設定する必要があります。 これは、Fusionの特定のWorkfront接続に対して1回だけ実行する必要があります。

1. Workfrontで、OAuth アプリケーションの作成を開始します。「[!DNL Workfront]統合のOAuth2 アプリケーションの作成」の記事の「[ ユーザー資格情報（認証コードフロー） ](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-application-using-user-credentials-authorization-code-flow)を使用してOAuth2 アプリケーションを作成する」で説明されています。
1. クライアント IDとクライアントシークレットを安全な場所にコピーします。
1. 「**リダイレクト URI**」フィールドに、次のように入力します。

   ```
   http://app.workfrontfusion.com/oauth/cb/workfront-workfront
   ```

1. 「**保存**」をクリックします。

Fusionでモジュールの接続を設定する際には、このクライアント IDとクライアント秘密鍵を使用します。

接続の作成手順については、Workfront モジュールの「[Connect [!DNL Workfront] to [!DNL Workfront Fusion]](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-modules#connect-workfront-to-workfront-fusion)」を参照してください。

## トラブルシューティング

**問題**: カスタムフォームが予期せずFusionで作成されたプロジェクトに添付される

**回避策**：

`categoryID`を高度なプロジェクト JSONから`project_new.categoryID`に移動します（Fusion UIの構造化フィールドを使用）。

具体的には、マッパーを次のように変更します。

```
// project_new — set just this one field via the structured UI
{
    "categoryID": "5d3a292300b69eb5d80c37e8ce6269d3"
}
```

```
// project (advanced JSON) — remove categoryID from here
{
    "aemNativeFolderTreeIDs": ["693c40280e09eb1bd4085a5e"],
    "aemNativeFolderWorkflowEnabled": "true",
    "name": "{{1.name}}",
    "templateID": "{{if(...)}}",
    "ownerID": "{{1.ownerID}}",
    "sponsorID": "{{1.ownerID}}",
    "priority": "2",
    "programID": "{{ifempty(7.ID; null)}}",
    "description": "test",
    "portfolioID": "{{ifempty(8.ID; null)}}",
    "scheduleMode": "S",
    "completionType": "AUT"
}
```

**なぜこれが機能するのか**:

1. `isCtgyIDsGive`nは`project_new.categoryID = "5d3a292300b69eb5d80c37e8ce6269d3"`を見て`temp.isCtgyIDsGiven = true`→真実→返します
2. ステップ （`getAttachedAndAttachableCategoryID`s）はスキップされます。条件は`!temp.isCtgyIDsGiven`です
3. 代わりに、この手順が実行されます：`ctgyIds = split(parameters.project_new.categoryID, ',')` → [&quot;5d3a292300b69eb5d80c37e8ce6269d3&quot;]
4. `prepareMiscActionData`は、AEM固有のすべてのフィールドに高度なプロジェクト JSONを引き続き使用し（`project_new`よりも優先）、その後`objectCategories: [{ categoryID: "5d3a292300b69eb5d80c37e8ce6269d3" }]`をオーバーレイします。意図したフォームのみがオーバーレイされ、予期しないフォームは表示されません
5. ソース OPTASKから新しいプロジェクトにカスタム フィールド値をコピーする手順は、`isCopyCustomData: true`で期待どおりに実行されます

AEM フィールド （`aemNativeFolderTreeIDs`, `aemNativeFolderWorkflowEnabled`）は、影響を受けません。 このプロセスは、`categoryID`が見つかった場所でのみ変更されます。



