---
title: Claude Code スキルを使用したApp Builder アプリケーションの構築
description: Claude Codeの一連のスキルを使用して、セットアップとデプロイメントの手順を自分で実行するのではなく、目的を記述してカスタムのAdobe Workfront App Builder アプリケーションを構築します。
author: Becky
feature: Digital Content and Documents
hide: true
source-git-commit: e5a288dcac20be9176d1541d531edaf0d8c99a8c
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 5%

---


# Claude Code スキルを使用したApp Builder アプリケーションの構築

[!DNL Claude Code] スキルのセットを使用すると、[!DNL Claude]は[!DNL Workfront]用のカスタム [!DNL Adobe App Builder] アプリを構築できます。 つまり、開発者でなくても、自分で設定ステップを記述しなくても、目的のものを平易な英語で記述して構築できます。

Adobe App Builder を活用した Workfront UI 拡張機能を使用すると、顧客およびパートナーはカスタマイズされたユーザーエクスペリエンスを作成できます。 UI拡張機能を使用すると、組織のWorkfront エクスペリエンスを変更して、組織のニーズにより適切に対応できます。これにより、効率性を向上させ、シームレスで連続性のあるエクスペリエンスを提供し、ユーザー満足度を大幅に向上させ、組織が独自のビジョンを実現するのに役立ちます。

Workfront UI拡張機能について詳しくは、[WorkfrontとAdobe App Builderのカスタムアプリケーションの作成](/help/quicksilver/app-builder/app-builder.md)を参照してください。

## ClaudeのUI拡張性スキル

[!DNL Adobe App Builder]上に構築するのは非常に技術的な場合があり、ユーザーが手順やテクニックに精通していない場合に障壁が生じる可能性があります。 UI拡張性スキルは、[!DNL Claude]を使用してこのプロセスを簡素化します。 必要な機能について説明すると、[!DNL Claude]は、ツールの設定、[!DNL Adobe App Builder]でのプロジェクトの作成、アプリの構築、Adobe cloudへのデプロイ、Workfront内での実行など、実践的な作業を行います。 ユーザーは、自分のアクションが必要な決定またはログインがある場合にのみ、プロセスに関与します。

## 前提条件

まず、次の項目を確認してください。

* **[!DNL Claude Code]**&#x200B;がインストールされました。
* **スキルへのアクセス**。

  * スキルは、[https://github.com/adobe/skills/blob/main/plugins/app-builder/skills/appbuilder-workfront/SKILL.md](https://github.com/adobe/skills/blob/main/plugins/app-builder/skills/appbuilder-workfront/SKILL.md)で見つけることができます。

    このリンクが開かない場合は、管理者にアクセス権の付与を依頼してください。
  * スキルをダウンロードしたら、次のコマンドを実行して設定します。

    ```
    /plugin marketplace add adobe/skills
    ```

    ```
    /plugin install app-builder@adobe-skills
    ```

* 開発者の役割&#x200B;**を持つ**&#x200B;[!DNL Adobe App Builder] アクセス。 Adobeの組織にはApp Builder ライセンスが必要です。そのライセンスには開発者として追加する必要があります。 これは、[!DNL Claude]がAdobe Developer Consoleを開いてプロジェクトを作成できるようにするものです。

  この前提条件が満たされているかどうかを確認するには：

  1. [Adobe Developer Console](https://developer.adobe.com/console) を開きます。
  1. 右上隅に表示されている組織が正しいことを確認します。
  1. **新しいプロジェクトを作成** > **テンプレートからプロジェクトを作成**&#x200B;をクリックします。
  1. リストに&#x200B;**App Builder**&#x200B;が表示されているかどうかを確認します。

     * リストに&#x200B;**App Builder**&#x200B;が表示されている場合は、アクセスできます。
     * **テンプレートからプロジェクトを作成** オプションがない場合、または&#x200B;**App Builder** オプションがない場合は、まだアクセスできません。 WorkfrontまたはAdobeの管理者に開発者として追加してもらい（Adobe Admin Console/ユーザー/開発者）、自社がApp Builder ライセンスを保有していることを確認します。
* **Workfront MCP サーバーは**&#x200B;に接続したので、[!DNL Claude]はデータ型、フィールド、およびコマンドを推測する代わりに実際のWorkfront APIを使用します。

  Workfront MCP サーバーが既に接続されているかどうかを確認するには、[!DNL Claude]に問い合わせます。*「Workfront MCP リソースを表示できますか？」*

  詳しくは、「[WorkfrontをClaudeに接続](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#connect-workfront-to-claude)する」を参照してください。Adobe Workfront MCP サーバーの構成に関する記事を参照してください。
