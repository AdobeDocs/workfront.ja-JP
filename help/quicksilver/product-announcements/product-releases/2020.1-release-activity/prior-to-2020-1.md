---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: 2020.1 リリースより前に実稼動環境にリリースされたその他の Workfront Classic 機能
description: 次の機能は、2020.1 が本番にリリースされる前に、Workfront Classic 本番環境で利用できるようになりました。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 267757fb-a8ef-43cf-a93c-3ac59d8bb432
TQID: https://experienceleague.adobe.com/E-knnp2lqfo7D45q9KtIRzazdBO-woliweMCHAl7Xww
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: e14a7f57-c82c-4874-a495-5d036cbbdc3did: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2: id: b8ea32d4-f1fe-4c71-8871-afe5a702a009
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 355
ht-degree: 100%

---

# 2020.1 リリースより前に実稼動環境にリリースされたその他の Workfront Classic 機能

次の機能は、2020.1 が本番にリリースされる前に、Workfront Classic 本番環境で利用できるようになりました。

リリース期間と 2020.1 リリースで利用可能なすべての機能については、[2020.1 リリースの概要](../../../product-announcements/product-releases/2020.1-release-activity/2020-1-release-overview.md)を参照してください。

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td> Chrome との互換性を維持するために Workfront クッキーの動作を更新しました <p>今後の Google Chrome の更新（Chrome v80）との互換性を維持するために、Workfront のプラットフォームを更新し、リクエストに応じてクッキーが適切に送信されるようにしました。 </p> <p>この Chrome の更新により、SameSite クッキー属性のデフォルト値が変更になります。 Google Chrome を更新後に Workfront インスタンスがどのように動作するかをテストするには、Chrome でフラグを調整し、次のオプションを有効にします。 </p> 
    <ul> 
     <li>「デフォルトのクッキーによる SameSite」 </li> 
     <li>「SameSite を使用しないクッキーは安全でなければならない」</li> 
    </ul> 
    <div class="workfront_plans"> 
     <p><strong>利用可能な環境：</strong> </p> 
     <ul> 
      <li>Workfront Classic</li> 
      <li>新バージョンの Workfront</li> 
     </ul> 
     <p><strong>プレビューリリース</strong> </p> 
     <ul> 
      <li>2020年1月29日（PT）</li> 
     </ul> 
     <p><strong>実稼動リリース：</strong> </p> 
     <ul> 
      <li> 2020年1月30日（PT）</li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>「アップデート」エリアのその他メニュー <p>更新の詳細メニューを使用して、次を行います。</p> 
    <ul> 
     <li>アップデートの本文をコピー</li> 
     <li>アップデートスレッドまたは単一の更新への直接リンクをコピー</li> 
     <li>アップデートを削除</li> 
    </ul> <p>詳しくは、<a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref" xrefformat="{para}">作業を更新</a>を参照してください。</p> 
    <div class="workfront_plans"> 
     <p><strong>利用可能な環境：</strong> </p> 
     <ul> 
      <li>Workfront Classic</li> 
      <li>新バージョンの Workfront</li> 
     </ul> 
     <p><strong>実稼動リリース：</strong> </p> 
     <ul> 
      <li> 2020年1月8日（PT）</li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>「アップデート」エリアの新しい進捗バー <p>アップデート領域の完了率の進捗率バーの外観が変わりました。 クリック&amp;ドラッグしてパーセントをアップデートするか、ダブルクリックして数字を手動で入力します。</p> <p>詳しくは、<a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref" xrefformat="{para}">作業を更新</a>を参照してください。</p> 
    <div class="workfront_plans"> 
     <p><strong>利用可能な環境：</strong> </p> 
     <ul> 
      <li>Workfront Classic</li> 
      <li>新バージョンの Workfront</li> 
     </ul> 
     <p><strong>実稼動リリース：</strong> </p> 
     <ul> 
      <li> 2020年1月8日（PT）</li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td> Workfront のコメントを Jira に同期しました <p>Workfront の Jira との統合により、Workfront のコメントを Jira のネイティブなコメントストリームに同期できるようになりました。</p> <p>以前は、Jira から Workfront にコメントを同期できましたが、Workfront から Jira にコメントを同期することはできませんでした。 </p> <p>詳しくは、<a href="../../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront の Jira 向け設定</a>を参照してください。</p> 
    <div class="workfront_plans"> 
     <p><strong>利用可能な環境：</strong> </p> 
     <ul> 
      <li>Workfront Classic</li> 
      <li>新バージョンの Workfront</li> 
     </ul> 
     <p><strong>実稼動リリース：</strong> </p> 
     <ul> 
      <li> 2019年12月20日（PT）</li> 
     </ul> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>
