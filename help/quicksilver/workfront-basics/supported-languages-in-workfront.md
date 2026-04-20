---
content-type: reference
navigation-topic: get-started-with-workfront
title: Adobe Workfront でサポートされている言語
description: ブラウザーの言語設定と Workfront 内のデフォルトのメールロケールを調整することで、Adobe Workfront とWorkfront からのメールを表示する言語を変更できます。
feature: Get Started with Workfront
author: Becky
exl-id: 0b76175f-5fe2-49df-b605-68e6e66b4366
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: eb5296348c27f806dd50b997970166ebae4c97f4
workflow-type: tm+mt
source-wordcount: '964'
ht-degree: 97%

---

# Adobe Workfront でサポートされている言語

Adobe Workfront の表示言語や Workfront から送信されるメールの表示言語は、ブラウザーの言語の環境設定（組織が Adobe Admin Console に移行していない場合）、Adobe Experience Cloud プロファイルの言語の環境設定（組織が Adobe Admin Console 上にある場合）、および Workfront 内のデフォルトのメールロケールを調整することで変更できます。

Workfront の表示言語を変更するには、この記事の[言語の変更](#change-the-language)を参照してください。

Workfront の用語は、Workfront が更新されるたびに、サポート対象の言語に合わせて更新されます。

Workfront は、次の言語をサポートしています。

* 英語（en-US）
* フランス語（fr-FR）
* ドイツ語（de-DE）
* 日本語（ja-JP）
* スペイン語（es-ES）
* イタリア語（it-IT）
* ポルトガル語（pt-BR）
* 韓国語（ko-KR）
* 中国語 - 簡体字（zh-CN）
* 中国語 - 繁体字（zh-TW）

ブラウザーで Workfront を表示する際に使用する言語は、組織が Adobe Admin Console 上にない場合はブラウザーの言語設定によって、組織が Adobe Admin Console 上にある場合は Adobe Experience Cloud プロファイルの言語によって制御されます。いずれの場合も、サポートされる言語リストに表示されている言語を選択していることを確認してください。

サポートされている言語のいずれかで送信メールを表示するには、Workfront のユーザーのメールロケールまたは顧客情報の設定を変更します。\
顧客情報の設定を変更するには、Workfront 管理者である必要があります。\
顧客情報とユーザーのメールロケールの変更について詳しくは、[Workfront とユーザーのメールロケールを変更](#change-the-workfront-and-user-locales)を参照してください。

サードパーティに契約して、Workfront インターフェイスと Workfront からの送信メールを他の言語に翻訳することができます。これらの翻訳は Workfront ではサポートされておらず、上記以外の言語はサポートされていません。

>[!NOTE]
>
>インターフェイスの一部は、次の場合に未翻訳になる可能性があります。
>
>* サポートされていない言語を使用している場合、インターフェイスは英語で表示されます
>* ヘルプメニューと、そのメニューからアクセスするヘルプコンテンツは、英語で表示されます
>* ユーザーが入力したテキストは、入力した元の言語のままです。これには、以下のものが含まれますが、これらに限定されません。
>
>   * プロジェクト名
>   * タスク名
>   * イシュー名
>   * ポートフォリオ名
>   * プログラム名
>   * 承認名
>   * 説明
>   * カスタムフォーム名
>   * 時間タイプ名
>   * 費用タイプ
>   * マイルストーン
>   * カスタムタブ
>   * ステータス
>   * レポート名
>

## プルーフを使用する際にサポートされる言語の不一致

Workfront 内の web プルーフビューアは、Workfront でサポートされているほとんどの言語をサポートしています。

次の言語は、プルーフツールではサポートされていません。

* 中国語 - 繁体字（zh-TW）
* 韓国語（ko-KR）

Web プルーフビューアにアクセスするには、会社がプルーフ用ライセンスを購入する必要があります。

プルーフについて詳しくは、[プルーフ](../review-and-approve-work/proofing/proofing.md)を参照してください。

Workfront をプルーフツールでサポートされていない言語で表示する場合、web プルーフビューアは英語で表示されます。

Workfront でサポートされていない言語で Workfront Proof（スタンドアロンプルーフツール）を使用する場合、Workfront 内の web プルーフビューアは英語で表示されます。\
Workfront Proof でサポートされる言語について詳しくは、[Workfront Proof の言語設定](../workfront-proof/wp-getstarted/system-information/language-settings.md)を参照してください。

## Adobe Workfront Fusion でサポートされている言語

現在、Workfront Fusion は英語のみをサポートしています。

* Workfront Fusion のすべてのコンテンツと、Workfront Fusion に関連するヘルプコンテンツは、英語で表示されます。
* Workfront Fusion では、ユーザー入力フィールドで英語以外のテキスト文字の使用はサポートされていません。

Workfront Fusion にアクセスするには、会社が Workfront Fusion ライセンスを購入している必要があります。\
Workfront Fusion について詳しくは、[Adobe Workfront Fusion の概要](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)を参照してください。

## 言語を変更

以下の設定を変更することで、Workfront を表示する言語と送信メールの言語を変更できます。

<!--* DELETE THIS SECTION MARCH 2026 The language on your browser (for users not on the Adobe Admin Console)-->
* AEM プロファイルのプライマリ言語とセカンダリ言語（Adobe Admin Console 上にあるユーザー）
* Workfront アカウントの「顧客情報」および「ユーザーメールのロケール」設定。

選択した言語で使用可能なすべての翻訳を表示するには、Workfront のロケールとブラウザーのロケールの両方を同じ言語に設定する必要があります。

組織が Adobe Admin Console に移行されたかどうかを判断するには、Workfront を表示する際に使用する URL を確認します。

| URL | Adobe Experience | 言語コントロール |
|---|---|---|
| (CompanyName).my.workfront.com | Adobe Admin Console に移行していません | [ブラウザーの言語の変更](#change-the-browser-language) |
| experience.adobe.com | Adobe Admin Console に移行済み | [Adobe Experience Cloud の言語の変更](#change-the-adobe-experience-cloud-language) |

* [ブラウザーの言語の変更](#change-the-browser-language)
* [Adobe Experience Cloud の言語の変更](#change-the-adobe-experience-cloud-language)
* [Workfront とユーザーのメールロケールの変更](#change-the-workfront-and-user-locales)

<!--DELETE THIS SECTION MARCH 2026-->

<!--

### Change the browser language {#change-the-browser-language}

If your organization has not been migrated to the Adobe Admin Console, when you change the browser language, your Workfront interface displays in that language.   
For more information about what languages are supported by Workfront, see [Supported languages in Adobe Workfront](#supported-languages).

The browser language must be changed on an individual user basis.

See the "Help" menu for your browser for specific information about how to change the language of your browser.-->

### Adobe Experience Cloud の言語の変更

組織が Adobe Admin Console に移行済みである場合、Workfront に表示される言語は Adobe Experience Cloud のプロファイル言語によって決まります。

1. Adobe Experience Cloud ツールバーの右端にあるプロファイル写真をクリックし、「**環境設定**」をクリックします。Adobe Experience Cloud ツールバーは、メインの Workfront ツールバーのすぐ上にあります。

1. 自分の名前とメールアドレスの下の&#x200B;**プロファイル**&#x200B;で、現在選択されている言語の名前をクリックします。

1. **第 1 言語**&#x200B;と&#x200B;**第 2 言語**&#x200B;のドロップダウンで、優先する言語を選択します。第 1 言語はデフォルトの言語の選択ですが、第 2 言語は、第 1 言語が特定のアプリケーションでサポートされていない場合にのみ表示されます。

### Workfront とユーザーのメールロケールの変更 {#change-the-workfront-and-user-locales}

* [デフォルトの Workfront メールロケールを変更](#change-the-workfront-locale)
* [ユーザーのメールロケールを変更](#change-the-user-locale)

### デフォルトの Workfront メールロケールを変更 {#change-the-workfront-locale}

デフォルトの Workfront メールロケールを変更する場合は、すべての Workfront ユーザー向けに送信メッセージで使用される言語、日付、数値の形式を変更します。これらの設定は、作成するすべての新しいユーザーのデフォルトになります。

デフォルトの Workfront メールロケールを変更するには：

1. Workfront 管理者として Workfront にログインします。

{{step-1-to-setup}}

1. **システム**／**顧客情報**&#x200B;をクリックします。

1. 「**基本情報**」セクションで、**デフォルトのメールロケール**&#x200B;ドロップダウンリストをクリックして、Workfront のメールを表示する言語を選択します。

1. 「**保存**」をクリックします。

### ユーザーのメールロケールを変更 {#change-the-user-locale}

<!--


When changing your User Email Locale, you modify the language, date, and number format used in your outgoing messages. These settings override the system settings selected in the Customer Info area of Setup.-->

>[!NOTE]
>
>言語設定はAdobe プロファイルに保存され、電子メールのロケールは使用されません。 詳しくは、この記事の [Adobe Experience Cloud の言語の変更](#change-the-adobe-experience-cloud-language)を参照してください。

<!--To change your User Email Locale:

{{step1-click-main-menu}}

1. Click your user profile picture.

1. Click the More menu ![](assets/more-icon.png), then click **Edit**.

1. In the **Preferences** section, click the **Email Locale** drop-down list to select the language that you want Workfront emails to display in.

1. Click **Save Changes**.-->
