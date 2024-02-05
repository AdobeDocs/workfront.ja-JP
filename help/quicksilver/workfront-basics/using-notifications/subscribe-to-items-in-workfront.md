---
navigation-topic: notifications
title: Adobe Workfront の項目を購読
description: Adobe Workfront では、ユーザーが割り当てられているアイテムや、ユーザーが所有しているアイテムに関する通知をユーザーに送信します。自分には割り当てられていないが、自分の作業に影響を与える可能性のあるアイテムについてのコミュニケーションをフォローする場合、ユーザーはそのアイテムに登録できます。
author: Lisa
feature: Get Started with Workfront
exl-id: 5eee62b8-d72e-4263-a0c5-749047bc6812
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1574'
ht-degree: 99%

---

# [!DNL Adobe Workfront] でのアイテムへの登録

[!UICONTROL Adobe Workfront] では、ユーザーが割り当てられているアイテムや、ユーザーが所有しているアイテムに関する通知をユーザーに送信します。自分には割り当てられていないが、自分の作業に影響を与える可能性のあるアイテムについてのコミュニケーションをフォローする場合、ユーザーはそのアイテムに登録できます。

また、ユーザーは、自分が[!UICONTROL 管理]および[!UICONTROL 共有]権限を持つアイテムの更新ステータスに管理者や同僚を登録することで、自分の作業の最新情報を管理者や同僚に絶えず知らせることができます。

現在、次のアイテムに登録できます。

* イシュー
* タスク
* プロジェクト

イシュー、タスクまたはプロジェクトに登録すると、誰かがそれらのアイテムにコメントを投稿したときにアプリ内通知が届きます。有効にしてある機能によっては、登録したアイテムに関するメール通知やモバイルアプリのプッシュ通知を受け取る場合もあります。

>[!NOTE]
>
>登録したアイテムで発生する他のイベントについては、通知を受け取りません。誰かがそのアイテムにコメントを投稿したときにのみ通知を受け取ります。

登録の操作について詳しくは、[登録の操作について](#about-working-with-subscriptions)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Adobe Workfront] プラン*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL Request] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>[!DNL Workfront] 管理者が、ユーザーのアクセスレベルで「<strong>[!UICONTROL View only updates in which they have been included in the conversation]</strong>」を有効にしてある場合、ユーザーは [!DNL Workfront] のアイテムに登録できません。</p> <p>メモ：それでもアクセスできない場合は、アクセスレベルに追加の制限が設定されているかどうかを [!UICONTROL Workfront] 管理者にお問い合わせください。[!UICONTROL Workfront] 管理者がユーザーのアクセスレベルを変更する方法については、<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>（登録する）プロジェクト、タスクまたはイシューへの[!UICONTROL View]アクセス権またはそれ以上の権限</p> <p>（他のユーザーを登録する）プロジェクト、タスクまたはイシューへの[!UICONTROL Manage]アクセス権および[!UICONTROL Share]権限</p> </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## アイテムに登録

アイテムに登録するプロセスは、どのアイテムでも同じです。

例えば、イシューに登録する手順は次のとおりです。

1. 登録するイシューに移動します。

   >[!TIP]
   >
   >プロジェクトに登録するには、次のいずれかを行います。
   >
   >* 登録するプロジェクトに移動し、プロジェクト名の右側にある&#x200B;**[!UICONTROL その他]**&#x200B;アイコン ![](assets/qs-more-menu.png) をクリックしたあと、「**[!UICONTROL 登録]**」をクリックします。
   >* プロジェクトリストまたはレポートに移動してプロジェクトを選択し、リストの上部にある&#x200B;**[!UICONTROL その他]** アイコン ![](assets/qs-more-menu.png) をクリックしたあと、「**[!UICONTROL 登録]**」をクリックします。これは、プロジェクトのリストでのみ使用できます。

1. **[!UICONTROL その他]**&#x200B;アイコン ![](assets/more-icon.png) をクリックしたあと、「**[!UICONTROL 登録]**」をクリックします。

   ![](assets/subscribe-to-a-work-item-350x258.png)

   ベルにチェックマークが表示され、その横の番号が更新されて、登録済みユーザー数に追加されます。

   これで、イシューに登録しました。イシューに登録したことがイシューの更新ステータスに記録されます。

   誰かがイシューにコメントするたびに、アプリ内通知が届きます。有効にしてある機能によっては、メール通知やモバイルアプリのプッシュ通知を受け取る場合もあります。

   購読電子メールについて詳しくは、 [独自の電子メール通知を変更する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## アイテムから登録解除

[!DNL Workfront] のアイテムから簡単に登録解除できます。[!DNL Workfront] のアイテムからの登録解除のプロセスは、どのアイテムでも同じです。

例えば、イシューから登録解除するには、次の手順に従います。

1. 登録解除するイシューに移動します。

   >[!TIP]
   >
   >プロジェクトへの登録を解除するには、次のいずれかの操作を実行します。
   >
   >* 登録解除元のプロジェクトに移動し、プロジェクト名の右側にある&#x200B;**[!UICONTROL その他]**&#x200B;アイコン ![](assets/qs-more-menu.png) をクリックして、「**[!UICONTROL 登録解除]**」をクリックします。
   >* プロジェクトリストまたはレポートに移動して、プロジェクトを選択し、リストの上部にある&#x200B;**[!UICONTROL その他]**&#x200B;アイコン ![](assets/qs-more-menu.png) をクリックして、「**[!UICONTROL 登録解除]**」をクリックします。これは、プロジェクトのリストでのみ使用できます。

1. 「**[!UICONTROL その他]**」![](assets/more-icon.png) をクリックしてから、「**[!UICONTROL 登録解除]**」をクリックします。

   ![](assets/unsubscribe-to-a-work-item-350x258.png)

1. 登録メールにある「[!UICONTROL 登録解除]」リンクをクリックして、登録している項目から登録解除することもできます。

   項目への登録を解除すると、そのイシューに対して誰かがコメントをした際に通知が届かなくなります。

   項目の更新ステータスに、イシューへの登録の解除が記録されます。

## サブスクライバーの管理

管理権限および共有権限を持つプロジェクト、タスクおよびイシューへのサブスクライバーを管理できます。

* [他のユーザーを項目に登録](#subscribe-another-user-to-an-item)
* [他のユーザーを項目から登録解除](#unsubscribe-another-person-from-an-item)

すべてのサブスクライバーには、登録項目に対する[!UICONTROL 表示]権限が付与されます。新しいサブスクライバーが既にその項目に対する権限を持っている場合は、その権限が維持されます。

### 他のユーザーを項目に登録

1. 他のユーザーを登録する項目に移動します。

   >[!TIP]
   >
   >他のユーザーをプロジェクトに登録するには、次のいずれかの操作を実行します。
   >
   >* 他のユーザーを登録するプロジェクトに移動するか、
   >   
   >* プロジェクトリストまたはレポートに移動し、プロジェクトを選択します。

1. **[!UICONTROL その他]**![](assets/more-icon.png)をクリックします。
1. **[!UICONTROL 登録]**&#x200B;リンクの横にある数字の吹き出しをクリックします。
1. 表示されるボックスで、「**[!UICONTROL 他のユーザーを登録]**」ボックスにユーザーの名前を入力し、表示されたオプションからユーザーを選択します。

1. （オプション）サブスクライバーをさらに追加するには、手順 4 を繰り返します。
1. 「**[!UICONTROL 保存]**」をクリックします。

サブスクライバーに登録の通知は送信されませんが、登録に関するエントリが項目のシステム更新に追加されます。

他のユーザーが項目の「[!UICONTROL 更新]」タブにコメントを追加すると、サブスクライバーはアプリ内通知を受け取ります。Workfront 管理者が有効にした機能に応じて、サブスクライバーが項目に関するメールおよびモバイル通知を受信することもできます。

### 他のユーザーを項目から登録解除

1. 他のユーザーを登録解除する項目に移動します。

   >[!TIP]
   >
   >他のユーザーをプロジェクトから登録解除するには、次のいずれかの操作を実行します。
   >
   >* 他のユーザーを登録解除するプロジェクトに移動するか、
   >   
   >* プロジェクトリストまたはレポートに移動し、プロジェクトを選択します。

1. **[!UICONTROL その他]** ![](assets/more-icon.png) をクリックします。
1. **[!UICONTROL 登録]**&#x200B;リンクまたは&#x200B;**[!UICONTROL 登録解除]**&#x200B;リンクの横にある数字の吹き出しをクリックします。
1. 表示される&#x200B;**[!UICONTROL サブスクライバー]**&#x200B;ページで、登録解除するユーザー名の横にある「X」をクリックします。

   または

   「**[!UICONTROL リスト内のユーザーを検索]**」ボックスにユーザーの名前を入力し、ユーザー名の右側にある「X」をクリックします。

1. 「**[!UICONTROL 保存]**」をクリックします。

   ユーザーに項目の登録解除の通知は送信されませんが、登録に関するエントリが項目のシステム更新に追加されます。

## アプリ内通知を受信

登録している項目に他のユーザーがコメントを投稿すると、すぐにアプリ内通知が届きます。

![](assets/in-app-not---cmmnt-sbscibd-to-350x164.png)

詳しくは、[アプリ内通知の表示と管理](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md)を参照してください。

## 登録メールを受信

[!UICONTROL Workfront] 管理者が有効にした機能に応じて、登録している項目に他のユーザーがコメントするたびに、アプリ内通知に加えて登録メールを受信することができます。

メールの設定または無効化について詳しくは、[システム内の全員に対するイベント通知の設定](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)を参照してください。

>[!NOTE]
>
>登録メールをオフにしても、登録している項目に他のユーザーがコメントするたびに、引き続きアプリ内通知が届きます。

## 項目に登録しているユーザーをリスト表示

項目のサブスクライバーを確認するには、次の操作を行います。

1. サブスクライバーを表示する項目に移動します。

   項目にサブスクライバーがいる場合は、サブスクライバーの数がベルの横に表示されます。この数にポインタを合わせると、その項目に登録しているユーザーのリストが表示されます。最初の 25 人のサブスクライバーがアルファベット順に表示されます。

   ![サブスクライバーを表示](assets/bell-hover-for-list-qs-350x90.png)

   「[!UICONTROL サブスクライバー]」フィールドをレポートまたは購読済みの項目のビューの列として追加することで、サブスクライバーのリストを表示することもできます。詳しくは、[ 用語集の [!DNL Adobe Workfront] 用語](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)を参照してください。

## 購読に関する作業について

購読に関する作業を行う場合は、次の点を考慮してください。

* [!DNL Workfront] 管理者は、ユーザーが購読可能または購読不可能な項目を制御できません。

  タスク、イシューまたはプロジェクトに対する[!UICONTROL 表示]以上の権限を持つユーザーは誰でも購読できます。

* 日次ダイジェストメールの購読を設定することはできません。
* タスク、イシューまたはプロジェクトを購読し、自分が担当者、主連絡先またはプロジェクト所有者である場合は、購読している項目に他のユーザーがコメントしたときにのみ購読メールが届きます。

  項目のいずれかに対してコメントが投稿された際にトリガーされるメール通知について詳しくは、[Adobe Workfront 通知](../../workfront-basics/using-notifications/wf-notifications.md)を参照してください。

* 項目を購読してコメントを投稿した場合、コメントに自分の名前を含めない限り、そのコメントに関する購読メールは届きません。
* 項目にコメントしたユーザーがコメントをロックして非公開に設定した場合、そのユーザーと同じ会社に所属していないユーザーにそのコメントの通知は届きません。コメントを自社で非公開にする方法について詳しくは、[作業の更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)の[作業項目に更新を追加](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add)の節を参照してください。

* 購読用のレポートを作成することはできません。監査は、項目が購読または購読解除されたときに、すべての項目の更新ステータスに記録されます。
* 子オブジェクトへのコメントは、親オブジェクトの購読通知をトリガーしません。プロジェクトを購読する場合、そのプロジェクトに対するコメントの通知のみを受け取ります。プロジェクトに関連付けられた子項目（タスクやイシュー）に対するコメントの通知は、それぞれの子項目を購読しない限り受け取りません。オブジェクトの関係について詳しくは、「[ [!DNL Adobe Workfront]](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) でのオブジェクトについて」の[オブジェクトの相互依存性と階層](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects)の節を参照してください。
