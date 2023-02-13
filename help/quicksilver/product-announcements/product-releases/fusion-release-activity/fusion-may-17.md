---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: '''Workfront Fusion リリースアクティビティ：2021 年 5 月 17 日の週'
description: このページでは、2021 年 5 月 17 日の週にAdobe Workfront Fusion でおこなわれたすべての機能強化について説明します。
author: Luke
feature: Product Announcements, Workfront Fusion
exl-id: 930c335e-2c88-41af-983f-82be790c1a4b
hidefromtoc: true
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 0%

---

# Workfront Fusion リリースアクティビティ： 2021 年 5 月 17 日の週

このページでは、2021 年 5 月 17 日の週にAdobe Workfront Fusion でおこなわれたすべての機能強化について説明します。

最近のすべての変更の一覧については、 [Adobe Workfront Fusion リリースアクティビティ](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Workfront Fusion の最近のバグ修正の一覧については、 [Workfrontメンテナンスの更新](https://one.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350) ページを開き、 Workfront Fusion メンテナンスアップデートというラベルの付いたアップデートがないか確認します。

## Workfront Fusion シナリオでのモジュールのコピー

Workfront Fusion シナリオの操作を容易にするために、モジュールのコピーと貼り付けを実行できました。 モジュールまたはモジュールのグループをコピーして、同じシナリオまたは別のシナリオに貼り付けることができます。 モジュールをコピーしても、そのモジュールのフィールド値は保持されます。

詳しくは、 [Adobe Workfront Fusion でのモジュールまたはシナリオのコピー](../../../workfront-fusion/scenarios/copy-modules-or-scenarios.md).

## Workfront Fusion シナリオでの複数のモジュールの選択

現在は、シナリオの編集時に、一度に複数のモジュールを選択できます。 その後、選択したモジュールに対してバルクアクションを実行できます。

* コピー
* 移動
* 削除

モジュールのコピーと移動は、モジュールの値とモジュールを接続するすべての線を保持します。

シナリオの編集について詳しくは、 [Adobe Workfront Fusion でシナリオを作成する](../../../workfront-fusion/scenarios/create-a-scenario.md).

## モジュールで未保存の情報が保持されるようになりました

シナリオを簡単に作成できるように、モジュールで、フォーカスがないときにフィールド値を保持できるようにしました。 ここで、保存せずにモジュールの外側をクリックし、そのモジュールに戻ると、フィールドには以前に入力した値が表示されます。 モジュールが閉じると、未保存のフィールドがあることを示すインジケーターが表示されます。

## Azure AD コネクタで、新しいレコードと更新されたレコードが別々に処理されるようになりました

新しいレコードと既存のレコードの更新が、別々のモジュールで処理されるようになりました。

* 新しいレコードを監視するには、「レコードを監視トリガー」モジュールを使用します。 このモジュールは、更新されたレコードを監視しなくなりました。
* 新しいユーザー/グループの検索デルタモジュールを使用して、更新されたレコードを取得できます。 このモジュールは、新しいレコード、更新されたレコード、削除されたレコードを返します。

詳しくは、 [Azure Active Directory モジュール](../../../workfront-fusion/apps-and-their-modules/azure-ad-modules.md).
