---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Google Calendar モジュール
description: 内 [!DNL Adobe Workfront Fusion] シナリオの場合、Googleカレンダーを使用するワークフローを自動化し、それを複数のサードパーティのアプリケーションおよびサービスに接続することができます。
author: Becky
feature: Workfront Fusion
exl-id: 168e8fce-645d-4108-84b7-46a113c83f41
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '3773'
ht-degree: 0%

---

# [!DNL Google Calendar] モジュール

内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!UICONTROL Google Calendar]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。

シナリオの作成手順については、 [でのシナリオの作成 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

モジュールについて詳しくは、 [のモジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

使用する [!DNL Google Calendar] モジュールの場合、 [!DNL Google] アカウント

## [!DNL Google Calendar] モジュールとそのフィールド

設定時に [!DNL Google Calendar] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL Google Calendar] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [イベント](#events)
* [カレンダー](#calendars)
* [アクセス制御ルール](#access-control-rules)
* [イテレーター（廃止）](#iterators-deprecated)
* [その他](#other)

### イベント

* [[!UICONTROL イベントを見る]](#watch-events)
* [[!UICONTROL イベントを検索]](#search-events)
* [[!UICONTROL イベントを取得]](#get-an-event)
* [[!UICONTROL イベントの作成]](#create-an-event)
* [[!UICONTROL イベントの更新]](#update-an-event)
* [[!UICONTROL イベントの削除]](#delete-an-event)


#### [!UICONTROL イベントを見る]

このトリガーモジュールは、指定したカレンダーで新しいイベントが追加、更新、削除、開始または終了された場合に、シナリオを実行します。 このモジュールは、レコードまたはレコードに関連付けられているすべての標準フィールドと、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Calendar] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL カレンダー ] </td> 
   <td> <p>モジュールを使用するカレンダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ウォッチイベント ]</td> 
   <td> <p>イベントを「作成日」、「更新日」、「開始日」、「終了日」のどれで監視するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 削除されたイベントを表示 ]</td> 
   <td> <p>削除されたイベントを含めるには、このオプションを有効にします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL クエリ ] </td> 
   <td> <p>検索するテキストを入力します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 制限 ]</td> 
   <td> <p> イベントの最大数を設定 [!DNL Workfront Fusion] は、1 サイクル（シナリオ実行あたりの繰り返し数）で使用されます。 値が大きすぎると、指定されたサードパーティサービス側（タイムアウト）で接続が中断される場合があります。 [!DNL Workfront Fusion] これに対する影響はありません。 サイクルの最大数に対しては、値を小さく設定して大きい値を定義するか、シナリオをより頻繁に実行することをお勧めします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL イベントを検索]

このアクションモジュールは、選択したカレンダー内のイベントを検索します。

カレンダーと検索のパラメーターを指定します。

このモジュールは、イベントの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td>接続方法 [!DNL Google Calendar] Workfront Fusion へのアカウントについては、 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe Workfront Fusion への接続の作成 — 基本手順</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL カレンダー ID]</td> 
   <td> <p>検索するカレンダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 開始日 ]</td> 
   <td> <p> イベントが開始する日付を入力またはマッピングします。 また、このモジュールは、この日付より前に開始し、入力された開始日にまだ発生しているイベントを取得します。 </p> <p>サポートされる日付と時刻の形式の一覧については、 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">強制入力 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 終了日 ]</td> 
   <td> <p> イベントが終了する日付を入力またはマッピングします。 </p> <p> サポートされる日付と時刻の形式の一覧については、 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">強制入力 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 単一イベント ]</td> 
   <td> <p> このオプションを有効にすると、繰り返しイベントが単一のインスタンスとして処理されます。 例えば、週次ミーティングがあり、このオプションが有効な場合、モジュールは各週のミーティングを個別のイベントとして返します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL クエリ ]</td> 
   <td> <p>検索する検索語句を入力またはマッピングします。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Order by]</td> 
   <td> <p>結果で返されるイベントの順序を選択します。</p> 
    <ul> 
     <li><strong>[!UICONTROL 開始時間 ]</strong>:開始日時（昇順）で並べ替え。 これは、単一のイベントに対するクエリ時にのみ使用できます。</li> 
     <li><strong>[!UICONTROL 更新時間 ]</strong>:最終変更時間による並べ替え（昇順）</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 制限 ]</td> 
   <td> <p>イベントの最大数を設定 [!DNL Workfront Fusion] は、1 回の実行サイクルでを返します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL イベントを取得]

このアクションモジュールは、指定されたカレンダー内の 1 つのイベントのメタデータを返します。

カレンダーとイベントを指定します。

このモジュールは、イベントと関連するすべてのフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Calendar] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL カレンダー ID]</td> 
   <td> <p>取得するイベントが含まれるカレンダーの ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL イベント ID] </td> 
   <td> <p>既存のイベントのイベント ID を入力 [!DNL Google Calendar] イベントを設定します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL イベントの作成]

このアクションモジュールは、イベントを作成します。

イベントのカレンダーとパラメーターを指定します。

このモジュールは、イベントの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td>接続方法 [!DNL Google Calendar] Workfront Fusion へのアカウントについては、 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe Workfront Fusion への接続の作成 — 基本手順</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL イベントの作成 ]</td> 
   <td> <p>イベントの作成方法を選択します。</p> 
    <ul> 
     <li><b>[!UICONTROL 詳細 ]</b><p>このオプションを使用すると、イベントの詳細を設定できます。<br></p></li> 
     <li><b>[!UICONTROL すばやく ]</b><p>必要なのは、カレンダーを選択し、イベントの名前を入力することだけです。 名前に時間や場所の詳細を含め、 [!DNL Google Calendar] その場所と時間にイベントをスケジュールします。</p></li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL カレンダー ID]</td> 
   <td> <p>イベントを表示するカレンダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL カラー ]</td> 
   <td>イベントがカレンダーに表示する色を選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL イベント名 ]</td> 
   <td> <p> イベントの名前を入力またはマップします。 </p> <p>注意：[!UICONTROL イベントを作成 ] フィールドで [!UICONTROL クイック追加 ] を選択した場合は、イベントの日時、および [!DNL Workfront Fusion] はその日時のイベントを作成します。 例: <code>Appointment at Capitol Hill on June 3rd 10am-10:25am</code>. [!UICONTROL クイック追加 ] を選択したが、イベント名に日時を含めない場合、イベントは現在の時刻から作成され、1 時間存続します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 終日イベント ]</td> 
   <td>イベントが終日イベントの場合は、このオプションを有効にします（開始時刻と終了時刻が不要）。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 開始日 ]</td> 
   <td> <p>これが終日イベントの場合は、イベントの開始日を入力します。 </p> <p>サポートされる日付形式のリストについては、 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">強制入力 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 終了日 ]</td> 
   <td> <p> これが終日イベントの場合は、イベントの終了日を入力します。 </p> <p>サポートされる日付形式のリストについては、 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">強制入力 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 説明 ]</td> 
   <td>イベントの説明を入力またはマッピングします。 このフィールドはHTMLをサポートします。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Location]</td> 
   <td>イベントの場所をテキスト形式で入力します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL このイベントのデフォルトのリマインダー設定を使用 ]</td> 
   <td>デフォルトのリマインダー設定を使用するには、このオプションを有効にします。 [!UICONTROL Reminder] フィールドにカスタムリマインダーを設定した場合、この値は No に設定されます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reminder] </td> 
   <td> <p>イベントのリマインダーを追加します。 各リマインダーについて、リマインダーを設定するメソッドを選択し、リマインダーを設定するイベントまでの時間（分単位）を定義します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attendees]</td> 
   <td>出席者をイベントに追加します。 出席者ごとに、名前と電子メールアドレスを入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 名前を付けて表示 ]</td> 
   <td>予定表を表示している人に、このイベント中に [ 忙しい ] または [ 利用可能 ] として表示するかどうかを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 表示 ] </td> 
   <td> <p>このイベントの表示を選択します。 </p> 
    <ul> 
     <li> <p><b>[!UICONTROL デフォルト ]</b></p> <p>イベントには、カレンダー設定で設定した表示設定が含まれます。</p> </li> 
     <li> <p><b>[!UICONTROL パブリック ]</b></p> <p>カレンダーを共有している人は誰でも、このイベントを表示できます。</p> </li> 
     <li> <p><b>[!UICONTROL プライベート ]</b></p> <p>出席者のみがこのイベントを表示できます。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL イベント作成に関する通知を送信します ]</td> 
   <td> <p>すべてのゲストに対して、新しいイベントの作成に関する通知を送信するかどうかを選択します。[!DNL Google Calendar] ゲスト、または誰にも。</p> <p>ヒント：[!UICONTROL なし ] オプションは、移行の使用例にのみ使用することをお勧めします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ゲストはイベントを変更できます ]</td> 
   <td> <p>ゲストがこのイベントを変更できるようにする場合は、このオプションを有効にします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 繰り返し ]</td> 
   <td>このイベントに適用する繰り返しルールを追加します。 各ルールには、繰り返しイベント用の [!UICONTROL RRULE]、[!UICONTROL EXRULE]、[!UICONTROL RDATE] および [!UICONTROL EXDATE] 行のリストが必要です。 このフィールドでは、[!UICONTROL DTSTART] 行と [!UICONTROL DTEND] 行は使用できないことに注意してください。イベントの開始および終了時間は、「開始」フィールドと「終了」フィールドで指定します。 このフィールドは、単一のイベントまたは繰り返しイベントのインスタンスでは省略されます。 詳しくは、 <a href="https://tools.ietf.org/html/rfc5545#section-3.8.5">RFC5545</a>.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL イベントの更新]

このアクションモジュールは、既存のイベントを変更します。

カレンダーとイベント ID を指定します。

このモジュールは、イベントの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Calendar] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL カレンダー ] </td> 
   <td> <p>作業するカレンダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL イベント ID] </td> 
   <td> <p>前に作成したイベントの ID を入力 [!DNL Google Calendar] イベントを更新します。</p> </td> 
  </tr> 
 </tbody> 
</table>

目的のフィールドに新しい値を入力することで、イベント情報を更新できます。 個々のフィールドについて詳しくは、 [[!UICONTROL イベントの作成]](#create-an-event).

#### [!UICONTROL イベントの削除]

このアクションモジュールは、イベントを削除します。

カレンダーとイベント ID を指定します。

このモジュールは、イベントの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Calendar] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL カレンダー ID]</td> 
   <td> <p>削除するイベントを含むカレンダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL イベント ID]</td> 
   <td> <p> 以前に作成したイベントの ID を入力 [!DNL Google Calendar] イベントを削除します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL イベント削除に関する通知を送信します ]</td> 
   <td>イベントの削除に関する通知を、使用しないすべてのゲスト、ゲストに送信するかどうかを選択します [!DNL Google Calendar]または 1 人も含まれません。</td> 
  </tr> 
 </tbody> 
</table>

### カレンダー

* [[!UICONTROL カレンダーのリスト]](#list-calendars)
* [[!UICONTROL カレンダーの取得]](#get-a-calendar)
* [[!UICONTROL カレンダーの作成]](#create-a-calendar)
* [[!UICONTROL カレンダーの更新]](#update-a-calendar)
* [[!UICONTROL カレンダーの削除]](#delete-a-calendar)
* [[!UICONTROL カレンダーをクリア]](#clear-a-calendar)

#### [!UICONTROL カレンダーのリスト]

このアクションモジュールは、ユーザーのカレンダーリストのカレンダーを返します。

このモジュールは、カレンダーの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Calendar] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 最小アクセスロール ]</td> 
   <td> <p>ユーザーの最小アクセスロールを選択します。 モジュールは、この最小アクセスロールに基づいてカレンダーを返します。</p> 
    <ul> 
     <li><strong>[!UICONTROL 空き時間Reader]</strong>:ユーザは空き時間情報を読み取ることができる。 </li> 
     <li><strong>[!UICONTROL 所有者 ]</strong>:ユーザーは、イベントの読み取りと変更を行ったり、コントロールリストにアクセスしたりできます。 </li> 
     <li><strong>[!UICONTROLReader]</strong>:ユーザーは、非公開でないイベントを読み取ることができます。 </li> 
     <li><strong>[!UICONTROL Writer]</strong>:ユーザーはイベントの読み取りと変更をおこなうことができます。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 非表示のカレンダーを表示 ]</td> 
   <td>モジュールが返すリストに非表示のカレンダーを含めるには、このオプションを有効にします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td>カレンダーの最大数を設定 [!DNL Workfront Fusion] は、1 回の実行サイクルでを返します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL カレンダーの取得]

このアクションモジュールは、カレンダーを取得します。

取得するカレンダーの ID を指定します。

このモジュールは、レコードと関連するフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Calendar] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL カレンダー ID]</td> 
   <td> <p>取得するカレンダーを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL カレンダーの作成]

このアクションモジュールは、新しいカレンダーを作成します。

カレンダーの名前を指定します。

このモジュールは、カレンダーの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Calendar] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL カレンダー名 ]</td> 
   <td> <p> 新しいカレンダーの名前を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL カレンダーの更新]

このアクションモジュールは、カレンダーを更新します。

更新するカレンダーの ID を指定します。

このモジュールは、カレンダーの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Calendar] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL カレンダー ID]</td> 
   <td> <p>更新するカレンダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL カレンダー名 ]</td> 
   <td> <p> カレンダーの新しい名前を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL カレンダーの削除]

このアクションモジュールは、カレンダーを削除します。

削除するカレンダーの ID を指定します。

このモジュールは、カレンダーの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Calendar] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL カレンダー ID]</td> 
   <td> <p>削除するカレンダーの ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL カレンダーをクリア]

このアクションモジュールは、アカウントのプライマリカレンダーからすべてのイベントを削除します。

消去するカレンダーを含むアカウントに接続する接続を指定します。

このモジュールは、カレンダーの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Calendar] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
 </tbody> 
</table>

### アクセス制御ルール

* [[!UICONTROL アクセス制御ルールのリスト]](#list-access-control-rules)
* [[!UICONTROL アクセス制御ルールを取得する]](#get-an-access-control-rule)
* [[!UICONTROL アクセス制御ルールの作成]](#create-an-access-control-rule)
* [[!UICONTROL アクセス制御ルールの更新]](#update-an-access-control-rule)
* [[!UICONTROL アクセス制御ルールの削除]](#delete-an-access-control-rule)

#### [!UICONTROL アクセス制御ルールのリスト]

このアクションモジュールは、カレンダーのアクセス制御リストのルールを返します。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Calendar] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL カレンダー ID]</td> 
   <td> <p>取得するアクセス制御ルールを含むカレンダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td>結果の最大数を設定 [!DNL Workfront Fusion] は、1 回の実行サイクルでを返します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アクセス制御ルールを取得する]

このアクションモジュールは、アクセス制御規則のメタデータを返します。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Calendar] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL カレンダー ID]</td> 
   <td> <p>取得するアクセス制御ルールを含むカレンダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL アクセス制御ルール ID]</td> 
   <td>取得するアクセス制御ルールを選択します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アクセス制御ルールの作成]

このアクションモジュールは、新しいアクセス制御規則を作成します。

カレンダーの名前を指定します。

このモジュールは、アクセス制御ルールと関連するフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Calendar] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL カレンダー ID]</td> 
   <td> <p>アクセス制御ルールを作成するカレンダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ロール ]</td> 
   <td> <p>アクセスルールに割り当てる役割を選択します。 </p> 
    <ul> 
     <li><strong>[!UICONTROL 空き時間Reader]</strong>:ユーザは空き時間情報を読み取ることができる。 </li> 
     <li><strong>[!UICONTROL 所有者 ]</strong>:ユーザーは、イベントの読み取りと変更を行ったり、コントロールリストにアクセスしたりできます。 </li> 
     <li><strong>[!UICONTROLReader]</strong>:ユーザーは、非公開でないイベントを読み取ることができます。 </li> 
     <li><strong>[!UICONTROL Writer]</strong>:ユーザーはイベントの読み取りと変更をおこなうことができます。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL の種類 ]</td> 
   <td> <p>スコープのタイプを選択します。 </p> 
    <ul> 
     <li><strong>[!UICONTROL デフォルト ]</strong>:パブリックスコープ。 これはデフォルト値です。 </li> 
     <li><strong>[!UICONTROL ユーザー ]</strong>:範囲を 1 人のユーザーに制限します。 </li> 
     <li><strong>[!UICONTROL グループ ]</strong>:範囲をグループに制限します。 </li> 
     <li><strong>[!UICONTROL ドメイン ]</strong>:範囲をドメインに制限します。 </li> 
    </ul> <p>注意：[!UICONTROL Default] またはパブリック、スコープに付与された権限は、認証済みまたは未認証のユーザーに適用されます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 値 ]</td> 
   <td>スコープのタイプに応じて、ユーザーまたはグループの電子メールアドレス、またはドメインの名前を入力します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 通知を送信 ]</td> 
   <td> <p>アクセスの変更に関する通知を送信するには、このオプションを有効にします。 </p> <p>注意：アクセスの削除に関する通知はありません。 </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アクセス制御ルールの更新]

このアクションモジュールは、アクセス制御規則を更新します。

カレンダーの名前を指定します。

このモジュールは、アクセス制御ルールと関連するフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Calendar] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL カレンダー ID]</td> 
   <td> <p>更新するアクセス制御規則を含むカレンダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL アクセス制御ルール ID]</td> 
   <td>更新するアクセス制御規則を選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ロール ]</td> 
   <td> <p>アクセスルールに割り当てる役割を選択します。 </p> 
    <ul> 
     <li><strong>[!UICONTROL なし ]</strong>:この役割ではアクセスできません。</li> 
     <li><strong>[!UICONTROL 空き時間Reader]</strong>:ユーザは空き時間情報を読み取ることができる。 </li> 
     <li><strong>[!UICONTROL 所有者 ]</strong>:ユーザーは、イベントの読み取りと変更を行ったり、コントロールリストにアクセスしたりできます。 </li> 
     <li><strong>[!UICONTROLReader]</strong>:ユーザーは、非公開でないイベントを読み取ることができます。 </li> 
     <li><strong>[!UICONTROL Writer]</strong>:ユーザーはイベントの読み取りと変更をおこなうことができます。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 通知を送信 ]</td> 
   <td> <p>アクセスの変更に関する通知を送信するには、このオプションを有効にします。 </p> <p>注意：アクセスの削除に関する通知はありません。 </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アクセス制御ルールの削除]

このアクションモジュールは、アクセス制御規則を削除します。

カレンダーの名前を指定します。

このモジュールは、アクセス制御ルールと関連するフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Calendar] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL カレンダー ID]</td> 
   <td> <p>削除するアクセス制御ルールを含むカレンダーの ID を選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL アクセス制御ルール ID]</td> 
   <td>削除するアクセス制御ルールの ID を選択またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

### イテレーター（廃止）

この [!UICONTROL 添付ファイルを繰り返し] および [!UICONTROL 出席者を繰り返し] モジュールは非推奨（廃止予定）となりました。 添付ファイルまたは出席者を繰り返すには、 [!UICONTROL フロー制御] > [!UICONTROL 反復子] モジュール。 詳しくは、 [の Iterator モジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md)

### その他

* [[!UICONTROL API 呼び出しを実行する]](#make-an-api-call)
* [[!UICONTROL 空き時間情報の取得]](#get-freebusy-information)

#### [!UICONTROL API 呼び出しを実行する]

このモジュールでは、カスタム API 呼び出しを実行できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Google Calendar] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td>相対パスを入力 <code>https://www.googleapis.com/calendar</code>. 例: <code>/v3/users/me/calendarList</code></td> 
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

#### [!UICONTROL 空き時間情報の取得]

このアクションモジュールは、一連のカレンダーの空き時間情報を返します。

このモジュールは、カレンダーの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td>接続方法 [!DNL Google Calendar] Workfront Fusion へのアカウントについては、 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe Workfront Fusion への接続の作成 — 基本手順</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 最小時間 ]</td> 
   <td> <p> 情報を取得する間隔の開始を入力します。</p> <p> サポートされる日付と時刻の形式の一覧については、 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">強制入力 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 最大時間 ]</td> 
   <td> <p> 情報を取得する間隔の終わりを入力します。 </p> <p>サポートされる日付と時刻の形式の一覧については、 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">強制入力 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL カレンダー ]</td> 
   <td> <p>情報を取得する各カレンダーで、 <strong>追加</strong> カレンダー ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

## イベント前のシナリオのトリガー

標準の支援を受けて、トリガーの指定した時間前にシナリオをイベントに対して設定できます [!DNL Google Calendar] 電子メールのリマインダーと [!UICONTROL ウェブフック] >[!UICONTROL カスタムメールフック] モジュール。

1. 以下を使用： [!UICONTROL Google Calendar] >[!UICONTROL イベントの更新] イベントに電子メールリマインダーを追加するモジュール：

   ![](assets/trigger-scen-before-event-350x209.png)

1. 以下で始まる新しいシナリオを作成します。 [!UICONTROL ウェブフック] >[!UICONTROL カスタムメールフック] モジュール。

   1. メールフックの電子メールアドレスをコピーします。
   1. シナリオを保存し、実行します。

1. In [!DNL Gmail]、リダイレクト [!DNL Google Calendar] メールフックの電子メールアドレスに対する電子メールリマインダー：

   1. を開きます。 **[!UICONTROL [!DNL Gmail]設定]**.
   1. を開きます。 **[!UICONTROL 転送と POP/IMAP]** タブをクリックします。
   1. クリック **[!UICONTROL 転送先アドレスを追加].**
   1. コピーしたメールフックのメールアドレスを貼り付け、「 」をクリックしま&#x200B;す。**[!UICONTROL 次へ]**&#x200B;を押して確定 **[!UICONTROL 続行]** ポップアップウィンドウで、 **[!UICONTROL OK]**.

   1. In [!DNL Workfront Fusion]をクリックし、確認 E メールを受信して実行を終了する新しいシナリオに切り替えます。
   1. モジュールの上のバブルをクリックして、モジュールの出力を調べます。
   1. を展開します。 `Text` をクリックし、確認コードをコピーします。

      ![](assets/confirmation-code-350x252.png)

   1. Gmail で、編集ボックスに確認コードを貼り付け、「 」をクリックしま&#x200B;す。**[!UICONTROL 検証]**:

      ![](assets/paste-code-350x46.png)

   1. を開きます。 **[!UICONTROL フィルターとブロック済みアドレス]** タブをクリックします。
   1. クリック **[!UICONTROL 新しいフィルターの作成]**.
   1. からのすべての電子メールのフィルターを設定する `     calendar-notification@google.com` をクリックし&#x200B;、**[!UICONTROL フィルターの作成]**:
   1. 選択 **[!UICONTROL 転送先]** メールフックのメールアドレスをリストから選択します。
   1. クリック **[!UICONTROL フィルターを作成]** をクリックして、フィルターを作成します。

1. （オプション） [!DNL Workfront Fusion]、 [!UICONTROL テキストパーサー] > [!UICONTROL 一致パターン] モジュールの後 [!UICONTROL ウェブフック] >[!UICONTROL カスタムメールフック] モジュールを使用して、電子メールのHTMLコードを解析し、必要な情報を取得することができます。

   例えば、モジュールを次のように設定して、イベントの ID を取得できます。

   *パターン*: `<meta itemprop="eventId/googleCalendar" content="(?<evenitID>.*?)"/>`

   *テキスト*:この `HTML content` 次から出力された項目 [!UICONTROL ウェブフック] >[!UICONTROL カスタムメールフック] モジュール。
