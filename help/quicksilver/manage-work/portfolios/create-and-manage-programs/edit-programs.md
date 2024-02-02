---
product-area: programs
navigation-topic: create and manage programs
title: プログラムの編集
description: 自分が作成したプログラムや他のユーザーが作成したプログラム（そのユーザーと共有した場合）に関する情報を編集できます。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 7dcdfc5a-3fc1-48a8-ae28-a6a0a458732e
source-git-commit: 93c36a87667097729e89a61f68cc17e9c861d547
workflow-type: ht
source-wordcount: '1051'
ht-degree: 100%

---

# プログラムの編集

自分が作成したプログラムや他のユーザーが作成したプログラム（そのユーザーと共有した場合）に関する情報を編集できます。

プログラムページでプログラムを編集することも、リスト内のプログラムを編集することもできます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル*</td> 
   <td> <p>プログラムへの[!UICONTROL Edit]アクセス権</p> <p>メモ：アクセス権がない場合は、アクセスレベルに追加の制限が設定されているかを [!DNL Workfront] 管理者にお問い合わせください。アクセスレベルでのプログラムへのアクセスについては、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md" class="MCXref xref">プログラムへのアクセス権の付与</a>を参照してください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プログラムの[!UICONTROL Manage]権限</p> <p> プログラムの権限の付与については、<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-program.md" class="MCXref xref">プログラムの共有</a>を参照してください。 </p> <p>追加の権限の申請については、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトの利用申請</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## プログラムの編集

1. **[!UICONTROL メインメニュー]**&#x200B;に移動します。
1. 「**[!UICONTROL プログラム]**」をクリックし、プログラム名をクリックして開きます。

   >[!TIP]
   >
   >関連付けられているポートフォリオからプログラムにアクセスするには、まずポートフォリオに移動し、左パネルの「**[!UICONTROL プログラム]**」をクリックします。詳しくは、[プログラムの作成](../../../manage-work/portfolios/create-and-manage-programs/create-program.md)を参照してください。

1. （オプション）プログラムに関する限定的な情報を編集するには、左パネルの「**[!UICONTROL プログラムの詳細]**」をクリックします。

   >[!TIP]
   >
   >プログラムに関するすべての情報を編集する場合は、手順 4 に進みます。

   ![](assets/program-details-with-a-custom-form-section-nwe-350x137.png)

   >[!NOTE]
   >
   >[!DNL Workfront] 管理者またはグループ管理者がレイアウトテンプレートを変更した方法によっては、[!UICONTROL プログラムの詳細]エリアのフィールドが並べ替えられたり、表示されなかったりする場合があります。詳しくは、[レイアウトテンプレートを使用した[!UICONTROL 詳細]ビューのカスタマイズ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)を参照してください。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the above note will also come to the Edit Program box)</p>
   -->

   「[!UICONTROL 詳細]」セクションの情報を編集するには、以下を行います。

   1. （オプション）右上隅の&#x200B;**[!UICONTROL すべて折りたたむ]**&#x200B;アイコンをクリックして、すべてのエリアを折りたたみます。
   1. （オプションおよび条件付き）エリアが折りたたまれている場合、各エリアの横にある&#x200B;**右矢印** ![](assets/right-pointing-arrow.png) をクリックして、編集するエリアを展開します。
   1. 「[!UICONTROL プログラムの詳細]」セクションに表示されるフィールドについては、以下に説明するように、引き続き[!UICONTROL プログラムの編集]ボックスでプログラムを編集します。
   1. （オプション）プログラムにカスタムフォームが添付されていない場合は、「**[!UICONTROL カスタムフォームを追加]**」フィールドにフォームの名前を入力していき、リストに名前が表示されたら選択して、「**[!UICONTROL 変更を保存]**」をクリックします。
   1. （オプション）[!UICONTROL 概要]とカスタムフォームの情報をPDFファイルに書き出すには、**[!UICONTROL 書き出し]**&#x200B;アイコン ![](assets/export.png) をクリックし、「**[!UICONTROL 書き出し]**」をクリックします。次の中から選択します。

      * すべてを選択（1 つ以上のカスタムフォームが添付されている場合にのみ表示）
      * [!UICONTROL 概要]
      * 1 つまたは複数のカスタムフォームの名前

      PDF ファイルがお使いのコンピューターにダウンロードされます。

      ![](assets/export-portfolio-details-box-with-export-button-350x368.png)

      詳しくは、[カスタムフォームとオブジェクト詳細の書き出し](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md)を参照してください。


1. 1 つ以上のプログラムに関するすべての情報を編集するには、次のいずれかを行います。

   * プログラム名の横に表示される&#x200B;**[!UICONTROL その他]**&#x200B;メニューアイコン ![](assets/more-icon.png) をクリックしたあと、「**[!UICONTROL 編集]**」をクリックします。
   * プログラムのリストに移動し、編集する 1 つ以上のプログラムを選択して、リストの上部にある&#x200B;**[!UICONTROL 編集]**&#x200B;アイコン ![](assets/edit-icon.png) をクリックします。

   **[!UICONTROL プログラムの編集]**&#x200B;ダイアログボックスが表示されます。

   ![](assets/edit-program-box-nwe-350x236.png)

   すべてのプログラムフィールドが[!UICONTROL プログラムの編集]ボックスで使用でき、左パネルに表示されたエリアにグループ化されています。

1. 次のセクションのいずれかに情報を指定することを検討してください。

   * [[!UICONTROL 概要]](#overview)
   * [[!UICONTROL カスタムフォーム]](#Custom%C2%A0F)
   * [[!UICONTROL コメント]](#comment)

### [!UICONTROL 概要] {#overview}

1. 上記の説明に従って、プログラムの編集を開始します。
1. 「**[!UICONTROL 概要]**」をクリックし、以下のフィールドを指定します。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;note below drafted for now)</p>
   -->

   <!--
   <note type="note">
   Depending on how your Workfront administrator or Group administrator sets up our Layout Template, the fields in the Edit Program box might be rearranged or not display. For information, see
   <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md" class="MCXref xref">Customize the Details view using a layout template</a>.
   </note>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td> <p>プログラムの名前を更新します。 </p> <p>ヒント：複数のプログラムを選択した場合は使用できません。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td> <p>ポートフォリオの説明を入力して、その独自性を示します。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Program Manager]</td> 
      <td> <p>プログラムマネージャーとして指定するユーザの名前を入力していき、リストに目的の名前が表示されたら選択します。これは、プログラムのプロジェクトで定義された作業を監督できるユーザーです。 </p> <p>重要：ユーザーをプログラムマネージャーに指名すると、そのユーザーには、プログラムおよびプログラム内のプロジェクトの[!UICONTROL Manage]権限が自動的に付与されます。 </p> <p>ヒント：プログラムヘッダーで、プログラムマネージャーをすばやく更新できます。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Group]</td> 
      <td> <p>グループがプログラムに関連付けられている場合や、プログラムを完了する責任がある場合は、1 つのグループの名前を追加します。 </p> <p>ヒント：  <p>[!UICONTROL Program Details]ページから「[!UICONTROL Group]」フィールドにアクセスする場合は、以下を行います。 </p> <p>適切なグループを選択していることを確認するには、グループにポインタを合わせて、グループの横に表示される[!UICONTROL information]アイコン <img src="assets/info-icon.png"> をクリックします。グループの上位のグループの階層や管理者など、グループに関する情報が一覧表示されるツールチップが表示されます。</p> <p> <img src="assets/group-details-widget-programs-350x268.png" style="width: 350;height: 268;"> </p> <p>このオプションは、[!UICONTROL Edit Program]ボックスでは使用できません。 </p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Is Active]</td> 
      <td> <p> プログラムをアクティブにする場合は、このチェックボックスをオンにします。他のユーザーは、アクティブなプログラムを見つけてプロジェクトに添付したり、ポートフォリオに追加したりできます。非アクティブなプログラムは、プロジェクトやポートフォリオに添付できません。これはデフォルトで有効になっています。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 「**[!UICONTROL 変更を保存]**」をクリックするか、引き続き、以下のセクションを編集します。

### [!UICONTROL カスタムフォーム]

1. 上記の説明に従って、プログラムの編集を開始します。
1. **[!UICONTROL フォームを追加]**&#x200B;ドロップダウンメニューをクリックしてカスタムフォームを選択し、プログラムに追加します。

   追加できるようにするには、まず、プログラムのカスタムフォームを作成する必要があります。

   >[!NOTE]
   >
   >[!DNL Workfront] 管理者がカスタムフォームのセクションの権限を設定する方法によっては、特定のカスタムフォーム上の同じフィールドを誰でも表示または編集できるとは限りません。カスタムフォームのセクション内のフィールドを編集する権限は、プログラム自体に対する権限によって異なります。カスタムフォームのセクションに対する権限の設定については、[カスタムフォームの作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)を参照してください。

1. カスタムフォームのフィールドを更新し、「**[!UICONTROL 変更を保存]**」をクリックして、次のセクションに進みます。

### [!UICONTROL コメント] {#comment}

1. 上記の説明に従って、プログラムの編集を開始します。
1. 「**[!UICONTROL コメント]**」をクリックします。

   ![](assets/comment-box-in-program-edit-box-classic-350x195.png)

1. 「**[!UICONTROL プログラムに更新を投稿]**」フィールドにコメントを追加します。
1. （オプション）**[!UICONTROL ユーザー]**&#x200B;アイコンをクリックして、コメントにユーザーまたはチームを追加します。
1. （オプション）**[!UICONTROL ロック]**&#x200B;アイコンをクリックしてコメントをロックし、アクセスを社内のユーザーのみに限定します。

   変更を保存すると、追加したコメントがプログラムの「[!UICONTROL 更新]」タブに表示され、コメントに含まれているユーザーにメールが送信されます。
