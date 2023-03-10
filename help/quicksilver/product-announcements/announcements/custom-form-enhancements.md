---
title: カスタムフォームの強化
description: 22.2 リリースのカスタムフォーム管理に関する次の大幅な機能強化がおこなわれました。
author: Luke
exl-id: 81568eab-8a65-4767-b8ab-fb9353a90bb6
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 0%

---

# カスタムフォームの強化

22.2 リリースのカスタムフォーム管理に関する次の大幅な機能強化がおこなわれました。

## アセットウィジェットを追加

カスタムフォームに画像を埋め込むことができます。 これにより、よりインタラクティブで視覚的な方法でカスタムフォームユーザーとの通信が可能になります。 追加のウィジェットタイプは近日中に提供されます。

![](assets/image-in-custom-form.png)

ウィジェットを含むカスタムフォームがオブジェクトに添付されている場合、オブジェクトを操作するユーザーは、次の領域でそのフォームを表示できます。

* オブジェクトの [ 詳細 ] 領域（たとえば、プロジェクトの場合は [ プロジェクトの詳細 ] 領域）&#x200B;

   ![](assets/see-image-details-page.png)

* 新しいAdobe Workfrontエクスペリエンスのルックアンドフィール（「プロジェクトを編集」ボックスや「タスクを編集」ボックスなど）がある場合の、オブジェクトの編集ボックス&#x200B;

   ![](assets/image-see-in-edit.png)

現在、ユーザーは以下の領域でウィジェットを表示できません&#x200B;。

* リストとレポート
* ホームと概要
* 新しいAdobe Workfrontエクスペリエンスのルックアンドフィールがない場合は、オブジェクトの編集ボックス（「費用を編集」ボックスなど）
* Workfront &#x200B; Mobile アプリ

カスタムフォームにウィジェットを追加する方法について詳しくは、 [カスタムフォームでの画像や他のアセットウィジェットの追加や編集](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## カスタムフォームを複数のオブジェクトタイプに関連付ける

複数のオブジェクトタイプを任意の新しいカスタムフォームに関連付けることができます。

![](assets/new-custom-form-object-types.png)

または既存のカスタムフォーム：

![](assets/add-object-type-existing-form.png)

これにより、プロジェクト、タスク、問題、およびカスタムフォームでサポートされるその他の種類のオブジェクトで使用する単一のカスタムフォームを作成できます。

カスタムフォームとそのデータを変換後のオブジェクトに引き継ぐことができるので、問題やタスクを変換する場合は特に便利です。 様々なオブジェクトタイプに対して同じカスタムフォームの正確なコピーを作成して管理する必要がなくなり、カスタムフォームを手動でプロジェクトに追加する必要がなくなりました。

>[!INFO]
>
>**例:**
>
>誰かが内部 IT リクエスト（問題）を送信し、添付のカスタムフォームで必要な情報の詳細を提供します。
>
>このイシューを、作業を行うユーザー向けのプロジェクトに変換します。
>
>送信者の詳細を含むカスタムフォームは Issue オブジェクトと Project オブジェクトの両方の種類に関連付けられているので、変換時にカスタムフォームとその詳細のすべてがプロジェクトに引き継がれます。

>[!NOTE]
>
>変換処理が実行される場合、カスタムフォームは、変換先のオブジェクトタイプに既に関連付けられている必要があります。

アセットウィジェットをカスタムフォームに追加する手順については、 [カスタムフォームでの画像や他のアセットウィジェットの追加や編集](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

複数オブジェクトのカスタムフォームを作成または編集する際は、次の点に注意してください。

* [セクション区切りの権限オプション](#permission-options-for-section-breaks)
* [計算されたカスタムフィールドの互換性](#calculated-custom-field-compatibility)
* [カスタムフォームからオブジェクトタイプを削除する場合は注意が必要です](#caution-about-deleting-an-object-type-from-a-custom-form)

### セクション区切りの権限オプション

Issue、Task、Project、および User の各オブジェクトタイプで使用できるセクション区切り権限オプションのセットには、他のすべてのオブジェクトタイプで使用できる権限オプションのセットよりも 1 つ多くの権限オプションがあります。制限付き編集。

![](assets/section-break-permissions-limited-edit.png)

他のすべてのオブジェクトタイプ (Portfolio、ドキュメント、プログラム、費用、会社、イテレーション、請求レコード、グループ ) で使用できるセクション区切り権限のセットには、制限付き編集は含まれません。

![](assets/section-break-permissions-no-limited-edit.png)

これらの両方のグループのオブジェクトタイプに関連付けられたカスタムフォームでは、すべてのオブジェクトタイプに対して機能する、共通の断面区切り権限のセットが使用されます。 特に、制限付き編集権限オプションを使用する代わりに、この共通セットは、制限付き編集権限オプションの編集権限オプションに置き換わります。 「編集」オプションは、すべてのオブジェクトタイプと互換性があります。

カスタムフォームに既に存在する他のオブジェクトタイプとは異なる権限オプションを使用するオブジェクトタイプを関連付けると、メッセージが表示され、フォームで使用される共通の権限オプションのセットに切り替えることができます。 この変更は、セクション区切りの下にない場合でも、すべてのフィールドに適用されます。

詳しくは、 [カスタムフォームにセクション区切りを追加する](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md).

### 計算されたカスタムフィールドの互換性

複数オブジェクトのカスタムフォームで、フォームのすべての関連オブジェクトタイプ（複数のオブジェクトタイプで使用可能な {name}、{description}、{entryDate} など）で使用可能なフィールドを計算フィールドが参照する場合、データは、どのオブジェクトに関連付けても正しく計算されます。

例えば、プロジェクトとタスクの複数オブジェクトフォームがあり、{name} 式を含む計算フィールドを追加した場合、プロジェクトにフォームを追加するときにプロジェクト名が表示され、タスクにフォームを追加するときにタスク名が表示されます。

ただし、フォーム内の計算フィールドが、フォームのすべてのオブジェクトタイプと互換性がないフィールドを参照している場合は、調整を行うよう警告するメッセージが表示されます。

>[!INFO]
>
>**例：** Task オブジェクトの種類に関連付けられたカスタムフォームで、割り当て先の組み込みフィールドを参照する計算カスタムフィールドを作成します。フォームがタスクに添付されるたびに、担当の主な担当者の名前を表示するための名前：
>
>
```
>Assigned To: Name{assignedTo}.{name}
>```
>
>後で、カスタムフォームにプロジェクトオブジェクトタイプを追加します。 Project オブジェクトの種類が計算されたカスタムフィールドと互換性がないことを示す警告メッセージが表示されます。 これは、「割り当て先」フィールドがプロジェクトで使用できないためです。

この場合、次のいずれかの操作を実行できます。

* カスタムフォームから互換性のない 2 つの項目（オブジェクトタイプまたは参照フィールド）のいずれかを削除します。
* 両方の項目を保持し、ワイルドカードフィルター変数を使用します `$$OBJCODE` を IF 式の条件として使用して、「請求額」フィールドの 2 つの異なるバージョンを作成します。 これにより、フォームが関連付けられているオブジェクトの種類に関係なく、フィールドが正常に機能します。

   上記の例を使用すると、組み込みの割り当て先はありませんが、次のようになります。プロジェクトの「名前」フィールドには、組み込みの「所有者」フィールドがあります（手動で変更しない限り、プロジェクトを作成した人の名前が自動的に入力されます）。 そのため、カスタムの「請求」フィールドで、 `$$OBJCODE` 以下に示すように、カスタムフォームがプロジェクトに添付され、「割り当て先」が次の場合に「所有者」フィールドを参照します。フォームがタスクに添付される際の名前フィールド：

   ```
   IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})
   ```

>[!NOTE]
>
>  フィールド名の前にオブジェクトタイプを追加すると、そのオブジェクトはオブジェクトの親オブジェクトを参照するので、 `{project}.{name}` プロジェクトで使用できますが、タスクで使用できます。

計算カスタムフィールドをカスタムフォームに追加する手順については、 [計算データをカスタムフォームに追加する](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

次のような変数について詳しくは、 `$$OBJCODE`を参照してください。 [ワイルドカードフィルター変数](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

### カスタムフォームからオブジェクトタイプを削除する場合は注意が必要です

カスタムフォーム上のオブジェクトタイプはいつでも削除できますが、削除する場合は注意が必要です。 ユーザーが既に、削除する種類のオブジェクトにカスタムフォームを添付し、データを追加している場合、フォーム上でそのオブジェクトの種類を削除すると、そのデータは完全に削除されます。

また、カスタムフォームを使用しているユーザーに対して、削除されたことを通知する通知システムはありません。

詳しくは、 [システムからカスタムフィールドまたはウィジェットを削除する](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md).
