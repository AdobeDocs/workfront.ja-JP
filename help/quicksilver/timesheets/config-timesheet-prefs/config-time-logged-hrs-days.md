---
product-area: timesheets;setup
navigation-topic: configure-timesheet-preferences
title: 時間単位または日単位で時間を記録するよう設定
description: プランライセンスを持つユーザーは、Adobe Workfront で時間を時間数と日数のどちらで記録するかを設定できます。システム管理者は、個々のユーザーに対して、または組織内の複数のユーザーに対して、この設定を指定できます。デフォルトでは、ユーザーは時間単位で記録します。
author: Lisa
feature: Timesheets
exl-id: 4f801a13-182d-4e06-98ea-f6863f6a8edf
source-git-commit: b0a3a11a3c04a0969bee99f8e1cea231911f0e6a
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 72%

---

# 時間単位または日単位で時間を記録するよう設定

Standard ライセンスまたは Plan ライセンスを持つユーザーは、Adobe Workfrontに時間を数時間または数日のどちらでログインするかを設定できます。 システム管理者は、個々のユーザーに対して、または組織内の複数のユーザーに対して、この設定を指定できます。デフォルトでは、ユーザーは時間単位で記録します。Workfrontに時間をログ記録する方法について詳しくは、[&#x200B; 時間をログに記録 &#x200B;](../../timesheets/create-and-manage-timesheets/log-time.md) を参照してください。

>[!NOTE]
>
>レポートの正確性を確保するため、組織全体で同じ方法（時間数または日数）で時間を記録することをお勧めします。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td>
   <p>標準</p>
   <p>プラン</p></td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td><p>標準およびプランのユーザーは、自分で時間を設定できます。 他のユーザーの時間を設定できるのは、Workfront 管理者のみです。</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

1. 目的と、システムでのアクセスレベルに応じて、次のいずれかの操作を行います。

   * **標準ユーザーまたはプランユーザーが自分の時間ログを設定：** Adobe Workfrontの右上隅にある **[!UICONTROL メインメニュー]** アイコン ![&#x200B; メインメニュー &#x200B;](assets/main-menu-icon.png) をクリックし、プロファイル画像の横にあるユーザー名をクリックします。 または（利用可能な場合は）上部のナビゲーション領域で自分のプロフィール写真をクリックし、**[!UICONTROL Workfrontのプロフィール]** をクリックします。 次に、名前の横にある&#x200B;**その他**&#x200B;アイコンをクリックし、「**編集**」を選択します。

   * **システム管理者が他のユーザー用に時間の記録方法を設定：**&#x200B;[ユーザーのプロファイルの編集](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)の説明に従って、1 つ以上のユーザーアカウントの編集を開始します。

1. 表示されたダイアログ・ボックスの「**Resource Planning**」セクションで、「**Log time in**」オプションを探します。

   ![&#x200B; 時間をオプションで記録 &#x200B;](assets/user-profile-log-time-options.png)

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
