---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Workfront Fusion を使用して、Adobe Experience Manager ワークフローを含むWorkfront プロジェクトを作成します
description: Workfront Fusion でプロジェクトを作成していて、そのプロジェクトにAdobe Experience Manager ワークフローを含める場合は、ここで説明するように、特定の Fusion モジュール設定を使用する必要があります。
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps, Workfront Fusion
exl-id: b8132d5e-234d-47f6-a09c-ca46018a2d77
source-git-commit: 6a21465ab8c92888c83344f33574302c5cc446e8
workflow-type: tm+mt
source-wordcount: '877'
ht-degree: 12%

---

# Workfront Fusion を使用して、Workfront イシューをAdobe Experience Manager ワークフローを含むプロジェクトに変換する

Workfront Fusion でプロジェクトを作成していて、そのプロジェクトにAdobe Experience Manager ワークフローを含める場合は、ここで説明するように、特定の Fusion モジュール設定を使用する必要があります。

>[!NOTE]
>
>ワークフローを使用できるのは Adobe Experience Manager as a Cloud Service 統合のみで、Adobe Experience Manager Assets Essentials との統合では使用できません。


## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table>
  <tr>
    <td><strong>Adobe Workfront パッケージ</strong></td>
   <td> <p>任意のAdobe Workfront ワークフローパッケージと任意のAdobe Workfront Automation and Integration パッケージ</p><p>WorkfrontUltimate</p><p>Workfront Fusion を追加購入したWorkfront Primeおよび Select パッケージ。</p> </td> 
  </tr>
  <tr>
   <td><strong>Adobe Workfront ライセンス</strong></td>
   <td><p>投稿者以上</p><p>リクエスト以上</p></td>
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
        <p>組織がWorkfront Automation and Integration を含まない Select またはPrime Workfront パッケージを持っている場合は、Adobe Workfront Fusion を購入する必要があります。</li></ul>
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

* Workfront 管理者は、Adobe Experience Manager 統合でワークフローを設定する必要があります。詳しくは、[Experience Manager Assets as a Cloud Service 統合の設定](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional)を参照してください。
* Adobe Experience Manager統合にリンクされたフォルダーワークフローでプロジェクトテンプレートが設定されている。
* このモジュールの接続を設定するには、Workfrontで OAuth アプリケーションを作成している必要があります。

  手順については、この記事の [OAuth アプリケーションの作成 ](#create-an-oauth-application) を参照してください。

## モジュール設定

Workfront Fusion でAdobe Experience Manager ワークフローを含むプロジェクトを作成する場合は、Workfront/その他のアクション モジュールを使用する必要があります。

1. **Workfront** / **その他のアクション** モジュールをシナリオに追加します。
1. **Connection** フィールドで、このモジュールが使用するアカウントに接続するWorkfront接続を選択します。

   接続の作成方法については、「Workfront モジュール」の [Connect [!DNL Workfront] to [!DNL Workfront Fusion]](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-modules#connect-workfront-to-workfront-fusion) を参照してください。

   クライアント ID およびクライアントシークレットの作成方法については、この記事の [OAuth アプリケーションの作成 ](#create-an-oauth-application) を参照してください。

1. 「**レコードタイプ**」フィールドで「`Issue`」を選択します。
1. 「**アクション**」フィールドで「`convertToProject`」を選択します。
1. **ID** フィールドに、プロジェクトに変換するイシューの ID を入力またはマッピングします。
1. 有効にする **詳細設定を表示**。
1. モジュールの下部までスクロールし、「**プロジェクト （詳細コレクション）**」フィールドを見つけます。
1. 次のテキストを「**プロジェクト （詳細コレクション）**」フィールドに貼り付けます。

   ```
   {
       "aemNativeFolderTreeIDs": ["Folder Tree ID here"],
       "aemNativeFolderWorkflowEnabled": "true",
       "name": "New project name here",
       "templateID": "Template ID here"
   }
   ```

1. `Folder tree ID here` をフォルダー ID に置き換えます。

   フォルダーツリー ID を見つけるには、この記事の [ フォルダーツリー ID を見つける ](#locate-folder-tree-ids) を参照してください。

   複数のフォルダーツリーを使用するには、ID をコンマで区切ります。

   `"aemNativeFolderTreeIDs": ["Folder tree ID here","Second folder tree ID here"],`
1. `New project name here` を、新しいプロジェクトに付ける名前に置き換えます。
1. `Template ID here` を、新しいプロジェクトに使用するテンプレートの ID に置き換えます。

   以前のモジュール（Workfront/検索モジュールなど）からテンプレート ID をマッピングしたり、Workfrontでテンプレートのページの URL で見つけたりできます。

1. **OK** をクリックして、モジュール設定を保存します。

## フォルダーツリー ID の検索

フォルダーツリー ID を探すには：

>[!NOTE]
>
>この手順では、Chrome ブラウザーを使用します。

1. Workfrontで、このプロジェクトに使用するテンプレートを開きます。 このテンプレートには、プロジェクトに使用するAdobe Experience Manager設定を含める必要があります。
1. ブラウザーのデベロッパーツールを開きます。
1. デベロッパーツールの「**ネットワーク**」タブを開きます。
1. 「**フィルター**」ボックスに、`object-workflow` と入力します。
1. 名前列で、表示される英数字の ID をクリックします。

   ![ フォルダー ID 1 の場所 ](assets/finding-folder-id-1.png)

1. 英数字 ID の右側にある **プレビュー** タブをクリックします。
1. 次の折りたたまれたセクションを開きます。
   1. `data`
   1. `objectWorkflow`
   1. `workflows`
   1. `enhancedLinkedFolderCreationWorkflow`
   1. `enhancedLinkedFolderCreationWorkflowConfigurations`

   各フォルダーツリーは数値で表されます。 0 （ゼロ）はリストの最初のフォルダーを表し、1 は 2 番目のフォルダーを表します。以下同様に続きます。 テンプレートにフォルダーツリーが 1 つしか含まれていない場合は、その数は 0 になります。

1. 新規プロジェクトに使用するフォルダーツリーを開きます。 `_id` フィールドの値をメモします。 複数のフォルダーツリーを使用する場合は、使用するフォルダーツリーの `_id` のフィールド値をすべてメモしておきます。

   ![ フォルダー ID 2 を検索しています ](assets/finding-folder-id-2.png)

   これらは、Fusion モジュールの `aemNativeFolderTreeIDs`Workfront **/** その他のアクション **で** 「プロジェクト（詳細コレクション」フィールドに入力する **値** す。

## OAuth アプリケーションの作成

このモジュールの接続用に、Workfrontで OAuth アプリケーションを設定する必要があります。 Fusion の特定のWorkfront接続に対して、これを行う必要があるのは 1 回だけです。

1. [ ユーザー資格情報を使用して OAuth2 アプリケーションを作成する（認証コードフロー） ](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-application-using-user-credentials-authorization-code-flow) の説明に従って、Workfrontで [!DNL Workfront] アプリケーションの作成を開始します。
1. クライアント ID とクライアント秘密鍵を安全な場所にコピーします。
1. 「**リダイレクト URI**」フィールドに以下を入力します。

   ```
   http://app.workfrontfusion.com/oauth/cb/workfront-workfront
   ```

1. 「**保存**」をクリックします。

このクライアント ID とクライアントシークレットは、Fusion でモジュールの接続を設定する際に使用します。

接続の作成方法については、「Workfront モジュール」の [Connect [!DNL Workfront] to [!DNL Workfront Fusion]](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-modules#connect-workfront-to-workfront-fusion) を参照してください。
