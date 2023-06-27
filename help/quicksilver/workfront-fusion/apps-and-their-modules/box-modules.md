---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: ボックスモジュール
description: 内 [!DNL Adobe Workfront Fusion] シナリオの場合、Box を使用するワークフローを自動化し、それを複数のサードパーティのアプリケーションやサービスに接続できます。 指定されたフォルダを監視して、ファイルの変更を確認したり、既存のファイルを変更および削除したり、新しいファイルをフォルダにアップロードしたりします。
author: Becky
feature: Workfront Fusion
exl-id: 965ce570-40bf-474d-b318-0d2de8be6b9d
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1070'
ht-degree: 0%

---

# ボックスモジュール

内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Box]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。 指定されたフォルダを監視して、ファイルの変更を確認したり、既存のファイルを変更および削除したり、新しいファイルをフォルダにアップロードしたりします。

シナリオの作成手順については、 [でのシナリオの作成 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). モジュールについて詳しくは、 [のモジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <td>
   <p>現在のライセンス要件：いいえ [!DNL Workfront Fusion] ライセンス要件。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] がある場合 [!DNL Adobe Workfront] プラン（組織で購入する必要がある） [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。 [!DNL Workfront Fusion] は、[!UICONTROL Ultimate] に含まれています [!DNL Workfront] プラン</p>
   <p>または</p>
   <p>従来の製品要件：組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 前提条件

使用する [!DNL Box] モジュールの場合、 [!DNL Box] アカウント

## [!DNL Box] モジュールとそのフィールド

設定時に [!DNL Box] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL Box] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### トリガー

* [[!UICONTROL 新しいイベント]](#new-event)
* [[!UICONTROL 監視ファイル]](#watch-files)

#### [!UICONTROL 新しいイベント]

このインスタントトリガーモジュールは、ファイルが追加、移動、コピー、削除、ロックまたはロック解除されたときにシナリオを開始します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>送信メッセージの監視に使用する Webhook を選択します。 ウェブフックを追加するには、 <strong>[!UICONTROL 追加 ]</strong> ウェブフックの名前と接続を入力します。</p> <p> [!UICONTROL Box] アカウントを [!UICONTROL Workfront Fusion] に接続する手順については、 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスを [!UICONTROL Workfront Fusion] に接続する</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!UICONTROL Adobe Workfront Fusion] でシナリオを作成する</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 返されるイベントの最大数 ]</p> </td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すイベントの最大数を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 監視ファイル]

このトリガーモジュールは、新しいファイルが追加されたとき、または既存のファイルが監視対象のフォルダー内で更新されたときに、シナリオを開始します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>接続方法 [!DNL Box] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  <tr> 
   <td role="rowheader">所要時間</td> 
   <td> <p>監視するファイルの種類を選択します。</p> 
    <ul> 
     <li> <p><strong>新しいファイルのみ</strong> </p> <p>新しいファイルが追加されると、シナリオが開始します。</p> </li> 
     <li> <p><strong>新規ファイルとすべての変更</strong> </p> <p>このシナリオは、ファイルが追加されたとき、またはファイルの内容やファイル属性（名前など）が変更されたときに開始されます。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>ダウンロードされたファイルの最大数</p> </td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すファイルの最大数を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

### アクション

* [[!UICONTROL アップロード] ファイル](#upload-a-file)
* [[!UICONTROL ファイルの更新]](#update-a-file)
* [[!UICONTROL ファイルの削除]](#delete-a-file)
* [[!UICONTROL ファイルの取得]](#get-a-file)

#### [!UICONTROL ファイルのアップロード]

このアクションモジュールは、ファイルをアップロードします。

ファイルを指定します。 また、ファイルの新しいファイル名を指定することもできます。

このモジュールは、ファイルの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Box] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースファイル ]</td> 
   <td> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>このモジュールが正常に動作しない場合は、次の点を考慮してください。
>
>* ファイルのサイズが、 [!DNL Box] プランを作成するか、すべての [!DNL Box] アカウントのストレージクォータ。 より多くのストレージ領域を取得するには、次の場所から既存のファイルを削除します： [!DNL Box] または、 [!DNL Box] アカウント
>* [!DNL Box] では、同じ名前の複数のファイルを 1 つのフォルダーにアップロードしません。 アップロード先のフォルダに、アップロード先のファイルと同じ名前のファイルが含まれている場合、シナリオの実行はエラーで終了します。 この問題を回避するには、ファイルの名前を変更します。 ファイルを更新する場合は、 **[!UICONTROL ファイルの更新]** モジュール。

#### [!UICONTROL ファイルの更新]

このアクションモジュールは、ファイルを更新します。

ファイルの ID を指定します。

このモジュールは、ファイルの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Box] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイル ID]</td> 
   <td>モジュールを更新するファイルの一意の ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースファイル ]</td> 
   <td> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルの削除]

このアクションモジュールは、ファイルを削除します。

ファイルの ID を指定します。

このモジュールは、ファイルの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Box] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイル ID]</td> 
   <td>モジュールを更新するファイルの一意の ID を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルの取得]

このアクションモジュールは、ファイルをダウンロードします。

ファイルの ID を指定します。

このモジュールは、ファイルの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

>[!NOTE]
>
>このモジュールは、後続のモジュールにファイルを提供する場合に役立ちます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Box] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイル ID]</td> 
   <td>モジュールを更新するファイルの一意の ID を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Possible problems</h2>
-->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">This is drafted out because we don't have a download module for Box yet</p>
-->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Watch files trigger module doesn't download a file contained in the folder.</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">There are several situations when downloading a file fails:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">The current file lock setting does not allow the file to be downloaded or the downloading of the file is disabled. In this case, the file is ignored.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">When the scenario started, the file was being uploaded to the server and was not ready to be downloaded. The scenario run gets stopped and Workfront Fusion tries downloading the file again during the next execution of the scenario.</li>
  -->
