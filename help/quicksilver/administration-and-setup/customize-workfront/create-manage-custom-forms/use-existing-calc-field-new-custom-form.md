---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: レガシーフォームビルダーを使用して、カスタムフォーム内の既存の計算カスタムフィールドを再利用
description: 異なるオブジェクトに属するカスタムフォームでも、同じ計算済みカスタムフィールドを使用できます。例えば、プロジェクトカスタムフォーム用に作成した利益計算フィールドを、タスクカスタムフォームで使用できます。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 24482fca-94e4-406d-9d62-3db9f51481e6
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 100%

---

# レガシーフォームビルダーを使用して、カスタムフォーム内の既存の計算カスタムフィールドを再利用

{{form-designer-default}}

異なるオブジェクトに属するカスタムフォームでも、同じ計算済みカスタムフィールドを使用できます。例えば、プロジェクトカスタムフォーム用に作成した利益計算フィールドを、タスクカスタムフォームで使用できます。

計算カスタムフィールドをカスタムフォームに追加する方法について詳しくは、[レガシーフォームビルダーを使用して計算データをカスタムフォームに追加](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)を参照してください。

既存の計算カスタムフィールドを使用する場合、計算は新しいフォームに転送されません。同じフィールドの新しいカスタムフォームに、計算を再度追加する必要があります。

>[!TIP]
>
>これは、カスタムフォームヘルプの&#x200B;**指示**&#x200B;フィールドに保存されている計算を使用する場合です。

新しいフォーム上で、同じフィールドに対して別の計算を行うこともできます。計算カスタムフィールドに同じ名前を付けると、命名規則で纏りと一貫性を保つことができます。

>[!IMPORTANT]
>
>計算済みカスタムフィールドは、時間の経過と共に古くなる場合があります。これらのフィールドで常に最新の計算を表示するには、以下の操作のいずれかを行います。
>
>* 添付されたカスタムフォームでデータを編集したオブジェクトを保存したら、オブジェクトのメインページでその他アイコン ![](assets/more-icon.png) をクリックし、「カスタム式を再計算」をクリックします。
>* オブジェクトを一括編集する際に、「カスタム式を再計算」オプションを選択します。
>* カスタムフォームで計算カスタムフィールドを編集する場合は、「以前の計算を更新」オプションを選択します。
>
