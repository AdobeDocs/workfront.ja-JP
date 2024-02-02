---
content-type: tips-tricks-troubleshooting
product-previous: workfront;workfront-proof
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Workfront Proof マネージャー権限のトラブルシューティング
description: ' [!DNL Adobe]  Workfront でユーザーをプルーフするために使用できる権限プロファイルは、管理者、スーパーバイザー、およびマネージャーです。'
feature: Get Started with Workfront
exl-id: 913241d0-f5b0-4674-b078-9a1ad3682aff
source-git-commit: 114d306d99ae9ba0a18abd63a6137ad0568ab202
workflow-type: ht
source-wordcount: '256'
ht-degree: 100%

---

# [!UICONTROL [!DNL Workfront] Proof マネージャー]権限のトラブルシューティング

[!DNL Adobe Workfront] でプルーフユーザーに使用できる権限プロファイルは次のとおりです。

* [!UICONTROL 管理者]
* [!UICONTROL スーパーバイザ－]
* [!UICONTROL マネージャー]

<!--For detailed information about these options and how to configure them, see .-->

ユーザーに[!UICONTROL マネージャー]権限を付与する場合、次のトラブルシューティング情報を使用できます。

* **問題：**[!UICONTROL マネージャー]権限を持つユーザーは、他のユーザーが作成したプルーフを表示できません。代わりに、[!UICONTROL アクセス拒否]画面が表示されます。

  ![](assets/access-denied-350x161.png)

  **解決策：**[!UICONTROL マネージャー]権限を持つユーザーは、プルーフに明示的に追加する必要があります。プルーフは常に[!UICONTROL 詳細プルーフオプション]ウィンドウを使用して作成する必要があり、ユーザーは常にこのオプションを使用して追加する必要があります。

* **問題：**[!UICONTROL マネージャー]権限を持つユーザーは、他のユーザーが作成したプルーフにプルーフバージョンを追加できません（ドキュメントセット内のプルーフを送信する可能性はありますが、そのバージョンは別のユーザーが作成した元のセットに関連付けられません）。\
   **解決策：**[!UICONTROL マネージャー]権限を持つユーザーは、[!UICONTROL マネージャー]権限を持つユーザーが次の両方の場合にのみ、別のユーザーのプルーフにバージョンを送信できます。

   * プルーフに明示的に追加された
   * プルーフで[!UICONTROL 作成者]（プルーフの役割）として設定する

* **問題：**[!UICONTROL マネージャー]権限を持つユーザーは、自分が所有していない、または自分が作成していないプルーフに関する他のユーザーのコメントを編集することはできません。\
   **解決策：**[!UICONTROL マネージャー]権限を持つユーザーがプルーフを所有していないが、コメントを編集する必要がある場合は、そのユーザーを[!UICONTROL 作成者]（[!UICONTROL またはモデレーター]）として追加します\
   これら 3 タイプの権限は、[!DNL Workfront] で[!UICONTROL プランナー]、[!UICONTROL 作業者]、[!UICONTROL リクエスター]、[!UICONTROL レビュアー]タイプのライセンスに使用できます。[!DNL Workfront] のシステム管理者またはユーザー管理者は、そこからユーザーのプロファイルを編集し、[!DNL Workfront Proof] 権限を調整できます。
