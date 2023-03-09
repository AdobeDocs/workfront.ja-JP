---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: レガシーフォームビルダーを使用したカスタムフォームへのカスタムフィールドの追加
description: カスタムフォームを使用している場合、新しいカスタムフィールドを作成してカスタムフォームに追加できます。 また、別のカスタムフォームに既に追加されているカスタムフィールドを追加することもできます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3579ae0f-1d2e-4ff5-bbdf-58fdd20d01d7
source-git-commit: e02e28d9a62a6bafbe19de7e6fda043b56210cf7
workflow-type: tm+mt
source-wordcount: '2208'
ht-degree: 2%

---

# レガシーフォームビルダーを使用したカスタムフォームへのカスタムフィールドの追加

カスタムフォームを使用している場合、新しいカスタムフィールドを作成してカスタムフォームに追加できます。

また、別のカスタムフォームに既に追加されているカスタムフィールドを追加することもできます。 手順については、 [カスタムフォームでカスタムフィールドまたはウィジェットを再利用する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

カスタムフィールドの追加と同様のプロセスである、カスタムフォームにアセットウィジェットを追加する方法について詳しくは、 [カスタムフォームでのアセットウィジェットの追加または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

>[!NOTE]
>
>多数のカスタムフィールドを含むカスタムフォームや、カスタムフィールドで多数の複数選択オプションを使用する場合、ユーザーは、これらのフィールドの値を追加または変更する際にパフォーマンスが低下する可能性があります。 例えば、100 個のカスタムフィールドを含むフォームや、200 個を超えるオプションを含む複数選択カスタムフィールドを使用すると、ユーザーが操作する際に時間がかかる場合があります。

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td>計画</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>カスタムフォームへの管理アクセス</p> <p>Workfront管理者がこのアクセス権を付与する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定の領域に対する管理者アクセス権をユーザーに付与する</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスタイプ、アクセスレベル設定を確認するには、Workfront管理者に問い合わせてください。

## カスタムフォームにカスタムフィールドを追加する

1. カスタムフォームの作成または編集を開始します ( [カスタムフォームの作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. を開きます。 **フィールドを追加** タブをクリックします。

   ![](assets/add-a-field.jpg)

1. を使用 **新規フィールド** ![](assets/new-field.jpg) 「 」を選択した場合、次のいずれかのフィールドタイプを選択します。

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">一行のテキストフィールド</td> 
      <td>ユーザーがフィールドに 1 行のテキストを入力できるようにします。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">段落テキストフィールド</td> 
      <td>ユーザーがフィールドに複数行のテキストを入力できるようにします。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">書式付きテキスト フィールド</td> 
      <td>フィールドに複数行のテキストを入力し、太字、斜体、下線、箇条書き、段落番号、ハイパーリンク、ブロック引用符でテキストを書式設定できます。 これは、Workfrontオブジェクトの「ホーム」、「更新」領域、リストおよび「詳細」領域で使用できます。 文字数の上限を 15,000 に設定すると、多くのテキストと書式を設定できます。</p> <p>API を使用したこのフィールドへのアクセスについて詳しくは、 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/rich-text-field-storage-in-the-api.md" class="MCXref xref">API のリッチテキストフィールドストレージ</a>.</p> <p><b>注意</b>:書式を持つテキストフィールドは、Workfrontモバイルアプリでは使用できません（今後のリリースで利用できます）。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ドロップダウン</td> 
      <td>ドロップダウンの選択肢のリストを提供します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">先行入力 </td> 
      <td>ユーザーがWorkfrontに存在するオブジェクトの名前を入力できるようにします。 ユーザーが入力を開始すると、候補のリストが表示されます。
      このフィールドタイプでは、次のオブジェクトがサポートされます。
      <ul><li>ユーザー</li>
      <li>グループ</li>
      <li>担当業務</li>
      <li>ポートフォリオ</li>
      <li>プログラム</li>
      <li>プロジェクト</li>
      <li>チーム</li>
      <li>テンプレート</li>
      <li>会社</li>
      </ul>      
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">計算済み</td> 
      <td>式を定義し、結果をカスタムフォームに表示できます。 詳しくは、 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">計算データをカスタムフォームに追加する</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">日付</td> 
      <td>ユーザーが日時を選択できるカレンダーを表示します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">チェック ボックス</td> 
      <td>ユーザーが複数選択できるようにします。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ラジオ ボタン</td> 
      <td>ユーザーが 1 つの選択肢のみを選択する必要があります。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">説明テキスト</td> 
      <td>Workfrontの外部のページに手順とリンクを含めることができます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">セクション区切り</td> 
      <td>セクション区切りは、実際にはフィールドではありません。 セクション区切りを使用して、カスタムフィールドとウィジェットをセクションに整理し、必要に応じて、セクションごとに異なる表示および編集権限を設定できます。 セクション区切りの追加と設定については、 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md" class="MCXref xref">カスタムフォームにセクション区切りを追加する</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. の **フィールド設定** 「 」タブで、追加するカスタムフィールドのタイプに使用できるオプションを設定します。

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">ラベル</td> 
      <td> <p>（必須）カスタムフィールドの上に表示する説明的なラベルを入力します。 ラベルはいつでも変更できます。</p> <p><b>重要</b>:このラベルでは特殊文字を使用しないでください。 レポートでは正しく表示されません。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">名前</td> 
      <td> <p>（必須）カスタムフィールドをWorkfront全体の様々な領域（レポート、ホーム、API の操作など）に追加したとき、この名前は、カスタムフィールドを識別する方法です。</p> <p>初めてカスタムフィールドを設定し、ラベルを入力すると、「名前」フィールドが自動的に設定され、それに一致するようになります。 ただし、「ラベル」フィールドと「名前」フィールドは同期されません。これにより、システムで表示される名前を変更することなく、ユーザーに表示されるラベルを自由に変更できます。</p> 
      <p><b>重要</b>:   
      <ul> 
      <li>これは可能ですが、他のユーザーがWorkfrontでカスタムフォームを使用し始めた後は、この名前を変更しないことをお勧めします。 その場合、Workfrontの他の領域で参照される可能性のあるカスタムフィールドが認識されなくなります。 <p>例えば、カスタムフィールドをレポートに追加し、後で名前を変更した場合、Workfrontはレポート内のフィールドを認識せず、新しい名前でレポートに再追加しない限り、正しく機能しなくなります。</p> </li>
      <li> <p>組み込みのWorkfrontフィールドに既に使用されている名前は入力しないことをお勧めします。</p> </li>
      <li><p>Workfrontの様々な領域でフィールドを使用する際にエラーが発生しないよう、カスタムフィールド名にはピリオド (.) やドット (.) を使用しないことをお勧めします。</p></li>
      </ul> <p>各カスタムフィールド名は、組織のWorkfrontインスタンス内で一意である必要があります。 これにより、既に作成済みのものを別のカスタムフォームに再利用できます。 詳しくは、 <a href="#Add" class="MCXref xref">カスタムフォームにカスタムフィールドを追加する</a> 」を参照してください。</p> </td>
     </tr> 
     <tr> 
      <td role="rowheader">指示</td> 
      <td> <p>カスタムフィールドに関する追加情報を入力します。 カスタムフォームに入力する際に、疑問符アイコンの上にマウスポインターを置くと、ここに入力した情報を含むツールヒントが表示されます。</p> 
      <p> <img src="assets/custom-field-tooltip.png"> </p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">形式</td> 
      <td> <p>カスタムフィールドに取り込むデータのタイプを選択します。</p> <p><b>メモ</b>:   
        <ul> 
         <li>フォームを保存した後は、このフィールドを編集できません。 数学計算でフィールドを使用する場合は、必ず「数値」または「通貨」フォーマットを選択してください。<br></li> 
         <li>「数値」または「通貨」を選択すると、0 から始まる数値が自動的に切り捨てられます。</li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">表示タイプ</td> 
      <td>（ドロップダウン、チェックボックス、ラジオボタンのみ）フィールドに必要なオプション選択のタイプを切り替えます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">サイズ</td> 
      <td>（テキストフィールドのみ）フィールドの幅を選択します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">時刻の表示</td> 
      <td>（日付フィールドのみ）日付と共にフィールドに表示する場合は、このオプションを選択します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">参照オブジェクト タイプ</td> 
      <td> <p>（Typeahead フィールドのみ）フィールドに関連付けるオブジェクトの種類を選択します。</p> <p>[ 適用 ] または [ 保存して閉じる ] をクリックした後は、フィールドのオブジェクトの種類を変更できません。</p> <p><b>メモ</b>:   
        <ul> 
         <li>Workfront管理者がWorkfrontユーザーインターフェイスでPortfolio、プログラムまたはプロジェクトの名前をカスタマイズした場合、オブジェクトのデフォルトのWorkfront名がこのドロップダウンリストに表示され、カスタマイズされた名前は表示されません。 詳しくは、Workfront管理者にお問い合わせください。<br></li> 
         <li>次のオブジェクトタイプは、iOSおよび Android Workfront Mobile アプリでサポートされています。ユーザー、会社、グループ、ジョブの役割、Portfolio、プログラム、プロジェクト、テンプレート。</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">フィルターの追加</td> 
      <td> <p>（先読みフィールドのみ）オブジェクトタイプにフィルターを追加して、ユーザーがフィールドを使用する際に選択できるオブジェクトを制限します。 </p> <p>例えば、次の条件を満たすユーザー名のみを選択できるようにフィールドを制限できます。</p> 
       <ul> 
        <li>ユーザーが指定した 1 つ以上のグループに属している</li> 
        <li>指定した役割または職位に関連付けられます</li> 
        <li>フィールドを使用するユーザーと同じグループに属しています</li> 
       </ul> <p>テキストモードの構文を使用して、選択したオブジェクトタイプのフィルタを定義する必要があります。 テキストモードを使用したフィルターの作成について詳しくは、 <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md#editing2" class="MCXref xref">フィルターでのテキストの編集モード</a> 記事内 <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md" class="MCXref xref">テキストモードの概要</a>. </p> <p><b>メモ</b>:   
        <ul> 
         <li>既存のカスタムフォームを編集している場合、Typeahead フィールドにフィルターを追加しても、ユーザーがフィールドを使用して既に追加したオブジェクトは削除されません（フィルターの範囲外）。</li> 
         <li>このフィルターは、モバイルデバイスでは使用できません。 Typeahead フィールドにフィルターを使用すると、このフィールドは、フィルターの影響を受けないユーザーのモバイルデバイスに表示されます。</li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">説明テキスト</td> 
      <td>（説明テキストフィールドのみ）カスタムフォーム上の手順やリンクを提供するために表示するテキストを入力します。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ハイパーリンク</td> 
      <td>（説明テキストフィールドのみ）入力した説明テキストにハイパーリンクを適用する場合は、ここに追加します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">必須フィールドの作成</td> 
      <td>ユーザーがカスタムフォームに入力するためにフィールドを必須にする場合は、このオプションを選択します。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">更新フィードでフィールドの変更を追跡</td> 
      <td><p>ドロップダウンリストをクリックし、フィールドの値の変更を自動的に追跡するオブジェクトタイプを選択します。</p> 
      <p><b>注意</b>:このオプションは、次の場合は使用できません。</p> 
      <ul> 
      <li>次のオブジェクトタイプに関連付けられたカスタムフォーム：費用、会社、反復、請求レコード、グループ。</li> 
      <li>次のフィールドタイプを指定します。計算済み、説明テキストおよびセクション区切り</li> 
      </ul>
      <p><b>重要</b>:ここでオブジェクトタイプの選択または選択解除を行うと、選択したオブジェクトタイプに関連付けられ、このフィールドを含むすべてのカスタムフォームに影響します。 例えば、ここでオブジェクトタイプの選択を解除し、カスタムフォームを保存すると、フィールドを含むカスタムフォームでは、そのオブジェクトタイプに対するフィールドの値の変更は追跡されなくなります。</p>
       <p>ここでフィールドのオブジェクトタイプを選択し、カスタムフォームを保存すると、そのフィールドが「セットアップ」の「フィードを更新」領域にある「カスタムフィールド」タブに表示されます。</p> 
       <p>逆に、セットアップの「フィードを更新」領域でこのフィールドを削除した場合、この設定のオブジェクトタイプは、オブジェクトタイプに関連付けられ、このフィールドを含むすべてのカスタムフォームで選択解除されます。</p> 
       <p>詳しくは、 <a href="../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md#adding-fields-to-the-update-feeds" class="MCXref xref">Workfrontで追跡するフィールドを追加します</a> 記事内 <a href="../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md" class="MCXref xref">システム更新の構成</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ロジックの追加</td> 
      <td>ユーザーが既存のフィールドで行った選択に基づいて、フォームに表示するフィールドを指定します。 詳しくは、 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">表示ロジックの追加とカスタムフォームへのロジックのスキップ</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">選択肢 </td> 
      <td> <p>( ドロップダウン、チェックボックス、ラジオボタンのみ。オプション )</p> 
       <ol> 
        <li> <p>クリック <b>オプション</b>次のいずれかを有効にします。</p> 
           <ul> 
            <li><strong>値を表示</strong>:各選択の値をフィールドに表示します。 各選択のラベルは、デフォルトで表示されます。</li> 
            <li><strong>並べ替えの選択肢 A ～ Z</strong>:フィールドに追加した選択をアルファベット順に並べ替えます。</li> 
           </ul> 
        </li> 
        <li> <p>ユーザーに追加する各選択に対して、歯車アイコンをクリックします。 <img src="assets/gear-icon-settings.png">次のいずれかのオプションを選択します。</p> 
           <ul> 
            <li><strong>デフォルトで選択</strong>:「 」フィールドでデフォルトの選択肢を選択します。</li> 
            <li> <p><strong>選択肢を非表示</strong>:フィールドで選択を非表示にします。 非表示の選択は、レポート内で引き続きアクセスできます。</p> </li> 
            <li> <p><strong>選択肢を削除</strong>:「 」フィールドから選択を削除します。</p> <p><b>警告</b>:この選択を使用する現在のオブジェクトがある場合は、フィールドから削除しないでください。 削除すると、履歴データが失われます。 代わりに、「 」オプションを選択して非表示にします。これにより、ユーザーは将来このオプションを選択できなくなります。</p> </li> 
           </ul> 
        </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

1. （条件付き）カスタムフォーム上のフィールドの表示タイプを変更するには、 **表示タイプ** ドロップダウンメニューから、目的のタイプを選択します。

   次のフィールド表示タイプを切り替えることができます。

   * **選択タイプのフィールド**:チェックボックス、ドロップダウン、ラジオボタン。
   * **テキストタイプのフィールド**:1 行のテキストフィールド、段落のテキストフィールド。 ( 書式設定のあるテキストフィールドを別の表示タイプに切り替えることはできません。 ただし、削除して別のタイプのフィールドを追加することもできます )。

   例えば、チェックボックスフィールドを作成した場合は、そのフィールドをドロップダウンフィールドまたはラジオボタンフィールドに変更できます。 また、1 行のテキストフィールドを作成した場合は、そのフィールドを段落テキストフィールドに変更できます。

   >[!NOTE]
   >
   >フィールドの表示タイプをチェックボックスフィールドまたは複数選択ドロップダウンフィールド（複数のオプションを選択できるドロップダウン）から単一選択フィールドタイプに変更する場合は、次の点を考慮します。
   >
   >* ラジオボタンに変更した場合、Workfrontは、ユーザーがフォームの任意の部分でデータを変更して保存するまで、フィールドに入力した複数選択値を保持します。 この時点で、複数選択タイプのフィールドを使用して選択された値は、選択されたラジオボタンの値に置き換えられます。
   >* 単一選択ドロップダウンに変更した場合、Workfrontは、ユーザーがフィールドに値を変更して保存するまで、ユーザーがフィールドに入力した複数選択値を保持します。 この時点で、複数選択タイプのフィールドを使用して選択した値は、選択したドロップダウン値に置き換えられます。


1. （オプション）手順 2～6 を繰り返して、他のカスタムフィールドを追加します。

   または

   組織用に既に作成されているフィールドを追加します。詳しくは、 [カスタムフォームでカスタムフィールドまたはウィジェットを再利用する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md#add).

   >[!NOTE]
   >
   >1 つのカスタムフォームに最大 500 個のフィールドとウィジェットを追加できます。 ただし、フォームの複雑さに応じて 100 を超える場合は、パフォーマンスの低下が生じる可能性があります。 複雑なフォームの例としては、カスケードパラメーターを持つフォーム、計算済みカスタムデータフィールド、単一のフィールドに複数の値を入力するオプションなどがあります。

1. クリック **適用**.
1. 他の方法でカスタムフォームの作成を続ける場合は、次の記事のいずれかに進みます。

   * [カスタムフォーム内でのカスタムフィールドおよびウィジェットの配置](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [カスタムフォームでのアセットウィジェットの追加または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [計算データをカスタムフォームに追加する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [カスタムフォームにセクション区切りを追加する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [カスタムフォームで既存の計算済みカスタムフィールドを再利用する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [表示ロジックの追加とカスタムフォームへのロジックのスキップ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [カスタムフォームのプレビューと完了](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)
