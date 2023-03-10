---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: でのカスタムフィールドの作成と管理 [!DNL Workfront Proof]
description: Select または Premium [!DNL Workfront] この機能を使用するにはプランが必要です。 利用可能な様々なプランの詳細については、「 Workfront Plans 」を参照してください。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 87c8aff7-b638-4d14-9c5a-7e316f1ec608
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '988'
ht-degree: 0%

---

# でのカスタムフィールドの作成と管理 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品の機能について説明します [!DNL Workfront Proof]. 内部での検証に関する情報 [!DNL Adobe Workfront]を参照してください。 [校正](../../../review-and-approve-work/proofing/proofing.md).

Select または Premium [!DNL Workfront] この機能を使用するにはプランが必要です。 利用可能な様々なプランについて詳しくは、 [Workfront Plans](https://www.workfront.com/plans).

カスタムフィールドを使用すると、新しい配達確認、新しいユーザーまたは新しいゲストを作成する際に、追加のデータを取り込むことができます。

たとえば、新しい配達確認を作成するユーザーには、「製造オーダー番号」、「部門コード」または「仕入先参照」を取り込むための追加のセクションを含める必要があります。

>[!NOTE]
>
>* また、カスタムフィールドを使用して新しい配達確認ページでこのタイプの情報を取り込むと、配達確認名の長さを短くすることもできます。これは、名前に含める必要がないためです。 新しい配達確認ページについて詳しくは、「 [!DNL Workfront Proof].&quot;
>
>配達確認、ユーザー、または連絡先でカスタムフィールドが使用されると、そのフィールドを削除したり、フィールドタイプを編集したりすることはできません。 ただし、 [!UICONTROL カスタムフィールド設定] ページ ) を使用して、新しい項目に使用されないようにします。
>
>カスタムフィールドセクションを非表示にすると、個々のフィールドが表示可能に設定されている場合でも、セクション内のすべてのフィールドは非表示になります。

この記事では、次の操作方法について説明します。

## カスタムフィールドの作成

まず、カスタムフィールドを追加する「カスタムフィールド」セクションを設定する必要があります。

1. クリック **[!UICONTROL 設定]** >**[!UICONTROL アカウント設定]**&#x200B;をクリックし、 **[!UICONTROL カスタムフィールド]** タブをクリックします。

1. クリック **[!UICONTROL カスタムフィールドセクションを追加]** 関連するモジュール（配達確認、ユーザー、連絡先）内で使用する必要があります。
1. タイプ a **名前** カスタムフィールドセクションの場合は、 **[!UICONTROL 保存]**.

   次に、セクション内でカスタムフィールドを設定できます。

1. 次をクリック： **[!UICONTROL カスタムフィールド設定]** タブでページを更新します。
1. 新しいカスタムフィールドセクションの名前をクリックして、 **[!UICONTROL カスタムフィールド] セクション** 新しいセクション用のページ。
1. 次をクリック： **[!UICONTROL 新しいカスタムフィールド]** 右上隅付近にある
1. 内 **[!UICONTROL 新しいカスタムフィールド]** 表示されるページで、カスタムフィールドの詳細を指定します。

   | **必須** | Workfrontでは、ユーザーがフィールドに入力する必要があります。 |
   |---|---|
   | **検索可能** | ユーザーがカスタムフィールドデータを検索して項目を検索できるようにします。 |
   | **非表示** | カスタムフィールドを [!UICONTROL 新しい配達確認]、新規ゲスト、 [!UICONTROL 新しいユーザー] ページ |

   {style=&quot;table-layout:auto&quot;}

1. 「**[!UICONTROL 保存]**」をクリックします。
1. 内 **カスタムフィールド** 表示されるページで、 **[!UICONTROL カスタムフィールド設定]** タブでページを更新します。

1. フィールドの設定をさらに変更します。

   * 「 **[!UICONTROL 詳細]** （3 ドット）メニューを使用してカスタムフィールドのセクション名の右に移動し、 **[!UICONTROL セクションを非表示]** または **[!UICONTROL セクションを表示]**.

   * カスタムフィールドの表示/非表示を切り替えるには、 **[!UICONTROL 詳細]** （3 ドット）メニューを使用してカスタムフィールドのセクション名の右に移動し、 **[!UICONTROL カスタムフィールドを非表示]** または **[!UICONTROL カスタムフィールドを表示]**.

   * フィールド名の右側に表示される上下の矢印を使用して、フィールドの順序を変更します（セクションに複数のフィールドを追加した場合）。

1. を開きます。 **[!UICONTROL 表示ルール]** タブをクリックします。\
   表示ルールを使用すると、最初のカスタムフィールドの入力に基づいて、追加のフィールドを表示するかどうかを指定できます。 例えば、依存フィールドが A で、制御フィールドが X の場合、フィールド A はフィールド X が入力された場合にのみ表示されます。

   制御値を使用して、制御フィールドの値を決定できます。選択した場合、依存フィールドが表示されます。 例えば、依存フィールドが A で、制御フィールドが X で、X の制御値をオプション 1 と 2 のみに設定したとします。 つまり、フィールド A はフィールド X オプション 1 または 2 が選択された場合にのみ表示されます。 つまり、X のオプション 3 または 4 が選択されている場合、A のフィールドは表示されません。 を開きます。 **[!UICONTROL 表示ルール]** タブをクリックします。

   表示規則を追加するには：

   1. クリック **[!UICONTROL 新しい表示ルール]** を設定します。
   1. ルールの設定を選択し、「 **[!UICONTROL 保存]**.

1. を開きます。 **[!UICONTROL 依存関係ルール]** タブをクリックします。

   依存関係ルールを使用すると、制御フィールドで特定のオプションが選択された場合に、依存フィールドで使用できるオプションを決定できます。 例えば、依存フィールドが「B」で、制御フィールドが「Y」の場合、次のように設定できます。

   フィールド Y のオプション 1 を選択した場合は、フィールド B のオプション 1 と 2 のみが表示されます。

   フィールド Y のオプション 2 を選択した場合、フィールド B のオプション 3 と 4 のみが表示されます。

   依存関係ルールを追加する手順は、次のとおりです。

   1. クリック **[!UICONTROL 新しい依存関係ルール]** を設定します。
   1. 依存関係の設定を選択し、 **[!UICONTROL 保存]**.

## カスタムフィールドの管理

カスタムフィールドセクションまたは個々のカスタムフィールドの詳細を表示および編集できます。

1. クリック **[!UICONTROL 設定]** >**[!UICONTROL アカウント設定]**&#x200B;をクリックし、 **[!UICONTROL カスタムフィールド]** タブをクリックします。

1. カスタムフィールドセクションまたは個々のカスタムフィールドの名前をクリックします。
1. （条件付き）カスタムフィールドセクションを管理している場合、 **[!UICONTROL カスタムフィールドセクション]** ページ：

   * セクションの名前を編集します。
   * 別のモジュールに移動します。
   * セクションを表示/非表示にします。

1. （条件付き）カスタムフィールドを管理している場合、 **[!UICONTROL カスタムフィールド]** ページ：

   * フィールドを別のセクションに移動します。
   * フィールドの名前を編集します。
   * ヘルプテキストを入力します（フィールドセクションの横に疑問符アイコンが表示され、カーソルを合わせるとテキストが表示されます）。
   * を有効/無効にします。 **[!UICONTROL 必須]** を設定します。
   * を有効/無効にします。 **[!UICONTROL 検索可能]** を設定します。
   * フィールドの表示/非表示を切り替えます。
   * フィールドタイプを編集します。
   * フィールドのデフォルト値を設定または編集します。
   * 表示と依存関係ルールを設定します（上記の手順 11 および 12 で説明）。
