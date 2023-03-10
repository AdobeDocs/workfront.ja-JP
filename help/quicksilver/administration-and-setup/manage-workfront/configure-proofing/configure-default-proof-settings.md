---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: デフォルトの配達確認設定を構成
description: これらの設定を使用すると、ユーザーが作成するすべての新しい配達確認に適用されるデフォルト値を設定できます。 ただし、配達確認の作成時に、ユーザーがこれらの設定のほとんどを上書きできます。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: cfccb120-8759-49f2-8b7b-dabcd57d4fda
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 7%

---

# デフォルトの配達確認設定を構成

これらの設定を使用すると、ユーザーが作成するすべての新しい配達確認に適用されるデフォルト値を設定できます。 ただし、配達確認の作成時に、ユーザーがこれらの設定のほとんどを上書きできます。

## 新しい配達確認のデフォルト設定を構成

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定**.
1. 左側のパネルで、 **配達確認** > **配達確認の設定**.
1. 内 **新しい配達確認のデフォルト** セクションで、次の設定を行います。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader" colspan="2"><b>受信者</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">ログインが必要</td> 
      <td> <p>レビュー担当者は、組織のアカウントで作成した配達確認を表示できるようにする前に、電子メールとパスワードを使用してログインする必要があります。 有効にすると、ユーザーはゲストレビュー担当者と配達確認を共有できなくなります。</p> <p><b>重要</b>:有効にした場合、新しく作成されたすべての配達確認に対してログインが必要です。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">新しいバージョンのオリジナルの配達確認から所有者をコピー</td> 
      <td> <p>また、配達確認の最初のバージョンの所有者は、誰が作成したかに関係なく、配達確認の連続するすべてのバージョンの所有者にもなります。 この設定は、デフォルトで有効になっています。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ユーザーが配達確認のコメントを削除することを許可します</td> 
      <td>ユーザーは自分のコメントを削除できます。 この設定は、デフォルトで有効になっています。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">電子署名するには決定が必要です </td> 
      <td> <p>意思決定者は、配達確認を決定する際に、Workfrontのログイン資格情報を入力するよう求められます。</p> <p><b>重要</b>:有効にすると、ユーザーはログイン資格情報を持たないゲストレビュー担当者と配達確認を共有できなくなります。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"><b>期限</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">デフォルトの期限を設定</td> 
      <td> <p>自動ワークフローを持たないアカウント内のすべての新しい配達確認に、この期限が適用されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">配達確認がリスクにさらされる前に受信者に通知</td> 
      <td>上記の期限に応じて配達確認がアットリスクと見なされる前に、受信者に E メールで通知されます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"><b>メール通知</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">受信者が配達確認に追加されたとき受信者に通知する</td> 
      <td>受信者は、配達確認に追加されると、E メールで通知されます。</td> 
     </tr> 
    </tbody> 
   </table>

1. 「**保存**」をクリックします。

## 配達確認の決定を設定

ユーザーは、配達確認の決定を使用して、レビュー後の配達確認のステータスを示すことができます。

>[!NOTE]
>
>配達確認の決定の背後にあるロジックは、様々なレベルの複数の決定がある場合に、配達確認ワークフローの全体的なステータスを計算するために使用されます。 自動ワークフローの次の段階で、「承認済み」および「変更により承認済み」のトリガーが表示されます。

配達確認の決定を設定するには：

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定**.
1. 左側のパネルで、 **配達確認** > **配達確認の設定**.
1. 内 **決定**&#x200B;セクションで、以下の操作を実行できます。

   1. **決定の名前を変更**:決定ボックス内のテキストをクリックし、新しい決定ラベルを入力します。

      >[!TIP]
      >
      >決定のロジックは、名前を変更する際に保持します。 例えば、デフォルトの「却下」の決定をに変更できます。 *新しいバージョンが必要です*&#x200B;に変更する必要はありませんが、 *プリンタに送信*.

      ![](assets/rename-decision-350x109.png)

   1. **決定順序の並べ替え**:判定ボックスを、校正ビューアに表示する順序にドラッグします。

      ![](assets/move-decision-350x110.png)

   1. **決定を非表示にする**:決定ボックスの上にマウスポインターを置き、右上隅の非表示アイコンをクリックします。

      ![](assets/hide-decision-350x109.png)

1. （オプション） Workfrontのデフォルトに戻るには、 **デフォルトに戻す**.
1. 「**保存**」をクリックします。
