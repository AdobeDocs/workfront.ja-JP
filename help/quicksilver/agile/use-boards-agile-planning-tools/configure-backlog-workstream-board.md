---
filename: configure-backlog-workstream-board.md
content-type: reference
navigation-topic: boards
title: ワークストリームボードでのバックログの設定
description: ワークストリームのボードにバックログ列の表示を選択し、ワークストリームカードリストからボードバックログに取り込まれるカードのクエリを定義できます。
author: Lisa
feature: Agile
exl-id: fd2f6eeb-a565-4461-a153-0504ad3c07d7
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 96%

---

# ワークストリームボード上でバックログを設定

>[!IMPORTANT]
>
>ワークストリームは、特定の顧客グループのみが使用できます。

ワークストリームのボードにバックログ列の表示を選択し、ワークストリームカードリストからボードバックログに取り込まれるカードのクエリを定義できます。

>[!NOTE]
>
>クエリの条件に一致しない新しいカードをバックログ列に追加すると、ボードが更新されると、カードはバックログから消え、カードリストでのみ使用可能になります。クエリはいつでも変更でき、バックログ列に表示されるカードを調整できます。

バックログ列とクエリは、スタンドアロンボードでは使用できません。スタンドアロンボードに取り込み列を追加する方法について詳しくは、[ボードへの取り込み列の追加](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td> 
   <p>新規：[!UICONTROL Contributor]以上</p> 
   <p>または</p>
   <p>現在：[!UICONTROL Request] 以上</p>
   </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ワークストリームボード上でバックログを設定

{{step1-to-boards}}

1. 作業するワークストリームを開きます。ワークストリームを開くには、「[!UICONTROL **ワークストリームを表示**]」をクリックします。
1. ワークストリーム内の任意のボードをクリックして開きます。
1. ボードの右側にある「[!UICONTROL **設定**]」をクリックして、設定パネルを開きます。
1. 「[!UICONTROL **このボードにバックログ列を含める**]」をオンにします。

   ボードの左側にバックログ列が追加されます。この列は、クエリを適用するまで空白のままとなります。

1. [!UICONTROL **バックログクエリ**]&#x200B;を展開します。

   >[!NOTE]
   >
   >デフォルトのクエリがバックログに既に適用され、ステータスを持つカードリストおよびステータスが完了のカードリストのすべての作業アイテムが表示されている場合があります。

1. 「[!UICONTROL **条件を追加**]」をクリックして、「空」フィールド内をクリックします。
1. クエリを実行するフィールドを選択します。

   選択できるフィールドは、カードのデフォルトフィールドです。

1. クエリ修飾子を選択します。

   修飾子のオプションは、適用できるフィールドによって異なります。例えば、「名前」フィールドには、修飾子の選択肢として「より大きい」または「より小さい」はありません。これらの修飾子は数値にのみ適用されるからです。

1. 値を選択します。

   この値は、修飾子に「exists」または「not exists」を使用する場合は使用できません。

   例えば、「期限」と「存在」を選択した場合、バックログには期限が割り当てられたカードが表示されます。期限のないカードは、バックログに取り込まれません。

1. （オプション）「[!UICONTROL **条件を追加**]」をクリックして、クエリに別の条件を追加します。

   ![バックログクエリ](assets/backlog-query-wrkstrm-board.png)

1. （オプション）「[!UICONTROL **グループを作成**]」をクリックして、OR 演算子で最初の条件に接続された条件のグループを追加します。
1. 「[!UICONTROL **クエリを保存**]」をクリックします。

   クエリが適用され、条件を満たすカードがバックログ列に表示されます。
