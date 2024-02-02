---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Google カレンダーモジュール
description: ' [!DNL Adobe Workfront Fusion] シナリオでは、Google Calendar を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりすることができます。'
author: Becky
feature: Workfront Fusion
exl-id: 168e8fce-645d-4108-84b7-46a113c83f41
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '3821'
ht-degree: 100%

---

# [!DNL Google Calendar] モジュール

[!DNL Adobe Workfront Fusion] シナリオでは、[!UICONTROL Google Calendar] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりすることができます。

シナリオの作成手順が必要な場合は、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md) でのシナリオの作成を参照してください。

モジュールについて詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md) のモジュールを参照してください。

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td>
  <td> <p>[!UICONTROL Pro] 以降</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td>
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件なし。</p>
   <p>または</p>
   <p>従来のライセンス要件： [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、[!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も組織で購入する必要があります。[!DNL Workfront Fusion] は [!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明されている機能を使用するには、[!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについては、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 前提条件

[!DNL Google Calendar] モジュールを使用するには、[!DNL Google] アカウントが必要です。

## [!DNL Google Calendar] モジュールとそのフィールド

[!DNL Google Calendar] モジュールを設定する際に、[!DNL Workfront Fusion] に以下のフィールドが表示されます。これらに加えて、アプリまたはサービスのアクセスレベルなどの要因に応じて、追加の [!DNL Google Calendar] フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) でモジュールから別のモジュールに情報をマッピングを参照してください。

![](assets/map-toggle-350x74.png)

* [イベント](#events)
* [カレンダー](#calendars)
* [アクセス制御ルール](#access-control-rules)
* [イテレーター（廃止）](#iterators-deprecated)
* [その他](#other)

### イベント

* [[!UICONTROL イベントを監視]](#watch-events)
* [[!UICONTROL イベントを検索]](#search-events)
* [[!UICONTROL イベントを取得]](#get-an-event)
* [[!UICONTROL イベントを作成]](#create-an-event)
* [[!UICONTROL イベントを更新]](#update-an-event)
* [[!UICONTROL イベントを削除]](#delete-an-event)


#### [!UICONTROL イベントを監視]

このトリガーモジュールは、指定したカレンダーで新しいイベントが追加、更新、削除、開始、または終了された場合に、シナリオを実行します。このモジュールは、レコードに関連付けられたすべての標準フィールドと、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Google Calendar] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar] </td> 
   <td> <p>モジュールを使用するカレンダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch Events]</td> 
   <td> <p>イベントを「作成日」、「更新日」、「開始日」、「終了日」のどれで監視するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Show deleted events]</td> 
   <td> <p>削除されたイベントを含めるには、このオプションを有効にします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query] </td> 
   <td> <p>検索するテキストを入力します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p> 1 回のサイクル中に [!DNL Workfront Fusion] が処理する結果の最大数（シナリオ実行あたりの繰り返し数）を設定します。値が大きすぎると、指定されたサードパーティサービス側で接続が中断される可能性があります（タイムアウト）。[!DNL Workfront Fusion] はこれに影響しません。より小さい値を設定し、最大サイクル数としてより大きい値を定義するか、シナリオをより頻繁に実行することをお勧めします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL イベントを検索]

このアクションモジュールは、選択したカレンダー内のイベントを検索します。

カレンダーと検索のパラメーターを指定します。

このモジュールは、イベントの ID や関連するフィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>[!DNL Google Calendar] アカウントを Workfront Fusion に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe Workfront Fusion への接続を作成 - 基本手順</a>を参照してください。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar ID]</td> 
   <td> <p>検索するカレンダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Start date]</td> 
   <td> <p> イベントが開始する日付を入力またはマッピングします。また、このモジュールは、この日付より前に開始し、入力された開始日にまだ発生しているイベントを取得します。 </p> <p>サポートされる日付と時刻の形式の一覧については、<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> での型強制を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL End date]</td> 
   <td> <p> イベントが終了する日付を入力またはマッピングします。 </p> <p> サポートされる日付と時刻の形式の一覧については、<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> での型強制を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Single events]</td> 
   <td> <p> このオプションを有効にすると、繰り返しイベントが単一のインスタンスとして処理されます。例えば、週次ミーティングがあり、このオプションが有効な場合、モジュールは各週のミーティングを個別のイベントとして返します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query]</td> 
   <td> <p>検索する検索語を入力またはマッピングします。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Order by]</td> 
   <td> <p>結果で返されるイベントの順序を選択します。</p> 
    <ul> 
     <li><strong>[!UICONTROL Start Time]</strong>：開始日時（昇順）で並べ替えます。これは、単一のイベントに対するクエリ時にのみ使用できます。</li> 
     <li><strong>[!UICONTROL Updated Time]</strong>：最終変更時間（昇順）で並べ替えます。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>[!DNL Workfront Fusion] が 1 回の実行サイクルで返すイベントの数の上限を設定します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL イベントを取得]

このアクションモジュールは、指定されたカレンダー内の 1 つのイベントのメタデータを返します。

カレンダーとイベントを指定します。

このモジュールは、イベントの ID や関連するフィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Google Calendar] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar ID]</td> 
   <td> <p>取得するイベントが含まれるカレンダーの ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event ID] </td> 
   <td> <p>取得する既存の [!DNL Google Calendar] イベントのイベント ID を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL イベントを作成]

このアクションモジュールは、イベントを作成します。

イベントのカレンダーとパラメーターを指定します。

このモジュールは、イベントの ID や関連するフィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>[!DNL Google Calendar] アカウントを Workfront Fusion に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe Workfront Fusion への接続を作成 - 基本手順</a>を参照してください。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Create an Event]</td> 
   <td> <p>イベントの作成方法を選択します。</p> 
    <ul> 
     <li><b>[!UICONTROL In Detail]</b><p>このオプションを使用すると、イベントの詳細を設定できます。<br></p></li> 
     <li><b>[!UICONTROL Quickly]</b><p>必要なのは、カレンダーを選択し、イベントの名前を入力することだけです。名前に時間や場所の詳細を含めると、[!DNL Google Calendar] がその場所と時間にイベントをスケジュールします。</p></li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar ID]</td> 
   <td> <p>イベントを表示するカレンダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Color]</td> 
   <td>イベントがカレンダーに表示する色を選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event name]</td> 
   <td> <p> イベントの名前を入力またはマッピングします。 </p> <p>メモ：「[!UICONTROL Create an event]」フィールドで [!UICONTROL Quick add] を選択した場合は、イベントの日時を含めることができ、[!DNL Workfront Fusion] によってその日時のイベントが作成されます。例：<code>Appointment at Capitol Hill on June 3rd 10am-10:25am</code>。[!UICONTROL Quick add] を選択し、イベント名に日時を含めない場合、イベントは現在の時刻から作成され、1 時間存続します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL All day event]</td> 
   <td>イベントが終日イベントの場合は、このオプションを有効にします（開始時刻と終了時刻が不要）。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Start date]</td> 
   <td> <p>これが終日イベントの場合は、イベントの開始日を入力します。 </p> <p>サポートされる日付形式のリストについては、<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> での型強制を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL End date]</td> 
   <td> <p> これが終日イベントの場合は、イベントの終了日を入力します。 </p> <p>サポートされる日付形式のリストについては、<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> での型強制を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Description]</td> 
   <td>イベントの説明を入力またはマッピングします。このフィールドでは HTML がサポートされています。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Location]</td> 
   <td>イベントの場所をテキスト形式で入力します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Use the default reminder settings for this event]</td> 
   <td>デフォルトのリマインダー設定を使用するには、このオプションを有効にします。「[!UICONTROL Reminder]」フィールドにカスタムリマインダーを設定した場合、この値は「No」に設定されます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reminder] </td> 
   <td> <p>イベントのリマインダーを追加します。各リマインダーについて、リマインダーを設定するメソッドを選択し、リマインダーを設定するイベントまでの時間（分単位）を定義します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attendees]</td> 
   <td>出席者をイベントに追加します。出席者ごとに、名前とメールアドレスを入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Show me as]</td> 
   <td>カレンダーを表示している人に、このイベント中に「忙しい」として表示するか「利用可能」として表示するかを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visibility] </td> 
   <td> <p>このイベントの表示を選択します。 </p> 
    <ul> 
     <li> <p><b>[!UICONTROL Default]</b></p> <p>イベントには、カレンダー設定で設定した表示設定が含まれます。</p> </li> 
     <li> <p><b>[!UICONTROL Public]</b></p> <p>カレンダーを共有している人は誰でも、このイベントを表示できます。</p> </li> 
     <li> <p><b>[!UICONTROL Private]</b></p> <p>出席者のみがこのイベントを表示できます。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Send notification about the event creation]</td> 
   <td> <p>新しいイベントの作成に関する通知をすべてのゲストに送信するか、[!DNL Google Calendar] を使用していないゲストに送信するか、または誰にも送信しないかを選択します。</p> <p>ヒント：[!UICONTROL None] オプションは、移行のユースケースにのみ使用することをお勧めします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Guests can modify the event]</td> 
   <td> <p>ゲストがこのイベントを変更できるようにする場合は、このオプションを有効にします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Recurrence]</td> 
   <td>このイベントに適用する繰り返しルールを追加します。各ルールには、繰り返しイベント用の [!UICONTROL RRULE]、[!UICONTROL EXRULE]、[!UICONTROL RDATE] および [!UICONTROL EXDATE] の各行のリストが必要です。[!UICONTROL DTSTART] 行と [!UICONTROL DTEND] 行は、このフィールドでは使用できません。イベントの開始時刻と終了時刻は、それぞれ「開始」フィールドと「終了」フィールドで指定します。このフィールドは、単一のイベントまたは繰り返しイベントのインスタンスでは省略されます。詳しくは、<a href="https://tools.ietf.org/html/rfc5545#section-3.8.5">RFC5545</a> を参照してください。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL イベントの更新]

このアクションモジュールでは、既存のイベントを変更できます。

カレンダーとイベント ID を指定します。

このモジュールは、イベントの ID や関連するフィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Google Calendar] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar] </td> 
   <td> <p>作業するカレンダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event ID] </td> 
   <td> <p>前に作成した更新対象の [!DNL Google Calendar] イベントの ID を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

目的のフィールドに新しい値を入力することで、イベント情報を更新できます。個々のフィールドについて詳しくは、[[!UICONTROL イベントの作成]](#create-an-event)を参照してください。

#### [!UICONTROL イベントの削除]

このアクションモジュールでは、イベントを削除します。

カレンダーとイベント ID を指定します。

このモジュールは、イベントの ID や関連するフィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Google Calendar] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar ID]</td> 
   <td> <p>削除するイベントを含むカレンダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event ID]</td> 
   <td> <p> 前に作成した削除対象の [!DNL Google Calendar] イベントの ID を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Send notification about the event deletion]</td> 
   <td>イベントの削除に関する通知をすべてのゲストに送信するか、[!DNL Google Calendar] を使用しないすべてのゲストに送信するか、または誰にも送信しないかを選択します。</td> 
  </tr> 
 </tbody> 
</table>

### カレンダー

* [[!UICONTROL カレンダーをリスト]](#list-calendars)
* [[!UICONTROL カレンダーを取得]](#get-a-calendar)
* [[!UICONTROL カレンダーを作成]](#create-a-calendar)
* [[!UICONTROL カレンダーを更新]](#update-a-calendar)
* [[!UICONTROL カレンダーを削除]](#delete-a-calendar)
* [[!UICONTROL カレンダーを消去]](#clear-a-calendar)

#### [!UICONTROL カレンダーをリスト]

このアクションモジュールは、ユーザーのカレンダーリストのカレンダーを返します。

このモジュールは、カレンダーの ID や関連するフィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Google Calendar] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Minimum access role]</td> 
   <td> <p>ユーザーの最小アクセス役割を選択します。モジュールは、この最小アクセス役割に基づいてカレンダーを返します。</p> 
    <ul> 
     <li><strong>[!UICONTROL Free Busy Reader]</strong>：ユーザーは空き時間情報を読み取ることができます。 </li> 
     <li><strong>[!UICONTROL Owner]</strong>：ユーザーはイベントの読み取りと変更を行い、コントロールリストにアクセスできます。 </li> 
     <li><strong>[!UICONTROL Reader]</strong>：ユーザーはプライベートでないイベントを読み取ることができます。 </li> 
     <li><strong>[!UICONTROL Writer]</strong>：ユーザーはイベントの読み取りと変更を行うことができます。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Show hidden calendars]</td> 
   <td>モジュールが返すリストに非表示のカレンダーを含めるには、このオプションを有効にします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>[!DNL Workfront Fusion] が 1 回の実行サイクルで返すカレンダーの数の上限を設定します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL カレンダーを取得]

このアクションモジュールは、カレンダーを取得します。

取得するカレンダーの ID を指定します。

このモジュールは、レコードの ID および関連するフィールドと共に、接続を介してアクセスされるカスタムフィールドとその値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Google Calendar] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar ID]</td> 
   <td> <p>取得するカレンダーを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL カレンダーを作成]

このアクションモジュールは、新しいカレンダーを作成します。

カレンダーの名前を指定します。

このモジュールは、カレンダーの ID や関連するフィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Google Calendar] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar name]</td> 
   <td> <p> 新しいカレンダーの名前を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL カレンダーを更新]

このアクションモジュールは、カレンダーを更新します。

更新するカレンダーの ID を指定します。

このモジュールは、カレンダーの ID や関連するフィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Google Calendar] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar ID]</td> 
   <td> <p>更新するカレンダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar name]</td> 
   <td> <p> カレンダーの新しい名前を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL カレンダーを削除]

このアクションモジュールは、カレンダーを削除します。

削除するカレンダーの ID を指定します。

このモジュールは、カレンダーの ID や関連するフィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Google Calendar] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar ID]</td> 
   <td> <p>削除するカレンダーの ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL カレンダーを消去]

このアクションモジュールは、アカウントのプライマリカレンダーからすべてのイベントを削除します。

消去するカレンダーを含むアカウントへの接続を指定します。

このモジュールは、カレンダーの ID や関連するフィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Google Calendar] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

### アクセス制御ルール

* [[!UICONTROL アクセス制御ルールをリスト]](#list-access-control-rules)
* [[!UICONTROL アクセス制御ルールを取得]](#get-an-access-control-rule)
* [[!UICONTROL アクセス制御ルールを作成]](#create-an-access-control-rule)
* [[!UICONTROL アクセス制御ルールを更新]](#update-an-access-control-rule)
* [[!UICONTROL アクセス制御ルールを削除]](#delete-an-access-control-rule)

#### [!UICONTROL アクセス制御ルールをリスト]

このアクションモジュールは、カレンダーのアクセス制御リストのルールを返します。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Google Calendar] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar ID]</td> 
   <td> <p>取得するアクセス制御ルールを含むカレンダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>[!DNL Workfront Fusion] が 1 回の実行サイクルで返す結果数の上限を設定します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アクセス制御ルールを取得]

このアクションモジュールは、アクセス制御ルールのメタデータを返します。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Google Calendar] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar ID]</td> 
   <td> <p>取得するアクセス制御ルールを含むカレンダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Access control rule ID]</td> 
   <td>取得するアクセス制御ルールを選択します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アクセス制御ルールを作成]

このアクションモジュールは、新しいアクセス制御ルールを作成します。

カレンダーの名前を指定します。

このモジュールは、アクセス制御ルールと関連するフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Google Calendar] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar ID]</td> 
   <td> <p>アクセス制御ルールを作成するカレンダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Role]</td> 
   <td> <p>アクセスルールに割り当てる役割を選択します。 </p> 
    <ul> 
     <li><strong>[!UICONTROL Free Busy Reader]</strong>：ユーザーは空き時間情報を読み取ることができます。 </li> 
     <li><strong>[!UICONTROL Owner]</strong>：ユーザーはイベントの読み取りと変更を行い、コントロールリストにアクセスできます。 </li> 
     <li><strong>[!UICONTROL Reader]</strong>：ユーザーはプライベートでないイベントを読み取ることができます。 </li> 
     <li><strong>[!UICONTROL Writer]</strong>：ユーザーはイベントの読み取りと変更を行うことができます。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type]</td> 
   <td> <p>スコープのタイプを選択します。 </p> 
    <ul> 
     <li><strong>[!UICONTROL Default]</strong>：パブリックスコープ。これはデフォルト値です。 </li> 
     <li><strong>[!UICONTROL User]</strong>：範囲を 1 人のユーザーに制限します。 </li> 
     <li><strong>[!UICONTROL Group]</strong>：範囲をグループに制限します。 </li> 
     <li><strong>[!UICONTROL Domain]</strong>：範囲をドメインに制限します。 </li> 
    </ul> <p>注意：[!UICONTROL Default]、またはパブリック、範囲に付与された権限は、認証済みまたは未認証のユーザーに適用されます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Value]</td> 
   <td>範囲のタイプに応じて、ユーザーまたはグループのメールアドレス、またはドメインの名前を入力します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Send notifications]</td> 
   <td> <p>アクセスの変更に関する通知を送信するには、このオプションを有効にします。 </p> <p>メモ：アクセスの削除に関する通知はありません。 </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アクセス制御ルールを更新]

このアクションモジュールは、アクセス制御ルールを更新します。

カレンダーの名前を指定します。

このモジュールは、アクセス制御ルールと関連するフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Google Calendar] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar ID]</td> 
   <td> <p>更新するアクセス制御ルールを含むカレンダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Access control rule ID]</td> 
   <td>更新するアクセス制御ルールを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Role]</td> 
   <td> <p>アクセスルールに割り当てる役割を選択します。 </p> 
    <ul> 
     <li><strong>[!UICONTROL None]</strong>：この役割はアクセス権を提供しません。</li> 
     <li><strong>[!UICONTROL Free Busy Reader]</strong>：ユーザーは空き時間情報を読み取ることができます。 </li> 
     <li><strong>[!UICONTROL Owner]</strong>：ユーザーはイベントの読み取りと変更を行い、制御リストにアクセスできます。 </li> 
     <li><strong>[!UICONTROL Reader]</strong>：ユーザーはプライベートでないイベントを読み取ることができます。 </li> 
     <li><strong>[!UICONTROL Writer]</strong>：ユーザーはイベントの読み取りと変更を行うことができます。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Send notifications]</td> 
   <td> <p>アクセスの変更に関する通知を送信するには、このオプションを有効にします。 </p> <p>メモ：アクセスの削除に関する通知はありません。 </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アクセス制御ルールを削除]

このアクションモジュールは、アクセス制御ルールを削除します。

カレンダーの名前を指定します。

このモジュールは、アクセス制御ルールと関連するフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Google Calendar] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar ID]</td> 
   <td> <p>削除するアクセス制御ルールを含むカレンダーの ID を選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Access control rule ID]</td> 
   <td>削除するアクセス制御ルールの ID を選択またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

### イテレーター（廃止）

[!UICONTROL 添付ファイルを反復]モジュールと[!UICONTROL 参加者を反復]モジュールは非推奨になりました。添付ファイルまたは出席者を反復するには、[!UICONTROL フロー制御]／[!UICONTROL イテレーター]モジュールを使用してください。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md) のイテレーターモジュールを参照してください。

### その他

* [[!UICONTROL API 呼び出しの実行]](#make-an-api-call)
* [[!UICONTROL 空き時間情報の取得]](#get-freebusy-information)

#### [!UICONTROL API 呼び出しの実行]

このモジュールでは、カスタム API 呼び出しを実行できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Google Calendar] アカウントを [!DNL Workfront Fusion] に接続する手順について詳しくは、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td><code>https://www.googleapis.com/calendar</code> への相対パスを入力します。例： <code>/v3/users/me/calendarList</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   td&gt; <p>API 呼び出しの設定に必要な HTTP リクエストメソッドを選択します。詳しくは、<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]</a>での HTTP リクエストメソッドを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>例えば <code>{"Content-type":"application/json"}</code> のように、標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。[!DNL Workfront Fusion] は認証ヘッダーを追加します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> API 呼び出しのクエリを標準 JSON オブジェクトの形式で追加します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文の内容を追加します。</p> <p>メモ：   <p><code>if</code> などの条件ステートメントを JSON で使用する場合は、条件ステートメントの外側に引用符を挿入します。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 空き時間情報の取得]

このアクションモジュールは、一連のカレンダーの空き時間情報を返します。

このモジュールは、カレンダーの ID や関連するフィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>[!DNL Google Calendar] アカウントを Workfront Fusion に接続する手順について詳しくは、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe Workfront Fusion への接続の作成 - 基本手順</a>を参照してください</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Minimum time]</td> 
   <td> <p> 情報を取得する間隔の開始点を入力します。</p> <p> サポートされる日付と時刻の形式の一覧について詳しくは、<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> での型強制を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximum time]</td> 
   <td> <p> 情報を取得する間隔の終了点を入力します。 </p> <p>サポートされる日付と時刻の形式の一覧について詳しくは、<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> での型強制を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendars]</td> 
   <td> <p>情報を取得する各カレンダーで、「<strong>追加</strong>」をクリックして、カレンダー ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

## イベント前のシナリオのトリガー

標準の [!DNL Google Calendar] メールリマインダーと [!UICONTROL Webhook]／[!UICONTROL カスタムメールフック]モジュールを利用して、イベントの指定時間前にシナリオをトリガーできます。

1. [!UICONTROL Google Calendar]／[!UICONTROL イベントを更新]モジュールを使用して、イベントにメールリマインダーを追加します。

   ![](assets/trigger-scen-before-event-350x209.png)

1. [!UICONTROL Webhooks]／[!UICONTROL カスタムメールフック]モジュールから新しいシナリオを作成します。

   1. メールフックのメールアドレスをコピーします。
   1. シナリオを保存し、実行します。

1. [!DNL Gmail] で、[!DNL Google Calendar] メールリマインダーをメールフックのメールアドレスにリダイレクトします。

   1. **[!UICONTROL [!DNL Gmail]設定]**&#x200B;を開きます。
   1. 「**[!UICONTROL 転送と POP/IMAP]**」タブを開きます。
   1. 「**[!UICONTROL 転送先アドレスを追加]」をクリックします。**
   1. コピーしたメールフックのメールアドレスをペーストして、「**[!UICONTROL 次へ]**」をクリックします。ポップアップウィンドウで「**[!UICONTROL 続行]**」を押して確定し、「**[!UICONTROL OK]**」をクリックします。

   1. [!DNL Workfront Fusion] で、新しいシナリオに切り替えると、確認メールを受信して実行が完了します。
   1. モジュールの上のバブルをクリックして、モジュールの出力を調べます。
   1. `Text` 項目を展開して、確認コードをコピーします。

      ![](assets/confirmation-code-350x252.png)

   1. Gmail で、編集ボックスに確認コードをペーストして、「**[!UICONTROL 検証]**」をクリックします。

      ![](assets/paste-code-350x46.png)

   1. 「**[!UICONTROL フィルターとブロック済みアドレス]**」タブを開きます。
   1. 「**[!UICONTROL 新規フィルターを作成]**」をクリックします。
   1. `     calendar-notification@google.com` から送信されるすべてのメールに対してフィルターを設定して、「**[!UICONTROL フィルターを作成]**」をクリックします。
   1. 「**[!UICONTROL 転送先]**」を選択して、メールフックのメールアドレスをリストから選択します。
   1. 「**[!UICONTROL フィルターを作成]**」をクリックして、フィルターを作成します。

1. （オプション）[!DNL Workfront Fusion] で、[!UICONTROL Webhooks]／[!UICONTROL カスタムメールフック]モジュールの後に、[!UICONTROL テキストパーサー]／[!UICONTROL 一致パターン]モジュールを追加して、メールの HTML コードを使用して必要な情報を取得します。

   例えば、モジュールを次のように設定して、イベントの ID を取得できます。

   *パターン*：`<meta itemprop="eventId/googleCalendar" content="(?<evenitID>.*?)"/>`

   *テキスト*：[!UICONTROL Webhook]／[!UICONTROL カスタムメールフック]モジュールから出力された `HTML content` 項目。
