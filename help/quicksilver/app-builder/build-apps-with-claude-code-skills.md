---
title: Claude Code スキルを使用したApp Builder アプリケーションの構築
description: Claude Codeの一連のスキルを使用して、セットアップとデプロイメントの手順を自分で実行するのではなく、目的を記述してカスタムのAdobe Workfront App Builder アプリケーションを構築します。
author: Becky
feature: Digital Content and Documents
hide: true
source-git-commit: 366cc4ffea48295b00389b5ee36f2df42b2c8a07
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 4%

---


# Claude Code スキルを使用したApp Builder アプリケーションの構築

スキルパッケージを使用すると、[!DNL Claude] （または、[!DNL Claude Code]や[!DNL OpenAI Codex]など、クロード形式のスキルをサポートするあらゆるAI コーディングハーネス）は、[!DNL Workfront]用のカスタム [!DNL Adobe App Builder] アプリを構築できます。 これらのツールの1つにアクセスできる場合は、開発者の経験や手動セットアップ手順を必要とせずに、目的のものを平易な英語で記述してUI拡張機能を作成できます。

Adobe App Builder を活用した Workfront UI 拡張機能を使用すると、顧客およびパートナーはカスタマイズされたユーザーエクスペリエンスを作成できます。 UI拡張機能を使用すると、組織のWorkfront エクスペリエンスを変更して、組織のニーズにより適切に対応できます。これにより、効率性を向上させ、シームレスで連続性のあるエクスペリエンスを提供し、ユーザー満足度を大幅に向上させ、組織が独自のビジョンを実現するのに役立ちます。

Workfront UI拡張機能について詳しくは、[WorkfrontとAdobe App Builderのカスタムアプリケーションの作成](/help/quicksilver/app-builder/app-builder.md)を参照してください。

## UIの拡張性スキル

UI拡張性スキルを使用すると、AI コーディングハーネスを使用して、WorkfrontでのUI拡張機能の作成を管理できます。 必要な機能を記述し、ツールの設定、[!DNL Adobe App Builder]でのプロジェクトの作成、アプリの構築、Adobe cloudへのデプロイ、Workfront内での実行など、実践的な作業を行います。 ユーザーは、自分のアクションが必要な決定またはログインがある場合にのみ、プロセスに関与します。 この記事では[!DNL Claude]を例として使用していますが、この手順は、Claude SkillsをサポートするAI コーディング ハーネスに適用されます。

## 前提条件

まず、次の項目を確認してください。

* **Claude Skills**&#x200B;をサポートする[!DNL Claude Code]などのAI コーディング ハーネス。

  Claude Skillsについて詳しくは、[ スキルとは何ですか？](https://support.claude.com/en/articles/12512176-what-are-skills)を参照してください 詳しくは、Claudeのドキュメントを参照してください。

* **スキルへのアクセス**。

  * スキルは、[https://github.com/adobe/skills/blob/main/plugins/app-builder/skills/appbuilder-workfront/SKILL.md](https://github.com/adobe/skills/blob/main/plugins/app-builder/skills/appbuilder-workfront/SKILL.md)で見つけることができます。

    このリンクが開かない場合は、管理者にアクセス権の付与を依頼してください。
  * スキルは、Adobeのパブリックスキルマーケットプレイス（[adobe/skills](https://github.com/adobe/skills)）で公開されます。 [!DNL Claude Code]で、次を実行：

    ```
    /plugin marketplace add adobe/skills
    ```

    ```
    /plugin install app-builder@adobe-skills
    ```

* 開発者の役割&#x200B;**を持つ**[!DNL Adobe App Builder] アクセス。 Adobeの組織にはApp Builder ライセンスが必要です。そのライセンスには開発者として追加する必要があります。 これは、[!DNL Claude]がAdobe Developer Consoleを開いてプロジェクトを作成できるようにするものです。

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
