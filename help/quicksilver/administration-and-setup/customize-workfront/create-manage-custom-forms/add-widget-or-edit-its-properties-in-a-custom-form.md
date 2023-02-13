---
title: カスタムフォームでの画像や他のアセットウィジェットの追加や編集
description: カスタムフォーム内の画像、ビデオ、PDFファイル、Adobe XDファイルなど、次のアセットウィジェットのプロパティを追加または編集できます。 これは、デザイン中のアプリに、ブランディング画像、説明用ビデオ、インタラクティブプロトタイプなどのビジュアルコンテンツを含める必要がある場合に役立ちます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 62a2f9a1-80de-40e7-9d8b-46ed9df083c1
source-git-commit: eeff0c8a3f7cbccd942c978d771d24f4cf9c425d
workflow-type: tm+mt
source-wordcount: '1325'
ht-degree: 1%

---

# カスタムフォームでの画像や他のアセットウィジェットの追加や編集

カスタムフォームでは、次のアセットウィジェットのプロパティを追加または編集できます。

* 画像
* ビデオ
* PDFファイル
* Adobe XDファイル

これは、デザイン中のアプリに、ブランディング画像、説明用ビデオ、インタラクティブプロトタイプなどのビジュアルコンテンツを含める必要がある場合に役立ちます。

ウィジェットを含むカスタムフォームがオブジェクトに添付されている場合、オブジェクトを操作するユーザーは、次の領域でそのフォームを表示できます。

* オブジェクトの [ 詳細 ] 領域（たとえば、プロジェクトの場合は [ プロジェクトの詳細 ] 領域）
* 新しいAdobe Workfrontエクスペリエンスのルックアンドフィール（「プロジェクトを編集」ボックスや「タスクを編集」ボックスなど）がある場合は、オブジェクトの編集ボックス

現在、ユーザーは以下の領域でウィジェットを表示できません&#x200B;。

* リストとレポート
* ホームと概要
* 新しいAdobe Workfrontエクスペリエンスのルックアンドフィールがない場合は、オブジェクトの編集ボックス（「費用を編集」ボックスなど）
* Workfront Mobile アプリ


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

## カスタムフォームでのアセットウィジェットの追加または編集

1. カスタムフォームの使用を開始する ( [カスタムフォームの作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. を使用 **フィールドを追加** タブを開き、次のいずれかの操作を行います。

   * 新しいウィジェットを追加する場合は、「 **画像**, **PDF**&#x200B;または **ビデオ** をクリックしてフォームの下部に追加するか、フォーム上の目的の場所にドラッグします。

      ![](assets/add-widget.png)


   * 別のカスタムフォームに既に追加されているウィジェットを追加する場合は、 **フィールドライブラリ**&#x200B;をクリックし、表示されるリストでウィジェットの名前をクリックします。 詳しくは、 [カスタムフォームでカスタムフィールドまたはウィジェットを再利用する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   * カスタムフォームに既に追加されているウィジェットを編集する場合は、そのウィジェットを選択します。

1. ウィジェットの次のいずれかのプロパティを入力または編集します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">ラベル</td> 
      <td> <p>（必須）ウィジェットの上に表示する説明的なラベルを入力します。 ラベルはいつでも変更できます。</p> <p><b>重要</b>:このラベルでは特殊文字を使用しないでください。 レポートでは正しく表示されません。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">名前</td> 
      <td> <p>（必須）この名前は、システムがウィジェットを識別する方法です。</p> <p>初めてウィジェットを設定し、ラベルを入力すると、「名前」フィールドが自動的に設定され、それに合わせて設定されます。 ただし、「ラベル」フィールドと「名前」フィールドは同期されません。これにより、システムで表示される名前を変更することなく、ユーザーに表示されるラベルを自由に変更できます。</p> <p><b>重要</b>:可能ですが、ウィジェットでカスタムフォームを使用し始めた後は、この名前を変更しないことをお勧めします。 そうすると、Workfrontの他の領域で参照される可能性のあるウィジェットが認識されなくなります。 </p> <p>各ウィジェット名は、組織のWorkfrontインスタンス内で一意である必要があります。 これにより、既に作成済みのものを別のカスタムフォームに再利用できます。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>（必須）ウィジェットがインターネット上で保存されているウィジェットの URL を入力または貼り付けます。</p> 
      <p>ビデオウィジェットを追加する場合は、現在、URL ボックスに次のコードを追加して追加できます。</p> 
      <ul> 
      <li> <p>YouTubeまたは Vimeo リンク</p> </li> 
      <li> <p>Google Drive ビデオリンク</p> </li> 
      <li> <p>MP4 および MOV 拡張子を持つビデオへのリンク</p> </li> 
      <li> <p>Workfrontインスタンスのドキュメント領域に既にアップロードされているビデオへのリンク。 手順については、 <a href="#add-a-video-widget-to-a-custom-form-from-the-documents-area" class="MCXref xref">「ドキュメント」領域からカスタムフォームにビデオウィジェットを追加する</a> 」を参照してください。</p> </li> 
      </ul> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">指示</td> 
      <td> <p>ウィジェットに関する追加情報を入力します。 カスタムフォームに入力する際に、疑問符アイコンの上にマウスポインターを置くと、ここに入力した情報を含むツールヒントが表示されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">サイズ</td> 
      <td>必要に応じてウィジェットの表示サイズを変更します。</td> 
     </tr> 
    </tbody> 
   </table>

1. クリック **適用**.
1. 他の方法でカスタムフォームの作成を続ける場合は、次の記事のいずれかに進みます。

   * [カスタムフォーム内でのカスタムフィールドおよびウィジェットの配置](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [カスタムフォームにカスタムフィールドを追加する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [カスタムフォームでカスタムフィールドまたはウィジェットを再利用する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md)
   * [計算データをカスタムフォームに追加する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [カスタムフォームで既存の計算済みカスタムフィールドを再利用する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [表示ロジックの追加とカスタムフォームへのロジックのスキップ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [カスタムフォームのプレビューと完了](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)


## カスタムフォームへのXDファイルの追加

1. カスタムフォームの使用を開始する ( [カスタムフォームの作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. を使用 **フィールドを追加** タブを開き、「」を選択します。 **Adobe XD**.
1. ウィジェットの次のいずれかのプロパティを入力または編集します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">ラベル</td> 
      <td> <p>（必須）ウィジェットの上に表示する説明的なラベルを入力します。 ラベルはいつでも変更できます。</p> <p><b>重要</b>:このラベルでは特殊文字を使用しないでください。 レポートでは正しく表示されません。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">名前</td> 
      <td> <p>（必須）この名前は、システムがウィジェットを識別する方法です。</p> <p>初めてウィジェットを設定し、ラベルを入力すると、「名前」フィールドが自動的に設定され、それに合わせて設定されます。 ただし、「ラベル」フィールドと「名前」フィールドは同期されません。これにより、システムで表示される名前を変更することなく、ユーザーに表示されるラベルを自由に変更できます。</p> <p><b>重要</b>:可能ですが、ウィジェットでカスタムフォームを使用し始めた後は、この名前を変更しないことをお勧めします。 そうすると、Workfrontの他の領域で参照される可能性のあるウィジェットが認識されなくなります。 </p> <p>各ウィジェット名は、組織のWorkfrontインスタンス内で一意である必要があります。 これにより、既に作成済みのものを別のカスタムフォームに再利用できます。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>（必須）有効なXDプロトタイプリンクを入力するか貼り付けます。</p> 
      <p>注意：Adobe XDの「共有」タブの「リンクアクセス」設定は、「リンクを知っているすべてのユーザー」に設定されている必要があります。 そうしないと、ユーザーはプロトタイプを表示できなくなります。 
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">指示</td> 
      <td> <p>（オプション）ウィジェットに関する追加情報を入力します。 カスタムフォームに入力する際に、疑問符アイコンの上にマウスポインターを置くと、ここに入力した情報を含むツールヒントが表示されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">サイズ</td> 
      <td>（オプション）必要に応じてウィジェットの表示サイズを変更します。</td> 
     </tr> 
    </tbody> 
   </table>

1. 他の方法でカスタムフォームの作成を続ける場合は、次の記事のいずれかに進みます。

   * [カスタムフォーム内でのカスタムフィールドおよびウィジェットの配置](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [カスタムフォームにカスタムフィールドを追加する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [カスタムフォームでカスタムフィールドまたはウィジェットを再利用する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md)
   * [計算データをカスタムフォームに追加する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [カスタムフォームで既存の計算済みカスタムフィールドを再利用する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [表示ロジックの追加とカスタムフォームへのロジックのスキップ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [カスタムフォームのプレビューと完了](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

## 「ドキュメント」領域からカスタムフォームにビデオウィジェットを追加する {#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>この方法でビデオをカスタムフォームに追加する場合、ユーザーがオブジェクトのフォームにアクセスするときは、カスタムフォームに設定された権限のみがビデオに適用され、ドキュメント領域のビデオに設定された権限は適用されません。

1. 「ドキュメント」領域のビデオに移動し、その配達確認を生成します ( [Web サイトまたはその他の Web コンテンツ用のインタラクティブな配達確認の作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md).
1. 配達確認を開きます。
1. ビデオの任意の場所を右クリックし、「 」を選択します。 **ビデオアドレスをコピー**.
1. ビデオウィジェットを追加するカスタムフォームで、コピーしたアドレスを **URL** ボックス
