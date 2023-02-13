---
content-type: tips-tricks-troubleshooting
product-previous: workfront;workfront-proof
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Workfront Proof Manager の権限のトラブルシューティング
description: 次に、 [!DNL Adobe] Workfrontを使用してユーザーを校正します。
feature: Get Started with Workfront
exl-id: 913241d0-f5b0-4674-b078-9a1ad3682aff
source-git-commit: ecb6928c946203b03a93cf5687fd53abf8e6a8f3
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 1%

---

# [!UICONTROL [!DNL Workfront] 配達確認マネージャー] 権限のトラブルシューティング

次に、 [!DNL Adobe Workfront] ユーザーの検証用：

* [!UICONTROL 管理者]
* [!UICONTROL スーパーバイザ－]
* [!UICONTROL マネージャー]

<!--For detailed information about these options and how to configure them, see .-->

ユーザーを許可する場合 [!UICONTROL マネージャ] 権限に関しては、次のトラブルシューティング情報を使用できます。

* **問題：** 次を持つユーザー： [!UICONTROL マネージャ] 権限は、他のユーザーが作成した配達確認を表示できません。 代わりに、 [!UICONTROL アクセス拒否] 画面

   ![](assets/access-denied-350x161.png)

   **解決策：** 次を持つユーザー： [!UICONTROL マネージャ] 権限は、配達確認に明示的に追加する必要があります。 配達確認は、常に [!UICONTROL 高度な校正オプション] ウィンドウとユーザーは、必ずこのオプションを使用して追加する必要があります。

* **問題：** 次を持つユーザー： [!UICONTROL マネージャ] 権限では、他のユーザーが作成した配達確認に配達確認のバージョンを追加できません（ドキュメントセットで配達確認を送信する可能性がありますが、バージョンが別のユーザーが作成した元のセットに接続されない可能性があります）。\
   **解決策：** 次を持つユーザー： [!UICONTROL マネージャ] 権限では、 [!UICONTROL マネージャ] 次の両方の場合の権限：

   * 配達確認に明示的に追加された
   * 設定形式 [!UICONTROL 発言者] （配達確認の役割）配達確認に関する

* **問題：** 次を持つユーザー： [!UICONTROL マネージャ] 権限は、所有していない配達確認や作成していない他のユーザーのコメントを編集できません。\
   **解決策：** 次の条件を満たすユーザー [!UICONTROL マネージャ] 権限は配達確認を所有しませんが、コメントを編集し、 [!UICONTROL 発言者] ( または [!UICONTROL モデレーター]) をクリックします。\
   次の 3 種類の権限をで使用できます。 [!DNL Workfront] 対象 [!UICONTROL プランナー], [!UICONTROL 作業者], [!UICONTROL 要求者], [!UICONTROL レビュー担当者] 「ライセンス」と入力します。 のシステム管理者またはユーザー管理者 [!DNL Workfront] ユーザーのプロファイルを編集し、 [!DNL Workfront Proof] 権限を設定します。
