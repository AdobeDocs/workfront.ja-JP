---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: 直接インストールに使用できるスキル
description: Workfrontには、LLMに直接インストールできるスキルがいくつかあります。
author: Becky
feature: Get Started with Workfront
source-git-commit: 20f5a513d8d33ecf8770f35bc73ee799a7de939e
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 1%

---


# 直接インストールに使用できるスキル

Workfrontには、LLMに直接インストールできるスキルがいくつかあります。 適切なステップが既に組み込まれているため、これらのツールを特定のタスクにどのように使用するかをスキルがガイドします。

これらのスキルは、Adobe SkillsのGitHub リポジトリで確認できます。

>[!NOTE]
>
>現在、これらのスキルはClaudeでのみ利用可能です。
>ClaudeをAdobeで設定する方法については、Adobe Developer ドキュメントの[はじめに](https://developer.adobe.com/adobe-for-creativity/getting-started/)を参照してください。

## Workfront GitHub リポジトリからスキルをClaudeにインストールします。

1. GitHubの[Adobe Workfront スキルリポジトリ &#x200B;](https://github.com/adobe/skills/tree/main/plugins/workfront)に移動します。
1. 使用するスキルフォルダーをダウンロードします。
1. フォルダーをClaude スキルライブラリにコピーします。

   * Claude Desktop: `~/Library/Application Support/Claude/skills/` （macOS）または同等の製品。
   * クロードコード：`~/.claude/skills/`。

<!--

1. Go to the [Adobe Workfront skills repository](https://github.com/adobe/skills/tree/main/plugins/workfront) on GitHub.
1. Download the skill file you want to use.
1. In Claude, click **Customize**.
1. Select **Skills**.
1. Click **Create skill** -> **Upload a skill**.
1. Upload the zipped skill file to Claude, then click **Confirm** to install.

-->

## 現在利用可能なスキル

| スキル / フォルダーへのリンク | スキルの説明 | 次の用途で使用可能 |
|---|---|---|
| [&#x200B; プランニング ソリューション アーキテクト &#x200B;](https://github.com/adobe/skills/tree/main/plugins/workfront/skills/wf-planning-solution-architect) | Workfront Planning Workspaceをニーズに合わせて構成し、Workfront Planningに関する質問に答えます。 | クロード |
