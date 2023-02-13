---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: グループのステータスの作成または編集
description: グループ管理者は、管理対象のグループに対してカスタムステータスを作成できます。 これにより、多くの会社全体のカスタムステータスを不要にし、グループ階層でより自立性を高めることができます。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 75018e0e-ff74-4afb-9a99-34bbb39b6e14
source-git-commit: 027d636e8256c6a12d552af736884f6f27886114
workflow-type: tm+mt
source-wordcount: '1313'
ht-degree: 1%

---

# グループのステータスの作成または編集

グループ管理者は、管理対象のグループに対してカスタムステータスを作成できます。 これにより、多くの会社全体のカスタムステータスを不要にし、グループ階層でより自立性を高めることができます。

Workfrontの管理者がステータスのロックを解除した場合に、管理対象のグループのシステムレベルのステータスを編集することもできます。 詳しくは、 [システムレベルのステータスのロックとロック解除](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md).

グループの上にグループがある場合は、その管理者がグループに対してこれらの操作を実行することもできます。 Workfront管理者（すべてのグループ）も同様です。

>[!NOTE]
>
>プロジェクトをアジャイルビューで表示する場合、カスタムグループステータスはプロジェクトに表示できません。 プロジェクトをアジャイルビューで表示する場合、デフォルトおよびカスタムのロック済みステータスのみが表示されます。 プロジェクトのアジャイルビューのカスタマイズについては、「 [アジャイルビューの作成またはカスタマイズ](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) 記事内 [Adobe Workfrontの概要を表示](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

ステータスに関する一般的な情報については、 [ステータスの概要](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> <p>グループのグループ管理者またはWorkfront管理者である必要があります。 詳しくは、 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">グループ管理者</a> および <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプランまたはライセンスの種類を確認する必要がある場合は、Workfront管理者にお問い合わせください。

## グループのステータスの作成または編集

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **グループ** ![](assets/groups-icon.png).

1. ステータスを作成またはカスタマイズするグループの名前をクリックします。
1. 左側のパネルで、 **ステータス**.

   表示しているグループが最上位のグループの場合、表示されるリストには次の項目が含まれます。

   * システムレベルのロック済みステータス。
   * グループに対して既にカスタムステータスが作成されています。

   また、表示しているグループがサブグループの場合、リストには次も含まれます。

   * サブグループの上のグループに属するロック済みステータス。
   * サブグループの作成時にサブグループの上のグループに属していた、ロックが解除されたステータス。

      サブグループを作成した後は、その上のグループで作成されたロックが解除されたステータスは、サブグループのステータスリストに含まれません。 ただし、誰かがそのうちの 1 つを後でロックした場合、そのサブグループのステータスリストに含まれます。 詳しくは、 [グループのステータス継承方法](../../../administration-and-setup/manage-groups/manage-group-statuses/how-groups-inherit-statuses.md).


1. オブジェクトタイプのタブを選択します (**プロジェクト**, **タスク**&#x200B;または **問題**) をクリックします。

1. （条件付き）ステータスが問題ステータスの場合は、 **マスターリスト** が選択されている。

   ![](assets/master-list.png)

   その他の問題タイプ（バグレポート、変更管理、問題、リクエスト）のカスタマイズについては、 [デフォルトの問題タイプをカスタマイズ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

1. （条件付き）新しいステータスを作成するには、 **新しいステータスの追加**.

   または

   既存のステータスを編集するには、編集するステータスの上にマウスポインターを置いて、 **編集** 」オプションが表示されます。

   ![](assets/group-statuses-edit.jpg)

   >[!NOTE]
   >次の場合にのみ、グループのステータスを編集できます。
   >      
   >* ステータスが作成されたグループを管理します
   >* Workfrontの管理者が、システムレベルでステータスのロックを解除しました
   >* グループの上のグループのグループ管理者がステータスをロック解除しました

   >      
   >      
   >既存のステータスを編集する際、名前、説明、色のみを変更できます。
   >
   >ロック状態を編集すると、変更は、グループからステータスを継承したすべてのサブグループに影響を与えます。
   >   
   >逆に、ロックが解除された状態を編集しても、その状態をグループから継承したサブグループには影響しません。

1. 次の情報を指定します。

   ステータスを編集している場合、変更できるのは最初の 3 つの設定のみです。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">状態名</td> 
      <td> <p>ステータスの名前を入力します。 必須フィールドです。</p> <p>ステータス名を作成する場合、システム内の他のユーザーは同じ名前のステータスを作成できます。 Workfrontでステータスを選択する際に混乱が生じないように、一意の名前を使用することをお勧めします。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">説明</td> 
      <td>（オプション）ステータスの説明を入力します。 これは、その目的を使用する人々に伝えます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">色</td> 
      <td> <p>カラーフィールドをクリックし、スウォッチパネルから色を選択して、ステータスの色をカスタマイズします。 また、「 」フィールドに 16 進数を入力することもできます。</p> <p>ステータスの色は、ユーザーがオブジェクトを表示したときにWorkfrontの右上隅に表示されます。</p> <p> <img src="assets/status-color.png"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">同等</td> 
      <td> <p>ステータスの機能に最も適したオプションをリストから 1 つ選択します。 例えば、ステータス名が「完了」の場合、「完了」と等しいオプションを指定する必要があります。</p> <p>ステータスがどのように機能するかを決定するので、各ステータスは、これらのオプションのいずれかと同じにする必要があります。</p> <p>ステータスの作成後は、このオプションを変更できません。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">キー</td> 
      <td> <p>新しいステータスを作成する場合は、ステータスのコードまたは省略形を入力するか、生成したステータスを使用します。 このキーは、レポート目的で使用できるので、Workfrontで一意である必要があります。 システムで既に使用されているキーを指定しようとすると、フィールドが赤に変わります。</p> <p>使用するユーザーが認識可能な省略形を使用すると便利です。</p> <p>ステータスの作成後は、このオプションを変更できません。</p> <p>Planning、Current、Complete の各ステータスのキーコードは変更できません。 これは、テキストモードでレポートを作成する場合に重要です。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ステータスを非表示</td> 
      <td> <p>（プロジェクトおよびタスクのステータスのみ）</p> <p>ユーザーにステータスを表示しない場合は、このオプションを有効にします。 無効にした場合（デフォルト設定）、グループの下のすべてのサブグループがステータスを使用できます。</p> <p>ヒント：4 つの問題タイプ（バグレポート、変更管理、問題、リクエスト）をすべて無効にすると、問題ステータスを非表示にできます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">すべてのグループについてロック</td> 
      <td> 
       <p>このオプションを有効にしたままにすると、グループとそのサブグループ内のユーザーはステータスを表示して使用でき、グループ管理者は下位のサブグループをカスタマイズできなくなります。</p> 
       <p>このオプションを無効にすると、グループ管理者は下位のサブグループのステータスをカスタマイズできます。</p> 
       <p><b>注意</b>:グループ承認プロセスでは、ロック済みステータスとロック解除済みステータスの両方を使用できます。 ロックが解除されたグループステータスでグループ承認プロセスを作成した場合、ユーザーは、そのグループに関連付けられているプロジェクト、タスクまたはイシューに承認プロセスを添付できます。</p> 
       <p>ステータスのロックについて詳しくは、 <a href="../../../administration-and-setup/manage-groups/manage-group-statuses/lock-or-unlock-a-custom-group-status.md" class="MCXref xref">ロックおよびロック解除されたグループステータス</a>.</p> 
       </td> 
     </tr>
    </tbody> 
   </table>

1. 「**保存**」をクリックします。

   これで、グループまたはサブグループに関連付けられたすべてのプロジェクトでステータスが使用できます。 ロックした場合は、下位のサブグループで使用できます。

   ステータスをグループのデフォルトのステータスに設定できます。 詳しくは、 [カスタムステータスをグループのデフォルトのステータスとして使用する](../../../administration-and-setup/manage-groups/manage-group-statuses/use-custom-statuses-as-default-statuses-group.md).

## 複数のグループのカスタムステータスの作成

Workfrontの管理者は、複数のグループのカスタムステータスを作成できます。そのためには、システム全体のステータスを作成し、必要のないグループからそのステータスを非表示にします。

グループ管理者 ( またはWorkfront管理者 ) の場合は、管理するグループ階層内の複数のサブグループのカスタムステータスを作成できます。そのためには、上位のグループのステータスを作成し、必要のない下位のサブグループからそのステータスを非表示にします。

1. Workfront管理者の場合は、 [ステータスの作成または編集](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
1. 右上隅のボックスで、 **システムステータス**&#x200B;をクリックし、ステータスを非表示にするグループの名前を入力し、表示されたら名前をクリックします。
1. グループに表示しないステータスの上にマウスポインターを置いて、 **編集** 表示されたとき。

   ![](assets/hover-click-edit.jpg)

1. を有効にします。 **ステータスを非表示** 」オプションが表示されます。

   ![](assets/hide-group-status.png)

1. 「**保存**」をクリックします。

   ステータスは灰色表示になり、そのグループのすべてのユーザーには表示されなくなります。

1. 手順 3 ～ 5 を繰り返して、不要な他のグループに対してカスタムステータスを非表示にします。
