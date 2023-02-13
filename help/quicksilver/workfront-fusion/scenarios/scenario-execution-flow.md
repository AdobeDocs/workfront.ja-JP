---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion のシナリオ実行フロー
description: この記事では、シナリオの実行方法と、シナリオを介したデータのフローを説明します。 また、処理されたデータに関する情報の場所と読み取り方法についても説明します。
author: Becky
feature: Workfront Fusion
exl-id: 95c6e969-66b4-4b57-9e62-aae0cfb9bf98
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 0%

---

# のシナリオ実行フロー [!DNL Adobe Workfront Fusion]

この記事では、シナリオの実行方法と、シナリオを介したデータのフローを説明します。 また、処理されたデータに関する情報の場所と読み取り方法についても説明します。

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計画*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL プラン ]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] ライセンス**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p><p>[!UICONTROL [!DNL Workfront Fusion] 自動化 (WA) </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## シナリオ実行フロー

シナリオが正しく設定され、アクティブ化されると、定義されたスケジュールに従って実行されます。

シナリオが開始すると、最初のモジュールは、監視するように設定されたイベントに応答します。 バンドル（データ）が返された場合、それらは次のモジュールに渡され、シナリオは続き、連続する各モジュールを 1 つずつ通過します。

バンドルがすべてのモジュールで正しく処理された場合、シナリオの詳細領域で成功とマークされます。詳しくは、 [シナリオの詳細 ( [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

* シナリオの設定について詳しくは、 [の基本的なシナリオ設定 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/basic-scenario-settings.md).
* シナリオの有効化について詳しくは、 [でのシナリオのアクティブ化または非アクティブ化 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).
* シナリオのスケジュールについて詳しくは、 [でのシナリオのスケジュール設定 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
* モジュールについて詳しくは、 [モジュールのタイプ](../../workfront-fusion/modules/module-types.md).

### 例： [!UICONTROL [!DNL Workfront Fusion] 自動化作業用]

>[!INFO]
>
>**例：** で受信リクエストを監視するシナリオの場合 [!DNL Workfront] を次に変換し、 [!DNL Workfront] プロジェクトの場合、データは次のようになります。
>
>最初のモジュールで実行されるシナリオの最初の手順は、リクエストを監視することです。 に含まれる各リクエストは、1 つのバンドルと見なされます。 バンドルが見つからずにモジュールが実行された場合、シナリオは最初のモジュールの後で終了します。
>
>最初のモジュールがバンドルを返した場合、バンドルは残りのシナリオを通過します。 この例では、残りのシナリオは 2 番目と最後のモジュールで構成され、このモジュールはリクエストをプロジェクトに変換します。
>
>?![](assets/example-execution-flow-wf-only-350x157.png)

### 例： [!UICONTROL [!DNL Workfront Fusion] 作業の自動化と統合]

>[!INFO]
>
>**例：** からドキュメントをダウンロードするシナリオで [!DNL Adobe Workfront] を追加し、を含むフォルダーに送信します。 [!DNL Dropbox]の場合、データは次のように流れます。
>
>最初のモジュールで実行されるシナリオの最初の手順は、バンドル（ドキュメント）を監視することです。 この例では、モジュールは内のバンドルを監視します。 [!DNL Workfront]. バンドルが返されない場合、シナリオは最初のモジュールの後で終了します。
>
>バンドルが返されると、バンドルは残りのシナリオを通過します。 この例では、残りのシナリオは 2 番目と最後のモジュールで構成され、バンドルがにアップロードされます [!DNL Dropbox] フォルダー。
>
>![](assets/example-wf-dropbox-scen-execution-flow-350x202.png)
>
>最初のモジュールが複数のバンドルを返した場合、最初のバンドルがにアップロードされます。 [!DNL Dropbox] 2 番目のバンドルがアップロードされる前に。 次に、2 番目のバンドルがアップロードされ、3 番目のバンドルがアップロードされます。

## 処理されたバンドルに関する情報

各モジュールについて、バンドルは 4 段階のプロセスを経てから次のモジュールに進むか、最後の宛先に到達します。 4 段階のプロセスは、初期化、操作、コミット/ロールバック、および確定です。 これはトランザクション処理と呼ばれ、モジュールでのデータの処理方法を説明するのに役立ちます。

シナリオの実行が完了すると、各モジュールに、実行された操作の数を示すアイコンが表示されます。 このアイコンをクリックすると、処理されたバンドルに関する詳細情報が上記の形式で表示されます。 どのモジュール設定が使用され、どのバンドルがどのモジュールから返されたかを確認できます。

![](assets/info-processed-bundles-350x396.png)

モジュールは次のような入力情報を受け取りました。

* 変換された画像
* 画像のアップロード先となる選択されたフォルダ
* 元の [!DNL Facebook] 画像

処理の後、モジュールは次の出力情報を返しました。

* 画像 ID の割り当て元 [!DNL Dropbox]
* 次の場所のフルパス： [!DNL Dropbox] [!DNL Workfront Fusion] ファイルをアップロードしました

上記の情報は、ドロップダウンボックスで示されるように、各バンドルに対して個別に取り込まれます [!UICONTROL 操作 1] および [!UICONTROL 操作 2] 画像内に表示されます。

トランザクション処理について詳しくは、 [のシナリオの実行、サイクル、フェーズ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## シナリオの実行中にエラーが発生しました

シナリオの実行中にエラーが発生する場合があります。 例えば、 [!DNL Dropbox] モジュール設定のターゲットフォルダーとして設定したフォルダーでは、シナリオが終了し、エラーメッセージが表示されます。 エラーの処理方法の詳細については、 [でのエラー処理 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).
