---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Microsoft Office 365 カレンダー
description: 内 [!DNL Adobe Workfront Fusion] シナリオの場合、Microsoft Office 365 カレンダーを使用するワークフローを自動化し、複数のサードパーティのアプリケーションやサービスに接続することができます。
author: Becky
feature: Workfront Fusion
exl-id: 814c285e-c106-458a-a0b1-760677634f4f
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1835'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Calendar]

内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Microsoft Office 365 Calendar]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。

を使用するには [!DNL Office 365 Calendar] と [!DNL Adobe Workfront Fusion]の場合、 [!DNL Office 365 Excel] アカウント 1 つは、 [www.office.com](http://www.office.com/).

Office 365 アカウントを次に接続する手順については、 [!DNL Workfront Fusion]を参照してください。 [Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順](../../workfront-fusion/connections/connect-to-fusion-general.md)

同意すると、 [!UICONTROL Workfront Fusion] シナリオの作成を続行できる管理ページです。

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画*</td>
  <td> <p>[!UICONTROL Pro] 以降</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td>
   <td> <p>[!UICONTROL プラン ]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 前提条件

使用する [!DNL Microsoft Office 365 Calendar] モジュールの場合、 [!DNL Microsoft Office 365 Calendar] アカウント

## [!DNL Microsoft Office 365 Calendar] モジュールとそのフィールド

設定時に [!DNL Microsoft Office 365 Calendar] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL Microsoft Office 365 Calendar] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [イベント](#event)
* [カレンダー](#calendar)
* [その他](#other)

### イベント

* [[!UICONTROL イベントを見る]](#watch-events)
* [[!UICONTROL イベントを検索]](#search-events)
* [[!UICONTROL イベントの取得]](#get-an-event)
* [[!UICONTROL イベントの作成]](#create-an-event)
* [[!UICONTROL イベントの更新]](#update-an-event)
* [[!UICONTROL イベントの削除]](#delete-an-event)

#### [!UICONTROL イベントを見る]

このトリガーモジュールは、選択したカレンダーでイベントが作成、更新、削除、開始または終了したときに、イベントの詳細を取得します。

>[!NOTE]
>
>イベントシリーズの削除済みのオカレンスを監視するには、 [!UICONTROL 更新時刻別] 内 [!UICONTROL イベントを見る] フィールドに入力します。 このモジュールは、削除された単一のイベントや削除されたイベントシリーズを監視しません。


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL イベントを監視 ]</td> 
   <td> <p>イベントの監視方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 作成日時別 ]</strong> </p> <p>新しいイベントを見る。</p> </li> 
     <li> <p><strong>[!UICONTROL 更新時刻別 ]</strong> </p> <p>更新されたイベントを監視します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL カレンダーグループ ID]</td> 
   <td>イベントを監視するカレンダーが含まれている [!UICONTROL カレンダーグループ ] を選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL カレンダー ]</td> 
   <td> <p>監視する特定のカレンダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フィルター ]</td> 
   <td>件名、イベント ID、本文で結果をフィルタリングするフィルター条件を設定します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td> <p>メッセージの最大数を入力 [!DNL Workfront Fusion] は、1 回のシナリオ実行サイクルで返されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL イベントを検索]

この検索モジュールは、選択したカレンダーでイベントが作成、更新、削除、開始または終了したときに、イベントの詳細を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL カレンダーグループ ID]</td> 
   <td>イベントを監視するカレンダーが含まれている [!UICONTROL カレンダーグループ ] を選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL カレンダー ]</td> 
   <td> <p>監視する特定のカレンダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フィルター ]</td> 
   <td> <p>結果をフィルタリングするフィルター条件を設定します。 次のプロパティでフィルタリングできます。</p> 
    <ul> 
     <li>[!UICONTROL 件名 ]</li> 
     <li>[!UICONTROL イベント ID]</li> 
     <li>[!UICONTROL 作成日時 ]</li> 
     <li>[!UICONTROL 最終変更日時 ]</li> 
     <li>[!UICONTROL 本文のプレビュー ]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order by]</td> 
   <td> <p>結果の並べ替え方法を選択します。</p> 
    <ul> 
     <li><strong>[!UICONTROL 件名 ]</strong>、昇順または降順</li> 
     <li><strong>[!UICONTROL 作成日時 ]</strong>、昇順または降順</li> 
     <li><strong>[!UICONTROL 最終変更日時 ]</strong>、昇順または降順</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td>イベントの最大数を入力 [!DNL Workfront Fusion] は、1 回のシナリオ実行サイクルで返されます。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL イベントの取得]

このアクションモジュールは、指定されたイベントの詳細を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL イベント ID]</td> 
   <td> <p>詳細を取得するイベントの ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL イベントの作成]

このアクションモジュールは、新しいイベントを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 件名 ]</td> 
   <td> <p>作成したイベントのタイトルを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 開始日 ]</td> 
   <td> イベントが日付と時刻の組み合わせで開始する単一の時点を入力します。 形式を使用 <code>({date}T{time}</code>;例： <code>2017-08-29T04:00:00.0000000</code>. サポートされる日付と時刻の形式の一覧については、 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">強制入力 [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 終了日 ]</td> 
   <td> イベントが日付と時間の組み合わせで終了する単一の時点を入力します。 形式を使用 <code>{date}T{time}</code>;例： <code>2017-08-29T04:00:00.0000000</code>. サポートされる日付と時刻の形式の一覧については、 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">強制入力 [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リマインダー日 ]</td> 
   <td>このイベントのリマインダーを有効にするかどうかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reminder]</td> 
   <td>リマインダーがトリガーする、イベントの開始前の分数を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 重要度 ]</td> 
   <td> <p>このイベントの重要度を選択します。</p> 
    <ul> 
     <li>[!UICONTROL 低 ]</li> 
     <li>[!UICONTROL Medium]</li> 
     <li>[!UICONTROL 高 ]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 感度 ] </td> 
   <td> <p>このイベントの感度を選択します。</p> 
    <ul> 
     <li><strong>[!UICONTROL 標準 ]</strong> </li> 
     <li> <p><strong>[!UICONTROL 個人 ]</strong> </p> <p>受信者に「[!UICONTROL Please treat this as Personal]」というメッセージが表示されます。</p> </li> 
     <li> <p><strong>[!UICONTROL プライベート ]</strong> </p> <p>受信者に「[!UICONTROL Please treat this as Private]」というメッセージが表示されます。 このイベントは、受信者の受信ボックスルールによって転送またはリダイレクトされません。</p> </li> 
     <li> <p><strong>[!UICONTROL 機密 ]</strong> </p> <p>受信者に「[!UICONTROL Please treat this as Confidential]」というメッセージが表示されます。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 本文コンテンツタイプ ]</td> 
   <td>本文のコンテンツをプレーンテキストにするか、HTMLにするかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 本文コンテンツ ]</td> 
   <td>イベントに関連付けられたメッセージの本文を入力またはマッピングします。 HTML形式またはテキスト形式で指定できます（上記の「[!UICONTROL Body Content Type]」フィールドで指定）。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Location]</td> 
   <td> <p>イベントの場所の詳細を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Response requested]</td> 
   <td>選択 <strong>[!UICONTROL はい ]</strong> ：招待者にイベントへの招待状への返信をリクエストする場合。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 表示形式 ]</td> 
   <td> <p>カレンダーを表示する人にイベントを表示する方法を選択します。</p> 
    <ul> 
     <li>[!UICONTROL 無料 ]</li> 
     <li>[!UICONTROL 仮 ]</li> 
     <li>[!UICONTROL ビジー ]</li> 
     <li>[!UICONTROL 不在 ]</li> 
     <li>[!UICONTROL 他の場所での作業 ]</li> 
     <li>[!UICONTROL 不明 ]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attendees]</p> </td> 
   <td> <p>イベントの出席者を追加します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 名前 ]</strong> </p> <p>出席者の名前を入力します。</p> </li> 
     <li> <p><strong>[!UICONTROL 電子メール ]</strong> </p> <p>出席者の電子メールアドレスを入力します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL カテゴリ ]</td> 
   <td>イベントをカレンダーに表示するカテゴリを入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL イベントの更新]

このアクションモジュールは、既存のイベントを更新します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL イベント ID]</td> 
   <td>更新するイベントの ID を入力、マッピング、または選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 件名 ]</td> 
   <td> <p>作成したイベントのタイトルを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 開始日 ]</td> 
   <td> イベントが日付と時刻の組み合わせで開始する単一の時点を入力します。 形式を使用 <code>{date}T{time}</code>;例： <code>2017-08-29T04:00:00.0000000</code>. サポートされる日付と時刻の形式の一覧については、 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">強制入力 [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 終了日 ]</td> 
   <td> イベントが日付と時間の組み合わせで終了する単一の時点を入力します。 形式を使用 <code>({date}T{time}</code>;例： <code>2017-08-29T04:00:00.0000000</code>. サポートされる日付と時刻の形式の一覧については、 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">強制入力 [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リマインダー日 ]</td> 
   <td>このイベントのリマインダーを有効にするかどうかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reminder]</td> 
   <td>リマインダーがトリガーする、イベントの開始前の分数を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 重要度 ]</td> 
   <td> <p>このイベントの重要度を選択します。</p> 
    <ul> 
     <li>[!UICONTROL 低 ]</li> 
     <li>[!UICONTROL Medium]</li> 
     <li>[!UICONTROL 高 ]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 感度 ] </td> 
   <td> <p>このイベントの感度を選択します。</p> 
    <ul> 
     <li><strong>[!UICONTROL 標準 ]</strong> </li> 
     <li> <p><strong>[!UICONTROL 個人 ]</strong> </p> <p>受信者に「[!UICONTROL Please treat this as Personal]」というメッセージが表示されます。</p> </li> 
     <li> <p><strong>[!UICONTROL プライベート ]</strong> </p> <p>受信者に「[!UICONTROL Please treat this as Private]」というメッセージが表示されます。 このイベントは、受信者の受信ボックスルールによって転送またはリダイレクトされません。</p> </li> 
     <li> <p><strong>[!UICONTROL 機密 ]</strong> </p> <p>受信者に「[!UICONTROL Please treat this as Confidential]」というメッセージが表示されます。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 本文コンテンツタイプ ]</td> 
   <td>イベントに関連付けられるメッセージの本文の内容を、プレーンテキストにするかHTMLにするかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 本文コンテンツ ]</td> 
   <td>イベントに関連付けられたメッセージの本文を入力またはマッピングします。 HTML形式またはテキスト形式で指定できます（上記の「[!UICONTROL Body Content Type]」フィールドで指定）。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Location]</td> 
   <td> <p>イベントの場所の詳細を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Response requested]</td> 
   <td>選択 <strong>[!UICONTROL はい ]</strong> ：招待者にイベントへの招待状への返信をリクエストする場合。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 表示形式 ]</td> 
   <td> <p>カレンダーを表示する人にイベントを表示する方法を選択します。</p> 
    <ul> 
     <li>[!UICONTROL 無料 ]</li> 
     <li>[!UICONTROL 仮 ]</li> 
     <li>[!UICONTROL ビジー ]</li> 
     <li>[!UICONTROL 不在 ]</li> 
     <li>[!UICONTROL 他の場所での作業 ]</li> 
     <li>[!DNL Unknown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attendees]</p> </td> 
   <td> <p>イベントの出席者を追加します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 名前 ]</strong> </p> <p>出席者の名前を入力します。</p> </li> 
     <li> <p><strong>[!UICONTROL 電子メール ]</strong> </p> <p>出席者の電子メールアドレスを入力します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL カテゴリ ]</td> 
   <td>イベントをカレンダーに表示するカテゴリを入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL イベントの削除]

このアクションモジュールは、既存のイベントを削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL イベント ID]</td> 
   <td> <p>削除するイベントの ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### カレンダー

* [[!UICONTROL カレンダーのリスト]](#list-calendars)
* [[!UICONTROL カレンダーの取得]](#get-a-calendar)
* [[!UICONTROL カレンダーの作成]](#create-a-calendar)
* [[!UICONTROL カレンダーの更新]](#update-a-calendar)
* [[!UICONTROL カレンダーの削除]](#delete-a-calendar)

#### [!UICONTROL カレンダーのリスト]

この検索モジュールは、認証済みユーザーのカレンダーのすべてのリストを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL カレンダーグループ ID]</td> 
   <td>リストに表示するカレンダーが含まれている [!UICONTROL カレンダーグループ ] を選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td>カレンダーの最大数を入力 [!DNL Workfront Fusion] は、1 回のシナリオ実行サイクルで返されます。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL カレンダーの取得]

このアクションモジュールは、1 つのカレンダーに関する詳細を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL カレンダー ID]</td> 
   <td> <p>詳細を取得するカレンダーの ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL カレンダーの作成]

このアクションモジュールは、Googleアカウントに新しいカレンダーを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL カレンダー名 ]</td> 
   <td> <p>新しいカレンダーの名前を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL カレンダーの更新]

このアクションモジュールは、既存のカレンダーを編集します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL カレンダー ID]</td> 
   <td>更新するカレンダーの [!UICONTROL カレンダー ID] を入力します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 新しいカレンダー名 ]</td> 
   <td> <p>新しいカレンダーの名前を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL カレンダーの削除]

このアクションモジュールは、既存のカレンダーを削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL カレンダー ID]</td> 
   <td>削除するカレンダーの [!UICONTROL カレンダー ] ID を入力します。</td> 
  </tr> 
 </tbody> 
</table>

### その他

#### [!UICONTROL API 呼び出しを実行する]

このモジュールでは、カスタム API 呼び出しを実行できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>相対パスを入力 <code>https://graph.microsoft.com</code>. 例:<code> /v1.0/me/events</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL メソッド ]</p> </td> 
   td&gt; <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。例： <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] によって、認証ヘッダーが追加されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL クエリ文字列 ]</td> 
   <td> <p> 標準の JSON オブジェクトの形式で、API 呼び出しのクエリを追加します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 本文 ]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文のコンテンツを追加します。</p> <p>メモ:   <p>条件文 ( <code>if</code> JSON で、条件文の外側に引用符を置きます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
