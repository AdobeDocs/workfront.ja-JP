---
title: レイアウトテンプレートを使用した Adobe Workfront のブランディング
user-type: administrator
product-area: system-administration;templates
navigation-topic: layout-templates
description: Adobe Workfront 管理者またはグループ管理者は、レイアウトテンプレートを使用して、特定のグループ、チーム、担当業務およびユーザーの上部ナビゲーション領域とメインメニューのロゴをカスタマイズできます。これは、大規模な組織内で独自のブランディングを持つにグループに特に役立ちます。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: ded9ab1e-c5f4-476b-ac81-0497dbe6b24d
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: ht
source-wordcount: '558'
ht-degree: 100%

---

# レイアウトテンプレートを使用した Adobe Workfront のブランディング

>[!IMPORTANT]
>
>このページで説明する手順は、まだ [!DNL Adobe Experience Cloud] にオンボーディングしていない組織にのみ適用されます。
>
> 組織が [!DNL Adobe Experience Cloud] にオンボーディング済みの場合、ブランディングは利用できません。

特定のグループ、チーム、担当業務およびユーザーの上部ナビゲーション領域とメインメニューのロゴをカスタマイズできます。これは、大規模な組織内で独自のブランディングを持つにグループに特に役立ちます。

グループのレイアウトテンプレートについて詳しくは、[グループのレイアウトテンプレートの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)を参照してください。

>[!NOTE]
>
>Workfront 管理者は、[Adobe Workfront インスタンスのブランディング](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md)で説明されているように、組織全体に対して同一ブランディングのカスタマイズをシステムレベルでを行うことができます。ただし、レイアウトテンプレートのブランディング設定は、システムレベルのブランディング設定をオーバーライドします。
><!--
>Maybe add a section about deleting these 2 settings to revert to default branding?
>-->

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>これらの手順をシステムレベルで実行するには、システム管理者のアクセスレベルが必要です。
グループに対して実行するには、そのグループの管理者である必要があります。</p> <p><b>メモ</b>：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## レイアウトテンプレートを使用した Adobe Workfront のブランディング

1. [レイアウトテンプレートを作成および管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)で説明されているように、レイアウトテンプレートの使用を開始します。
1. **ユーザーの表示項目をカスタマイズする**&#x200B;の下にある下向き矢印![](assets/dropdown-arrow.png)をクリックし、**ブランディング**&#x200B;を選択します。
1. このレイアウトテンプレートが割り当てられているユーザー向けに、ブランディングイメージを使用して Workfront をカスタマイズするには、次のいずれかの変更を行います。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>ホームアイコンをブランディングします<span style="font-weight: normal;">（ナビゲーション領域上部の左端に表示されます）</span></p> </td> 
      <td> <p><strong>ナビゲーション領域上部</strong>セクションの<strong>ホームアイコン</strong>の下のボックス内の任意の場所をクリックし、ロゴ画像を探して選択します。または、画像をボックスにドラッグします。</p> <p>画像を切り抜くには、スクロールコントロールを使用し、所定のスペース内の希望の位置に画像をドラッグします。</p> <p>120 x 120 の画像をお勧めします。GIF、JPG、PNG、SVG のいずれかの形式を使用できます。</p> <p>このアイコンは、レポート、リスト、ダッシュボード、およびユーザーが PDF ファイルとして書き出す配信レポートにも表示されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>メインメニューの <img src="assets/main-menu-icon.png"> ロゴ<span style="font-weight: normal;">のブランディング（メインメニューの右上隅に表示されます）</span></p> </td> 
      <td> <p> <p> <p><strong>ナビゲーション領域上部</strong>セクションの<strong>メインメニューロゴ</strong>の下のボックス内の任意の場所をクリックし、ロゴ画像を探して選択します。または、画像をボックスにドラッグします。</p> <p>画像を切り抜くには、スクロールコントロールを使用し、所定のスペース内の希望の位置に画像をドラッグします。</p> <p>300 x 120 ピクセルの画像をお勧めします。GIF、JPG、PNG、SVG のいずれかの形式を使用できます。</p> </p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 引き続きレイアウトテンプレートをカスタマイズします。

   または

   カスタマイズが終了したら、「**保存**」をクリックします。

   >[!TIP]
   >
   >いつでも「保存」をクリックして進行状況を保存して、後でテンプレートの変更を続行できます。

1. 「**保存**」をクリックします。

レイアウトテンプレートについて詳しくは、[レイアウトテンプレートの作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)を参照してください。
