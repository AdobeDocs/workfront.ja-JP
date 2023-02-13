---
product-area: projects
navigation-topic: manage-issues
title: イシューの移動
description: 問題をプロジェクトとタスクの間で移動できます。
author: Alina
feature: Work Management
exl-id: 8ab9be3e-0412-43d9-ad1e-75c43613fa82
source-git-commit: 6c82c585376b41cff0e57b253b6a214fb00309de
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 1%

---

# イシューの移動

次のオブジェクト間で問題を移動できます。

* プロジェクトから別のプロジェクトへ
* タスクから同じプロジェクト内の別のタスク、または別のプロジェクト内の別のタスクへ
* タスクからプロジェクト、または別のプロジェクトに
* プロジェクトから同じプロジェクト内のタスク、または別のプロジェクト内のタスクに

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>リクエスト以上</p> <p>ライセンスを確認して、プロジェクトの「問題」セクションの問題を移動します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>問題へのアクセスを編集</p> <p>プロジェクトとタスクへのアクセス権を表示または高くする</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 アクセスレベルの問題へのアクセスについて詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">問題へのアクセス権の付与</a>. Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>問題に対する権限の管理</p> <p>問題を移動する項目に対する権限を付与し、問題を追加する機能を付与します。</p> <p> 問題に対する権限の付与について詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">イシューの共有 </a></p> <p>追加の権限のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。

## 問題の移動に関する考慮事項

ドキュメントを含む問題やリクエストキューに関連付けられている問題を移動する際は、次の点を考慮してください。

* **問題がリクエストキューに関連付けられている場合：** イシューを別のオブジェクトに移動し、そのイシューをリクエストキューに関連付けると、そのイシューは最初のイシューが発生した元のキューに関連付けられなくなります。
* **ドキュメントが問題に添付された場合：** イシューを別のオブジェクトに移動し、イシューにドキュメントが添付されると、そのドキュメント、バージョンおよび配達確認も新しいイシューに移動します。 ドキュメントに関連付けられている承認は移動されません。
* **問題がドキュメントまたはフォルダーにリンクされている場合：** Google Drive などのサードパーティのサービスにリンクされたドキュメントまたはフォルダーを含むイシューを移動すると、そのイシューと共にドキュメントへのリンクが移動します。

## リスト内の問題の移動

1 つまたは複数のイシューをイシューのリストまたはイシューレポートから移動できます。

1. 移動する 1 つまたは複数の問題を含むプロジェクトに移動します。

   または

   問題レポートに移動します。

1. プロジェクトに移動する場合は、 **問題** をクリックします。
1. 移動する 1 つまたは複数の問題を選択し、 **その他のメニュー** 問題リストの上部にあるをクリックし、 **移動先**.

   ![](assets/copy-and-move-to-links-for-issue-in-a-list-nwe-350x119.png)

1. 「 」セクションで説明されているように、引き続き問題を移動します。 [単一のイシューの移動](#move-a-single-issue) 手順 2 から始めます。

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: ensure step stays accurate)
   </MadCap:conditionalText>
   -->

## 単一のイシューの移動 {#move-a-single-issue}

イシューの表示時に 1 つのイシューを移動できます。

### プレビュー環境での 1 つのイシューの移動

1. コピーする問題に移動し、 **詳細** メニュー ![](assets/more-icon.png)問題名の右にある「 」を選択し、 **移動** からへ

   ![](assets/nwe-move-at-issue-level-highlighted-350x579.png)

   この **問題の移動** ボックスが表示されます。

   ![](assets/move-issue-box-nwe-350x280.png)

1. 内 **宛先プロジェクトを選択** 「 」セクションで、イシューを移動するプロジェクトの名前を指定します。 デフォルトでは、現在のプロジェクトの名前が表示されます。

   >[!TIP]
   >
   >リストには 100 個のプロジェクトのみが表示されます。

1. （条件付き）クリック **アクセスを要求** 問題をプロジェクトに移動するアクセス権がない場合。
1. （条件付き）宛先プロジェクトのタスクの 1 つにイシューを追加するアクセス権がある場合は、アクセス権を要求せずに、選択した宛先プロジェクトでイシューを引き続き移動します。

   ![](assets/move-issue-request-access-from-project-nwe-350x118.png)

   >[!TIP]
   >
   >Workfront管理者がこれらのプロジェクトに問題を追加できない場合、選択したプロジェクトが承認待ち、完了または無効の場合にも、同様のメッセージが表示されます。 詳しくは、 [システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. （オプション） **オプション** 「 」セクションで、以下の表に示す項目の選択を解除して、移動したイシューから削除します。 デフォルトでは、すべてのオプションが選択されています。

   >[!IMPORTANT]
   >
   >オプションリストで項目の選択を解除すると、データが失われます。 既存の問題からの情報は削除され、復元できません。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">すべて選択</td> 
      <td>このオプションの選択を解除すると、問題のすべての情報を新しい場所に移動する際に問題から削除します。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">割り当て</td> 
      <td>イシューに割り当てられているユーザー、ジョブの役割、またはチームを削除します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">進捗状況</td> 
      <td>問題の完了率（存在する場合）を削除します。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>ドキュメント</p></td> 
      <td> <p>ドキュメントのバージョン、リンクされたドキュメント、フォルダなど、ドキュメントタブ内のすべてを削除します。

   <b>メモ</b>

   問題と共にドキュメントを移動しないように選択した場合、ドキュメントは削除され、30 日間ごみ箱に入れられます。 管理者が復元できます。移動した問題で復元されます。

   問題が移動後に削除された場合、復元されたドキュメントは、復元元の管理者のユーザーページの「ドキュメント」領域に配置されます。
   <br> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">権限</td> 
      <td>イシューの共有先エンティティを削除します。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">更新</td> 
      <td>イシューの「更新」セクションからコメントを削除します。</td> 
     </tr> 
    </tbody> 
   </table>


1. （オプション） **タスクを選択** 「 」セクションで、イシューを移動するタスクを選択します。
1. クリック **問題の移動** または **問題を移動**&#x200B;リストで複数のイシューを選択した場合は、を選択します。

   移動された問題は、指定したプロジェクトに追加されます。




