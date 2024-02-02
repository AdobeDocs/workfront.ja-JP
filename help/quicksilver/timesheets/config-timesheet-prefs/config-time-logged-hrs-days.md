---
product-area: timesheets;setup
navigation-topic: configure-timesheet-preferences
title: 時間単位または日単位で時間を記録するよう設定
description: プランライセンスを持つユーザーは、Adobe Workfront で時間を時間数と日数のどちらで記録するかを設定できます。システム管理者は、個々のユーザーに対して、または組織内の複数のユーザーに対して、この設定を指定できます。デフォルトでは、ユーザーは時間単位で記録します。
author: Alina
feature: Timesheets
exl-id: 4f801a13-182d-4e06-98ea-f6863f6a8edf
source-git-commit: b4ab350af22afa44774f06d82daf1c3fb266d2b9
workflow-type: ht
source-wordcount: '451'
ht-degree: 100%

---

# 時間単位または日単位で時間を記録するよう設定

プランナーライセンスを持つユーザーは、Adobe Workfront で時間を時間数と日数のどちらで記録するかを設定できます。システム管理者は、個々のユーザーに対して、または組織内の複数のユーザーに対して、この設定を指定できます。デフォルトでは、ユーザーは時間単位で記録します。Workfront で時間を記録する方法について詳しくは、[時間を記録](../../timesheets/create-and-manage-timesheets/log-time.md)を参照してください。

>[!NOTE]
>
>レポートの正確性を確保するため、組織全体で同じ方法（時間数または日数）で時間を記録することをお勧めします。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>プラン </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プランナーは、自分で時間を設定できます。他のユーザーの時間を設定できるのは、Workfront 管理者のみです。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。

1. 目的と、システムでのアクセスレベルに応じて、次のいずれかの操作を行います。

   * **プランナーユーザーが自分用に時間の記録方法を設定：** Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、プロフィール画像の横にあるユーザー名をクリックします。次に、名前の横にある&#x200B;**その他**&#x200B;アイコンをクリックし、「**編集**」を選択します。

   * **システム管理者が他のユーザー用に時間の記録方法を設定：**[ユーザーのプロファイルの編集](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)の説明に従って、1 つ以上のユーザーアカウントの編集を開始します。

1. 表示されたダイアログボックスの「**リソース計画**」セクションで、「**時間を記録する単位**」オプションを見つけます。

   ![](assets/new-timesheet-log-hours-350x249.png)

1. （条件付き）システム管理者が複数のユーザーを同時に編集する場合は、「**時間を記録する単位**」を選択します。
1. 時間の記録に関する次のオプションから選択します。

   | オプション | 説明 |
   |---|---|
   | **時間** | Workfront で時間を記録するときに時間数を指定します。 |
   | **日** | Workfront で時間を記録するときに日数を指定します。 |

1. （条件付き）日数で時間を記録することを選択した場合は、「**一就業日と同等の時間数**」フィールドに、丸 1 日と等しい時間数を入力します。ユーザーのタイムシートの 1 日は、ここに入力した時間数と同じです。

   この設定を指定する際は、次の点を考慮してください。

   * このオプションは、時間を時間数で記録するように設定する場合は使用できません。
   * このオプションは、時間を記録する目的でのみ使用されます。このオプションは、ユーザーを編集するときにも使用できる「**スケジュール**」オプションとは関係ありません。「**スケジュール**」オプションは、タイムラインの計算時や、Workfront の他のエリアで使用されます。（「**スケジュール**」オプションの使用について詳しくは、[スケジュールの作成](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)を参照してください）。

1. 「**変更を保存**」をクリックします。
