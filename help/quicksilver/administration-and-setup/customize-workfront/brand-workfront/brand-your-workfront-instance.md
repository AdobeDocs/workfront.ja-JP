---
title: Adobe Workfrontインスタンスのブランディング
user-type: administrator
product-area: system-administration
navigation-topic: brand-workfront
description: Workfront管理者は、ログイン画面、上部のナビゲーション領域、メインメニューで、Workfrontにロゴを使用してブランディングをおこなうことができます。 また、ログイン画面の背景画像や色を変更することもできます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 94603393-bdea-4673-9256-08da14f6916e
source-git-commit: 7b5b0fd95e39f37153e36abb4e3b8e738ac26d21
workflow-type: tm+mt
source-wordcount: '909'
ht-degree: 1%

---

# Adobe Workfrontインスタンスのブランディング

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **
-->

>[!IMPORTANT]
>
>このページで説明する手順は、まだにオンボーディングされていない組織にのみ適用されます。 [!DNL Adobe Experience Cloud].
>
> 組織が [!DNL Adobe Experience Cloud]、ブランディングを使用できません。

Workfrontの管理者は、次の場所でロゴを使用してWorkfrontのブランドを設定できます。

* ログイン画面

   ![](assets/brand-login-screen-nwe-adobe.jpg)

* ナビゲーション領域上部

   ![](assets/brand-top-nav-area-nwe-adobe.jpg)

* メインメニュー

   ![](assets/brand-main-menu-adobe.jpg)

また、ログイン画面の背景画像や色を変更することもできます。

![](assets/wf_banner_on_login_screen-adobe.png)

>[!NOTE]
>
>* 組織のWorkfrontインスタンスがカスタム SSO ポータルを使用している場合、ログインの背景画像と色の変更は使用できません。 詳細については、ネットワークまたは IT 管理者にお問い合わせください。

><!--
>or is enabled with Adobe IMS  >
>  >
>-->
>
>* Workfrontの管理者またはグループ管理者は、レイアウトテンプレートを使用して、特定のグループおよびユーザーのWorkfrontをブランディングすることもできます。 レイアウトテンプレートのブランディングは、この記事で説明するシステムレベルのブランディングを上書きします。 レイアウトテンプレートでのブランディングの手順については、 [レイアウトテンプレートを使用した Brand Adobe Workfront](../../../administration-and-setup/customize-workfront/use-layout-templates/brand-wf-using-a-layout-template.md).


## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront管理者である。</p> <p><b>注意</b>:まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## ログイン画面のブランディング

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **システム** > **ブランディング**.

1. 次の変更を加えて、ブランディング画像を使用してWorkfrontをカスタマイズします。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>「ホーム」アイコンのブランディング <span style="font-weight: normal;">（上部ナビゲーション領域の左端に表示）</span></p> </td> 
      <td> <p>内 <strong>上部ナビゲーション領域</strong> セクション、の下 <strong>ホームアイコン</strong>、ボックスの任意の場所をクリックし、ロゴ画像を探して選択します。 または、画像をボックスにドラッグします。</p> <p>画像を切り抜くには、スクロールコントロールを使用し、画像を指定されたスペース内の目的の位置までドラッグします。</p> <p>120 x 120 の画像を推奨します。 次のいずれかの形式にすることができます。GIF、JPG、PNG、SVG。</p> <p>このアイコンは、ユーザーがダッシュボードファイルとして書き出すレポート、リスト、ダッシュボード、配信されたレポートにもPDFされます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>メインメニューのブランディング <img src="assets/main-menu-icon.png"> ロゴ <span style="font-weight: normal;">（メインメニューの右上隅に表示）</span></p> </td> 
      <td> <p>内 <strong>上部ナビゲーション領域</strong> セクション、の下 <strong>メインメニューのロゴ</strong>、ボックスの任意の場所をクリックし、ロゴ画像を探して選択します。 または、画像をボックスにドラッグします。</p> <p>画像を切り抜くには、スクロールコントロールを使用し、画像を指定されたスペース内の目的の位置までドラッグします。</p> <p>300 x 120 ピクセルの画像を使用することをお勧めします。 次のいずれかの形式にすることができます。GIF、JPG、PNG、SVG。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ログイン画面のロゴのブランド化 <span style="font-weight: normal;">（ユーザーがログイン資格情報を入力するボックスの左上に表示されます）</span></td> 
      <td> <p>の下 <strong>ログイン画面</strong>、ボックスの任意の場所をクリックし、ロゴ画像を探して選択します。 画像を切り抜くには、スクロールコントロールを使用し、画像を指定されたスペース内の目的の位置までドラッグします。</p> <p>300 x 120 ピクセルの画像を使用することをお勧めします。 次のいずれかの形式にすることができます。GIF、JPG、PNG、SVG。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ログイン画面の背景色のブランディング <span style="font-weight: normal;">（ユーザーがログイン資格情報を入力するボックスの後ろに表示されます）</span></td> 
      <td> <p>の下 <strong>ログイン画面</strong>、 <strong>背景色</strong>. </p> <p>RGBまたは HEX カラーコードを使用できます。</p> <p>背景色は、ログイン画面の背景画像がログイン画面の背景画像より大きい場合（この表の次の行を参照）、または画像に透明度がある場合にのみ表示されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ログイン画面の背景画像のブランディング <span style="font-weight: normal;">（ユーザーがログイン資格情報を入力するボックスの後ろに表示されます）</span></td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1"> <p> 内 <strong>ログイン画面</strong> 領域、下 <strong>背景画像</strong>」、「 」の順にクリックし、JPG、PNG 画像、または画像（最大 20 個）を検索して選択します。 </p> <p>複数の背景画像がランダムな順序で表示され、ユーザーがログインページを更新するたびに変更されます。 2 MB 以下の画像を使用することをお勧めします。</p> </li> 
        <li value="2"> <p>アップロードした各背景画像の上にマウスポインターを置き、設定（歯車）アイコンをクリックし、次のいずれかのオプションを使用して、画像をログイン画面の背景に表示する場所と方法を指定します。</p> 
         <ul> 
          <li> <p><strong>塗りつぶし画面</strong>:画像をログイン画面の背景に合わせて調整します。画像は拡大される場合があります。 高解像度の画像（最大 2 MB）を使用すると、最適な結果が得られます。</p> <p>このオプションを使用すると、Workfrontバナーはカスタマイズできず、画像の一部が見えなくなります。</p> </li> 
          <li> <p><strong>タイル</strong>:画像を元のサイズで、ログイン画面の背景領域全体に並べます。 これは、パターンを作成する場合に便利です。 背景領域の左上隅、中央上、右上からタイルを開始するには、青い線形オプションを選択します。</p> </li> 
          <li> <p><strong>位置</strong>:青い位置揃えオプションを使用して、選択した位置に画像を元のサイズに配置します。ログイン画面の背景領域の左上、中央上または右上。</p> <p>ログイン画面の残りの背景領域は、背景色で塗りつぶされます。 背景色の詳細については、この表の前の行を参照してください。</p> </li> 
         </ul> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">デフォルトのブランディングにリセット</td> 
      <td> <p>デフォルトのブランディングにリセットすると、アップロードしたすべての写真と画像が削除されます。</p> <p>クリック <strong>すべてのブランディングをWorkfrontのデフォルトにリセット</strong> 画面の右下隅で、 <strong>はい</strong>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >組織のWorkfrontインスタンスがカスタム SSO ポータルを使用している場合は使用できません。
   ><!--   >
   >or is enabled with Adobe IMS   >
   >   >
   >-->
   >
   >詳細については、ネットワークまたは IT 管理者にお問い合わせください。

1. 「**保存**」をクリックします。
