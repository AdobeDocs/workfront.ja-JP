---
title: カスタム条件の作成または編集
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Adobe Workfront 管理者は、組織のニーズに合わせて、プロジェクト、タスクおよびイシューのカスタム条件を作成または編集できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5c950862-4358-4aab-997b-223972662150
source-git-commit: a3cb3d9d340d377e301c98480324bfe8bf507382
workflow-type: ht
source-wordcount: '640'
ht-degree: 100%

---

# カスタム条件の作成または編集

Adobe Workfront 管理者は、組織のニーズに合わせて、プロジェクト、タスクおよびイシューのカスタム条件を作成または編集できます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront ライセンス</td> 
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p> <p><b>メモ</b>：まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## カスタム条件の作成または編集

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)、**設定** ![](assets/gear-icon-settings.png) の順にクリックします。

1. **プロジェクト環境設定**／**条件**&#x200B;をクリックします。

1. 条件に関連付けるオブジェクトタイプ（**プロジェクト**、**タスク**&#x200B;または&#x200B;**イシュー**）のタブをクリックします。

1. 新しい条件を作成するには、「**新規条件を追加**」をクリックします。

   または

   既存の条件を編集するには、編集する条件にポインタを合わせ、右端に表示される&#x200B;**編集**&#x200B;アイコンをクリックします。

   ![](assets/custom-condition-edit-nwe.jpg)

1. 次のオプションを使用して、カスタム条件を設定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>条件名</td> 
      <td>（必須）条件のわかりやすい名前を入力します。</td> 
     </tr> 
     <tr> 
      <td>説明</td> 
      <td>（オプション）条件を使用するユーザー向けに、条件の目的の説明を入力します。</td> 
     </tr> 
     <tr> 
      <td>色</td> 
      <td>（オプション）色アイコンをクリックし、プロジェクト、タスクまたはイシューに表示される際の条件の色を選択します。16 進数を入力することもできます。</td> 
     </tr> 
     <tr> 
      <td>同等 </td> 
      <td><p>（プロジェクトの場合のみ必須）新しい条件の機能を最もよく記述するオプションをドロップダウンリストでクリックします。例えば、「Tracking Well」という名前の条件の場合に「目標どおり」をクリックするといった具合です。これにより、デフォルト条件がどのように機能するかが決まります。作成する条件はどれも、ドロップダウンメニューのオプションのいずれかと一致する必要があります。</p>
      <p>デフォルト条件については、<a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md" class="MCXref xref">カスタム条件をプロジェクトのデフォルトとして設定</a>および<a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md" class="MCXref xref">カスタム条件をタスクとイシューのデフォルトとして設定</a>を参照してください。</p>
      <p>条件の作成が終了した後は、このオプションを変更できません。</p></td> 
     </tr> 
     <tr> 
      <td>キー</td> 
      <td><p>（必須）プロジェクト条件の場合は、ユーザーが認識できる英数字の略語を入力します。タスク条件またはイシュー条件の場合は、01～99 の 2 桁の数値コードを入力します。 </p>
      <p>このキーは API で使用され、レポート目的で使用できるもので、オブジェクトごとに一意である必要があります。</p>
      <p>条件を保存した後は、条件のキーを変更することはできません。 </p></td> 
     </tr> 
     <tr> 
      <td>条件を非表示</td> 
      <td><p>（オプション）このオプションは、ユーザー用ではなくなったが、歴史的な理由で残しておくカスタム条件に使用できます。 </p>
      <p>作業アイテムで使用されてきたカスタム条件を非表示にした場合、その条件は非表示にした後も、それらの作業アイテムに引き続き表示されます。 </p></td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >条件の用語と色は、3 つのオブジェクトタイプすべてにわたって標準化できます。それには、条件名と色の 16 進コードを、1 つのタブ（「プロジェクト」、「タスク」、「イシュー」）から他の 2 つのタブの対応する条件にコピーします。

1. （オプション）任意の条件を新しい位置にドラッグ ![](assets/move-icon---dots.png) して、リストを並べ替えます。

   これにより、プロジェクト、タスクおよびイシューでの条件の表示順序が変わります。

   * ユーザーがプロジェクトを編集する場合：

     ![](assets/change-condition-edit-project.png)

   * ユーザーが「更新」タブでタスクまたはイシューの条件を変更する場合：

     ![](assets/change-condition-update-comment.png)

   * ユーザーがリスト表示でタスクまたはイシューの条件を変更する場合

     ![](assets/change-conditions-list-dropdown-only.png)

1. 「**保存**」をクリックします。

カスタム条件を、プロジェクトや、タスクおよびイシューのデフォルト条件として設定できます。詳しくは、[カスタム条件をプロジェクトのデフォルトとして設定](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md)および[カスタム条件をタスクとイシューのデフォルトとして設定](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md)を参照してください。

カスタム条件について詳しくは、[カスタム条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md)を参照してください。
