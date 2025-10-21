---
product-area: home
navigation-topic: use-the-home-area
title: 自分の承認ウィジェットを使用した承認の管理
description: 自分の承認ウィジェットには、保留中、割り当て済み、委任済み、送信済みのすべての承認が 1 か所で表示されます。 ここでは、承認をフィルタリングおよび整理し、決定を行い、必要に応じて承認を委任できます。
author: Courtney
feature: Get Started with Workfront
source-git-commit: 4981d9adb2cae53e30f13aa2a7aa6857befbf3ca
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 33%

---

# 自分の承認ウィジェットを使用した承認の管理

自分の承認ウィジェットには、保留中、割り当て済み、委任済み、送信済みのすべての承認が 1 か所で表示されます。 ここでは、承認をフィルタリングおよび整理し、決定を行い、必要に応じて承認を委任できます。

自分の承認ウィジェットは、次のWorkfront オブジェクトからの承認をサポートしています。

* タスク
* イシュー
* プロジェクト
* ドキュメント
* プルーフ
* レコード要求の計画
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
   <p>投稿者以上</p>
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

1. 右上隅の **[!UICONTROL メインメニュー]**![&#x200B; メインメニューアイコン &#x200B;](assets/main-menu-icon.png) をクリックし、**[!UICONTROL ホーム]** をクリックします。
1. （条件付き） **カスタマイズ** をクリックして **マイ承認** ウィジェットを追加します。
1. （条件付き） **フィルター** ドロップダウンメニューをクリックし、「**すべて**」を選択して、割り当てられた承認と委任された承認を確認します。

   >[!NOTE]
   >
   >担当業務またはグループに割り当てられた承認は、ホームに表示されません。 チームに割り当てられた承認は、各チームメンバーのマイ承認ウィジェットに表示されます。


1. 承認する項目を選択します。

   ![&#x200B; マイ承認ウィジェット &#x200B;](assets/my-approvals-widget.png)

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
      必要に応じて、<b> アクセス権を変更 </b> ドロップダウンメニューでアクセスレベルを調整できます。
      </td>
      <td>
         <ul>
         <li>承認</li>
         <li>Reject</li>
         </ul>
      決定ボタンのドロップダウンメニューをクリックして、決定にコメントを残すことができます。
      </td>
      <td>
   承認者として割り当てられました
         <ul>
         <li>承認</li>
         <li>変更して承認</li>
         <li>作業が必要</li>
         </ul>
   レビュアーとして割り当て済み
         <ul>
         <li>レビューの完了</li>
         </ul>
      この列のオプションは、統合承認にのみ適用されます。 従来のドキュメント承認は、作業項目の承認と同じように表示されます。 
      </td>
      <td>
         <ul>
         <li>プルーフに移動</li>
         </ul>
         決定はプルーフビューアで行います。 プルーフの確認について詳しくは、<a href="/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md">Adobe Workfront でのプルーフのレビュー</a>を参照してください。
      </td>
   </tr>
   </table>

決定を行うと、その承認が自分の承認ウィジェットから削除されます。