---
filename: configure-backlog-workstream-board.md
content-type: reference
navigation-topic: boards
title: ワークストリームボード上のバックログの設定
description: ワークストリーム内のボードにバックログ列を表示することを選択し、ワークストリームカードリストからボードバックログに取り込まれるカードの問合せを定義できます。
author: Lisa
source-git-commit: b58831d50c2be421c666515808091aa4863bb471
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 1%

---

# ワークストリームボード上のバックログの設定

ワークストリーム内のボードにバックログ列を表示することを選択し、ワークストリームカードリストからボードバックログに取り込まれるカードの問合せを定義できます。 これらのオプションは、スタンドアロンボードでは使用できません。 スタンドアロンボードに取り込みカラムを追加する方法については、 [ボードに吸気柱を追加する](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計画*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL リクエスト ] 以降</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## ワークストリームボード上のバックログの設定

{{step1-to-boards}}

1. 作業するワークストリームを開きます。 ワークストリームを開くには、 [!UICONTROL **ワークストリームを表示**].
1. ワークストリーム内の任意のボードをクリックして開きます。
1. クリック [!UICONTROL **設定**] をクリックして、設定パネルを開きます。
1. オンにする [!UICONTROL **このボードにバックログ列を含める**].

   ボードの左側にバックログ列が追加されます。 クエリを適用するまで空白のままです。

1. 展開 [!UICONTROL **バックログクエリ**].
1. クリック [!UICONTROL **条件を追加**] 「空の」フィールドをクリックします。
1. クエリを実行するフィールドを選択します。

   カードのデフォルトのフィールドから選択できます。

1. クエリ修飾子を選択します。

   オプションは次のとおりです。等しい、等しくない、存在する、存在しない。

   例：「期限」を選択し、「存在する」を選択した場合、バックログには、期限が割り当てられたカードが表示されます。 期限のないカードは、バックログに取り込まれません。

1. 値を選択します。

   値は、修飾子として等しいまたは等しくないを使用する場合にのみ使用できます。

1. （オプション）「 [!UICONTROL **条件を追加**] をクエリに追加します。

   ![バックログクエリ](assets/backlog-query-wrkstrm-board.png)

1. （オプション）「 [!UICONTROL **グループ化**] をクリックして、OR 演算子で最初の条件に接続された条件のグループを追加します。
1. クリック [!UICONTROL **クエリを保存**].

   クエリが適用され、条件を満たすカードが「バックログ」列に表示されます。
