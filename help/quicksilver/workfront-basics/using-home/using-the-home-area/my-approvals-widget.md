---
product-area: home
navigation-topic: use-the-home-area
title: マイ承認ウィジェットを使用した承認の管理
description: マイ承認ウィジェットには、保留中、割り当て済み、委任済み、送信済みのすべての承認が1か所に表示されます。 ここでは、承認のフィルタリングと整理、意思決定、必要に応じた承認の委任を行うことができます。
author: Courtney
feature: Get Started with Workfront
exl-id: 276a33f5-92de-440c-ae3a-8cd01731434f
source-git-commit: 30e27ba5a12733660a88cd7e9643bea868503774
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 38%

---

# マイ承認ウィジェットを使用した承認の管理

{{highlighted-preview}}

マイ承認ウィジェットには、保留中、割り当て済み、委任済み、送信済みのすべての承認が1か所に表示されます。 ここでは、承認のフィルタリングと整理、意思決定、必要に応じた承認の委任を行うことができます。

My Approvals ウィジェットでは、次のWorkfront オブジェクトからの承認をサポートしています。

* タスク
* イシュー
* プロジェクト
* ドキュメント
* プルーフ
* プランニングレコードのリクエスト
* タイムシート

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> 
   <p>コントリビューター以上</p>
   <p>レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>承認に関連付けられたオブジェクトに対する表示以上のアクセス権</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>承認に関連付けられたオブジェクトに対する表示以上の権限</p></td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 自分の承認ウィジェットからの作業の承認

1. 右上隅の&#x200B;**[!UICONTROL メインメニュー]** ![&#x200B; メインメニューアイコン &#x200B;](assets/main-menu-icon.png)をクリックし、**[!UICONTROL ホーム]**&#x200B;をクリックします。
1. （条件付き）「**カスタマイズ**」をクリックして、**自分の承認** ウィジェットを追加します。
1. （条件付き）「**フィルター**」ドロップダウンメニューをクリックし、**すべて**&#x200B;を選択して、自分に割り当てられた承認と委任された承認を表示します。

   >[!NOTE]
   >
   >担当業務またはグループに割り当てられた承認は、ホームに表示されません。 チームに割り当てられた承認は、各チームメンバーのマイ承認ウィジェットに表示されます。


1. <span class="preview"> （条件付き）「**並べ替え**」ドロップダウンメニューをクリックし、**最新の最初の**」を選択して、最近追加された承認を表示します。</span>


1. <span class="preview"> （オプション）全画面表示アイコン ![全画面表示アイコン &#x200B;](assets/full-screen.png)をクリックして、自分の承認ウィジェットを全画面表示で開きます。</span>

1. 承認する項目を選択します。

   ![自分の承認ウィジェット &#x200B;](assets/my-approvals-widget.png)

   <!--update screenshot after production release-->

1. 右側のパネルで承認を決定する際に、使用可能なオプションの 1 つをクリックします。 承認する項目のタイプに応じて、ページの右上隅に次のオプションが表示されます。

   <table>
   <tr>
      <td>
      <p><strong>アクセス</strong></p>
      </td>
      <td>
      <p><strong>作業項目</strong></p>
      </td>
      <td>
      <p><strong>ドキュメント</strong></p>
      </td>
      <td>
      <p><strong>プルーフ</strong></p>
      </td>
   </tr>
   <tr>
      <td>
       <ul>
      <li>付与</li>
      <li>無視</li>
      </ul>
      必要に応じて、<b> アクセス権の変更</b> ドロップダウンメニューでアクセス権のレベルを調整できます。
      </td>
      <td>
         <ul>
         <li>承認</li>
         <li>Reject</li>
         </ul>
      決定ボタンのドロップダウンメニューをクリックして、決定にコメントを残すことができます。
      </td>
      <td>
   承認者として割り当てられた
         <ul>
         <li>承認</li>
         <li>変更して承認</li>
         <li>作業が必要</li>
         </ul>
   レビュアーとして割り当てられました
         <ul>
         <li>レビューの完了</li>
         </ul>
      この列のオプションは、統合承認にのみ適用されます。 レガシードキュメントの承認は、作業項目の承認と同じように表示されます。 
      </td>
      <td>
         <ul>
         <li>プルーフを見る</li>
         </ul>
         プルーフビューアで決定します。 プルーフの確認について詳しくは、<a href="/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md">Adobe Workfront でのプルーフのレビュー</a>を参照してください。
      </td>
   </tr>
   </table>

決定を行うと、承認はマイ承認ウィジェットから削除されます。
