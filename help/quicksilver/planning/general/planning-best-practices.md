---
title: Adobe Workfrontの計画のベストプラクティス
description: マーケティング業務のリーダーとして、Adobe Workfront Planning を使用すると、すべてのチームのマーケティングライフサイクル全体の作業を整理できます。Workfrontの計画を始める際には、いくつかのベストプラクティスをお勧めします。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 6e039b80-e3bf-412c-8c86-8f801f5861e3
source-git-commit: 0e37a5a519770d3d48192f1799491aa53a871508
workflow-type: tm+mt
source-wordcount: '3344'
ht-degree: 2%

---

<!--drafted because Kari Woolf will write something for Field Readiness instead, nothing for ExL, public-facing documentation-->

# Adobe Workfrontの計画のベストプラクティス

<!-- add to TOC and mini TOC-->

{{planning-important-intro}}

マーケティング業務のリーダーとして、Adobe Workfront Planning を使用すると、すべてのチームのマーケティングライフサイクル全体の作業を整理できます。

この記事では、Workfrontの計画を始める際に推奨するよくある質問とベストプラクティスについて説明します。

## 設定のベストプラクティス

### ワークスペース

ワークスペースは、チームが作業を計画するための一元的な場所です。 ワークスペースは、チームが使用するレコードタイプのコレクションで、チームの作業ライフサイクルを表します。

Workfront Planning の構成に関するよくある質問を次に示します。

#### 何から始めればいいですか。

* ✅ Planning に初めてログインする場合は、Planning の価値を明確に伝え、製品を効果的にナビゲートして利用する方法をガイドするアプリ内オンボーディングプロセスに従ってください。 これにより、その機能と、作業を簡単に開始する方法を理解できるようになります。
* ✅ まず、既存の類似したユースケースのアイデアに対する事前定義済みのワークスペーステンプレートを調べます。 テンプレートに含まれる定義済みのレコードタイプ、フィールドを使用するか、自分で追加することができます。
* ✅ Workfront Planning で解決する主なユースケースを特定します。 例えば、ほとんどの組織は、より優れた「キャンペーンカレンダー」の構築など、戦略的活動の可視性を向上したいと考えています。 したがって、そのユースケースでは、まず次のいくつかの質問に答えることにします。

   * 誰が要求しているの？
   * カレンダーに入れたいものを何と呼びますか？
キャンペーン？ 戦術？ 取り組み？ 活動？ イベント？
   * このカレンダーに関してどのような質問に答えたいですか？
   * 同じオーディエンスに対して重複するキャンペーンはありますか？
   * そのキャンペーン、戦術、アクティビティまたはイベントの予算はどれくらいですか？

  これらの質問に対する回答は、Workfront Planning 内で何を構築する必要があるかを示します。

  また、現在Workfrontを使用していない他のプランナーがいる可能性も考慮してください。 これらのプランナーは、Excel スプレッドシート、Word ドキュメント、PowerPoint プレゼンテーションなどで動作する場合があります。 顧客がWorkfront Planning 内の情報にアクセスする方法を検討します。

* ✅ Workfront Planning を最大限に活用するには、Workfront Planning で、Workfrontのポートフォリオとプログラムを他の上位階層構造に置き換えることを検討してください。

  現在、Workfrontのお客様は、ポートフォリオやプログラムを通じて戦略的作業を表し、場合によっては異なるタイプのプロジェクトとして表します。 Planning の導入により、このような戦略的作業はすべてWorkfront Planning のカスタムレコードタイプで処理する必要がありますが、Workfrontはプロジェクトやタスクとして表される作業の実行段階を中心としています。

#### 既存のワークスペースの変更に対して、新しいワークスペースはどのような場合に作成する必要がありますか？

* 組織レベルのワークスペースのボリュームが最も少ない場合は、「✅ Design」を選択します。 各ユニットのユニークな動作方法に合わせて、特定の運用組織ユニットのワークスペースを作成できます。

  1 つのWorkspaceに情報を保持することで、すべてのデータ間の関係を容易に管理できるようにします。

  例えば、すべてのマーケティングに対して 1 つのワークスペースを作成しようとします。

  完全に異なる操作構造を持つチーム用に、新しいワークスペースを作成しても問題ありません。

  例えば、**製品開発** ワークスペースは、**マーケティング** ワークスペースとは異なる必要があります。

* ⛔ 組織内のチームまたはプロセスごとに一意のワークスペースを作成しないでください。

  マーケティング組織は、可視性を維持し、グローバルな計画レベルでデータをロールアップできるように、ワークスペースを 1 つだけ維持するように努める必要があります。

  類似のプロセスに従うチーム（例えば、EMEA マーケティングと APAC マーケティングなど）に対しては、類似したワークスペースや重複したワークスペースを作成しないでください。特に、これらのチームが共通の戦略的キャンペーンを前に進める作業を行う可能性がある場合には、避けます。

#### Workspace セクションの使用方法は？

* 「作成」セクションと「ラベル付け」セクションを ✅ 照すると、運用ライフサイクルを整理する方法をユーザーが理解しやすくなります。

  例えば、「**コアレコード** というセクションを作成して、キャンペーン、戦術、成果物をワークスペースに配置できます。
* ✅ の「類似」レコードタイプをグループ化します。

  たとえば、地域、国、市区町村などのレコードの種類を含む **地域** というセクションを作成できます。

### レコードタイプ

レコードタイプは、Workfront Planning Workspaceの構築ブロックです。 レコードタイプの相互接続の方法を定義できます。

#### ワークスペースでレコードタイプを定義するにはどうすればよいですか？

* ✅ 追跡が必要な情報（必要なレコードタイプ）と、その情報を関連付ける必要がある方法を特定するには、少し時間がかかります。 ワークスペースを使用する関係者と話し合い、すべてのニーズを検討します。 また、様々なレコードタイプでカスタムセクションを作成して、非常に使いやすい方法で情報を表示することもできます。

* ⛔ 異なる期間のレコードタイプを複製しないでください（例えば、**Campaigns 2024** と **Campaigns 2025** 用に別々のレコードタイプを作成しないでください）。

  異なるレコードタイプを作成すると、複数年のデータを比較する場合に、データのフローが中断されます。 今日のビューはレコードタイプごとなので、年が終わるとすぐに、そのレコードタイプのビューには将来の項目が表示されなくなります。 ベストプラクティスは、作業のタイプに対して 1 つのレコードタイプを用意し、必要に応じて、異なるフィールドに基づくフィルターを使用するか、アーカイブしてデータをセグメント化することです。

#### リンクされたレコードタイプに対して、単一選択フィールドまたは複数選択フィールドはどのような場合に使用すればよいですか？

* ✅ オブジェクトを他の複数のレコードタイプに接続して使用する場合は、新しいレコードタイプを追加します

  例えば、キャンペーンは複数のターゲットオーディエンスに接続でき、戦術は単一のターゲットオーディエンスに接続できます。 そのため、Campaign、Tactic、Audience は、複数選択のフィールドではなく、レコードタイプにする必要があります。

* ✅ オブジェクトが検索に役立つ追加のメタデータ値を保存する必要がある場合は、新しいレコードタイプを追加します

  例えば、**メール** などのチャネルレコードタイプは、サポートする成果物のリストを、ネイティブメタデータとして、またはスタンドアロンの **成果物** レコードタイプへの接続として保存できます。
* ⛔ 保存するデータが 1 つのレコードタイプにのみ関連する場合は、新しいレコードタイプを追加しません。

  例えば、**キャンペーン** レコードタイプには、**キャンペーンサイズ** と呼ばれる単一選択フィールドがあり、特定のキャンペーンに直接関連付けられている場合にのみ関連します。 この情報を取り込むには、代わりにフィールドを作成します。

#### レコードタイプにはどのようなラベルを付けるべきですか？

* ✅**Campaigns** など、単一の構成要素または名詞を表すレコードタイプを作成し、ラベルを付けてください。
* ⛔ ビューとして適切に表示されるレコードタイプを作成しない。

  例えば、**カレンダー** は、レコードタイプ自体ではなく、レコードのビューであるため、レコードタイプには適していません。

### フィールド管理

フィールドはレコードタイプの属性で、テーブル表示では列として表示されます。 レコードタイプのカスタムフィールドを作成し、フィールドをWorkfront Planning レコードに関連付けて、レコード情報を強化できます。

#### プライマリフィールドとして定義することをお勧めします。

* ✅ 一意のプライマリフィールド値を使用して、接続を行う際にこれらのレコードを簡単に見つけて「選択」できるようにしてください。 

  接続を作成する際、ユーザーはプライマリフィールドの値で検索し、値が一意でない場合、ユーザーはどの値を選択すればよいかわからない。 
* ⛔ 一意でない値をプライマリフィールドとして使用すると、接続ピッカーメニューの使用時に、プライマリフィールドで検索する必要があるユーザーに混乱を招く可能性があるので、避けてください。 

#### 数式の使い方

* ✅ 数式フィールドの種類を使用して、手動入力を減らしてください。 既にテーブル ビューに存在するデータに基づいて情報を入力する場合は、数式を使用してその情報を自動的に計算することにより、手間を省くことができます。

#### ワークスペースでデータの接続を開始するにはどうすればよいですか？

* ✅ 接続の作成は、Workfront Planning の最も強力な機能の 1 つです。 レコードタイプを相互に関連付けたり、Adobe Workfront（プロジェクト、ポートフォリオ、プログラム、会社およびグループへの接続）、Adobe Experience Manager Assets（アセットおよびフォルダーへの接続）、Adobe GenStudio for Performance Marketingなどの他のアプリケーションのオブジェクトタイプを使用してレコードタイプを関連付けることができます。

  オブジェクトとレコードの種類を接続すると、社内のすべてのものがどのように接続されているかの完全な概要を把握できます。

  例えば、**キャンペーン** レコードタイプと **戦術** レコードタイプがあり、これら 2 つのレコードタイプの間の接続を作成して、特定の **キャンペーン** に関連付けられている **戦術** を確認できます。

  接続を定義すると、ワークスペース内のすべてのユーザーは、接続フィールドをダブルクリックして **キャンペーン** の値の追加を開始できます。このフィールドには、使用可能なすべての **戦術** のリストが表示されます。 これにより、キャンペーンに関連付ける必要のある戦術をすばやく見つけることができます。

#### 参照フィールドの使用方法

* ✅ レコード間またはオブジェクト タイプ間の関連付けを確立した後、個々のレコードを相互に関連付けて、Workfront Planning レコードにリンクされたレコードまたはオブジェクト タイプのフィールドを表示することができます。 同じ情報を更新する必要がある場所の数を減らし、完全に一致するようにします。

  例えば、**Campaign** レコードタイプと **Tactics** レコードタイプを接続すると、プライマリフィールド情報は表示されますが、ルックアップフィールドを追加すると、**Tactic** の **ローンチ日** など、そのレコードタイプから追加の情報を取り込むことができます。 これらの参照フィールドのデータは、レコードの追加後に自動入力されます。

#### URL に推奨されるフィールドタイプは何ですか？ 

* ✅ 1 行テキストフィールドを使用して、レコードに URL データを追加します。

### ビュー

#### ビューとレコードタイプの違いを判断する方法は？

* ✅ 単一の構成要素または名詞を表すもの（**Campaigns** など）の場合、レコードタイプを作成します。 

* ⛔ ビューとして適切に表示されるレコードタイプを作成しない。

  例えば、**カレンダー** は、レコードタイプ自体ではなく、レコードのビューであるため、レコードタイプには適していません。 

#### 自分に関係のないフィールドを非表示にしたり削除したりする必要はありますか？

* ✅ この情報が同じレコードタイプを使用する別のユーザーに関連する可能性がある場合は、列を削除するのではなく非表示にします。 特定のテーブル ビューでフィールドを削除すると、このレコードの残りのビューと、このレコードの種類がリンクされている他のすべての場所でも、このフィールドが削除されます。

#### テーブルビューとタイムラインビューでは、フィルターとグループ化をどのように使用すればよいですか？

* ✅ フィルターおよびグループ化を使用したビューを使用して、表示する必要のある内容のスナップショットを表示します。 データをフィルタリングしてグループ化すると、より使いやすい方法で計画内容を把握できます。 メタデータフィールドでレコードをグループ化できます。

  例えば、**キャンペーン** レコードタイプのタイムライン表示を作成し、**ターゲットオーディエンス** でグループ化して、**日付** でフィルタリングすることで、現在の年のみを表示できます。

#### タイムライン ビューにすべてのレコードが表示されないのはなぜですか。

* ✅ レコードには 2 つの日付フィールドを必ず定義してください。 タイムライン表示を作成できるのは、1 つのレコードタイプに関連付けられた日付フィールドが少なくとも 2 つ存在する場合のみです。 開始日と終了日のどちらか一方または両方に値がない場合、または開始日が終了日より後の場合、一部のレコードがタイムライン ビューに表示されないことがあります。

#### タイムライン表示設定の使用方法

* ✅**バースタイル** や **カラー** など、タイムラインビューの設定を定義して、より視覚的に充実したビューを取得します。 **バースタイル** をカスタマイズするには、意味のある画像でサムネールを表示するかどうかを定義し、バーに表示するフィールドをさらに追加します（例：**所有者** または **ステータス**）。

  デフォルトでは、プライマリフィールドのみが表示されます。 また、フィールド値や適用したグループ化に基づいて、バーの色を定義することもできます。たとえば、[ ステータス ] フィールドと一致させてバーの色をカスタマイズできます。 デフォルトでは、カラーはレコードタイプのカラーに一致します。

  タイムラインのレコードバーの色に影響を与えることができるのは、レコードタイプの色または色に関連付けられたオプションを持つフィールドのみです。

### 権限と共有

共有機能を使用して、他のユーザーにビューやワークスペースに対する適切な権限を付与します。

#### ワークスペースに対する権限を管理するにはどうすればよいですか？

* ✅ **ワークスペース** を作成した場合は、自分だけが使用できます。 システム管理者でない他のユーザーは見つけることができません。 ワークスペースを定義し、チームでコラボレーションを開始する準備が整ったら、チームと共有して権限レベルを定義する必要があります。

  次の権限レベルから選択できます。

   * **管理**：ユーザーは、ワークスペース、レコードタイプ、レコードの編集、削除、作成を編集、削除、共有できます。
   * **投稿**：ユーザーは、レコードを作成、編集および削除できます。
   * **表示**：ユーザーはレコードを表示できます。

* ✅ 多くのお客様は、ほとんどのユーザーにワークスペースに **管理** 権限を付与したいと考えていますが、レコードタイプを誤って削除したり、不要なレコードタイプやフィールドを作成したりしない、信頼できるユーザーの選択されたグループに **管理** 権限を制限しないでください。 ワークスペースの編集、共有、削除も可能です。 このレベルの権限は、Workspaceへの完全な管理アクセス権を付与します。

  ワークスペースに対する管理権限を持つユーザーには、標準ユーザーライセンスが必要です。

* レコードの作成、編集、削除は可能でも、ワークスペースの構造を変更したくない場合は、ユーザーに ✅ 投稿 **権限を付与してくださ**。 **投稿** 権限を持つユーザーは、レコードタイプを作成したり、既存のレコードタイプのフィールドを変更したりすることはできません。

  ワークスペースに対する **投稿** 権限を持つユーザーには、標準ユーザーライセンスが必要です。

* レコードを表示するだけの場合は、ユーザーに ✅ 表示 **権限を付与してくださ**。

#### レコードタイプに対する権限を管理するにはどうすればよいですか？

* ✅ ワークスペースに対する管理権限を持つユーザーは、レコードタイプに対する権限を下げることはできません。 また、レコードタイプに対する管理権限も継承します。 ワークスペースに対する管理権限をユーザーに付与することはできませんが、レコードタイプに対する投稿または表示権限を付与します。
* ✅ ユーザーにワークスペースよりも低いレコードタイプの権限レベル（表示権限など）を付与する場合は、ワークスペースへの投稿権限を付与することをお勧めします。 その後、レコードタイプに対する表示権限を付与できます。
* レコードタイプの権限からユーザーを削除しても、少なくともワークスペースに対する表示権限は付与されます。

#### ビューへの権限を管理するにはどうすればよいですか？

* ✅ ビューを編集、削除、共有できるようにするユーザーに対して、**管理** 権限を予約しないでください。 つまり、フィルター、グループ化フィールド、またはビューの設定を変更できます。 これらの変更は、同じビューを使用しているすべてのユーザーに対して、ビューのメイン設定に影響します。

  ビューに対する管理権限を持つユーザーには、標準ユーザーライセンスが必要です。

* ✅ ユーザーに **ビュー** 権限を付与して、ビューを適用できるようにします。 これらのユーザーは、一部のフィルターやグループ化および並べ替えを変更できますが、それらの変更は一時的なものであり、ビューにアクセスする他のすべてのユーザーにとって、変更内容は保存されません。 これらの変更は、同じビューを使用している他のすべてのユーザーのビューのメイン設定には影響しません。  変更内容は、変更された設定を適用するユーザーにのみ表示されます。 画面を更新すると、変更はデフォルトにリセットされます。

* ワークスペースを表示できるすべてのユーザーに、特定のビューでレコードとそのフィールドを表示する場合は、✅ ワークスペース内のすべてのユーザーが表示できる **権限を** 与します。 これにより、ビューの共有権限ボックスに手動で誰かを追加する必要がなくなります。

  >[!NOTE]
  >
  >ビューが共有されておらず、他のユーザーとリンクを共有した場合、そのユーザーは **デフォルトのテーブルビュー** でレコードを表示できます。 標準Workfront ライセンスがある場合は、独自のビューを作成できます。

#### **Workspaceの共有** と **ビューの共有** の違いは？

* **Workspace共有** ワークスペース、ワークスペースのレコードの種類、レコード、およびワークスペースのフィールドに対するユーザーのアクセスを定義します。

* **ビューの共有** では、作成したビューをユーザーが表示できるかどうか、およびユーザーがフィルター、グループ化フィールド、またはその他のビューの設定を変更できるかどうかを定義します。 ビュー内に表示されるレコードの表示は、ビュー共有ではなく、Workspace共有によって制御されます。

#### Workfront ライセンスタイプがWorkfrontの Planning 権限に与える影響

* **Workspace共有** の場合：Light および Contribute ライセンスのユーザーは、Workspace への表示アクセス権しか取得できません。 ワークスペースに対する投稿または管理権限を付与するには、標準ライセンスが必要です。

* **ビュー共有**：ワークスペースに対する管理権限を持つ標準ライセンスユーザーは、ビューを作成できます。 Light および Contribute ライセンスユーザーは、Standard ユーザーが作成して共有したビューのみを使用できます。 何も共有されていない場合は、**デフォルトのテーブル表示** が表示されます。

#### Workspaceのオーナーが変更された場合はどうすればよいですか？

* Workfrontは Workspace の作成者をオーナーとして設定しますが、機能に関しては、オーナーは管理権限を持つ他のユーザーと同じ権限を持ちます。
* 所有者がアクティベート解除されると、他のメンバーは、作業を中断することなくワークスペースで作業を続行できます。
* システム管理者はどのワークスペースにもアクセスできるので、管理権限を持つ唯一のユーザーが所有者だった場合、管理者は別のユーザーを追加して、ワークスペースの管理を処理する管理権限を付与できます。

### Workfront Planning での要求の発行

レコードタイプのページ外にレコードを追加する場合は、レコードタイプごとにリクエストフォームを作成できます。 フォームを送信すると、レコードタイプに新しいレコードが追加されます。

#### レコードタイプのリクエストフォームの作成はいつ開始すべきですか？

* ✅ まず必要なフィールドをテーブルに追加して、レコードタイプ構造を設定する必要があります。 これらのフィールドはレコードを記述し、フォームビルダーでアクセスできます。

  レコードタイプ構造が完成した後にリクエストフォームまたは取り込みフォームを作成して、キーフィールドが欠落しないようにするのが理想的です。

#### リクエストフォームを作成できるユーザー

* ✅ ワークスペースへの管理アクセス権を持つユーザーは誰でも、レコードタイプのリクエストフォームを作成または編集できます。 この機能を許可するためにユーザーの権限が適切に割り当てられていることを確認します。

#### レコードタイプのリクエストフォームを作成または編集するにはどうすればよいですか？

* ✅ ワークスペースへの管理アクセス権を持つユーザーは誰でも、[Adobe Workfront Planning でのリクエストフォームの作成と管理 ](/help/quicksilver/planning/requests/create-request-form.md) の記事に記載されている手順に従うことができます。


#### 要求フォームを使用して新しいレコードを送信できるユーザー

* 送信権限 ✅、各フォームに対して設定する設定によって異なります。

  フォームビルダーでは、フォームを公開した後、権限を管理してリクエストを送信できるユーザーを制御できます。

  次の共有オプションから選択できます。

   * Workfront内ユーザーとの内部共有の場合：

      * **ワークスペースへの表示以上のアクセス権を持つすべてのユーザー：** ワークスペースに対する表示以上の権限を持つすべてのユーザーが、レコードを作成するリクエストを送信できます。
      * **ワークスペースへの投稿以上のアクセス権を持つすべてのユーザー**：ワークスペースに対する投稿以上の権限を持つユーザーへの送信を制限します。
      * **招待されたユーザーのみがアクセスできます**：フォームにリクエストを送信できるユーザー、チーム、役割、グループまたは会社を追加します。
   * Workfront アカウントを持たないユーザーとの外部共有の場合：
      * **公開リンクを作成** してから、コピーして任意のユーザー（Workfront アカウントを持っていないユーザーも含む）と共有します。フォームリンクを持つすべてのユーザーがリクエストを送信できます。
      * **リンクの有効期限：** セキュリティを強化するために、公開リンクの有効期限を必ず設定してください。

### リクエストフォームを管理するためのベストプラクティス

リクエストフォームを管理する場合は、次の推奨事項に従ってください。

* 事前に計画：後で過剰な修正が行われるのを避けるために、フォームを作成する前に、要求者に必要な情報や必要な情報を明確に定義します。
* 明確なラベルの使用：すべてのユーザーに対して、フィールドラベルと説明が明確で理解可能であることを確認します。
* フォームのテスト：新しいフォームをより広いオーディエンスに向けて展開する前に、フォームリンクとフォームのプレビュー機能を使用してテストし、すべてのフィールドとロジックが期待どおりに機能することを確認します。
* フォームを最新の状態に保つ：定期的にフォームを確認し、レコードタイプ構造や運用プロセスの変更に合わせて更新します。

<!--do we need to add anything for the Configuration tab of a request form?? -->

<!-- this is hidden, per Andrea:  

2.2 Migration  

Migrating your data from external <span style="text-decoration:underline;">s~~S~~</span>ystems to Workfront Planning unlocks new ways to create important connections in your workflow and uncover insights that you might not have been able to identify with your previous tools. 

By having all your data in one central location, you can more easily form connections between your Workfront data than if they all existed in separate tools. 

We have some options that will help you to accelerate the migration process:  

* **Fusion** – You can create a Scenario in Fusion that runs after certain criteria and connects objects. 
* **Bulk Data Operations** _through the new functionality -[ [E] Make connected Planning data consumable through WF forms](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6641b040000b880ccd74aab6365c3361/overview?source-id=unifiedShareMFE)  (Q3 2024)_ -  
* **Copy and paste – **You can copy and paste directly from a spreadsheet. This is best suited to a simple table of data from tools like Excel or Google Sheets.  
* **Upload a C<span style="text-decoration:underline;">SV~~VS~~</span> or Excel **- The CSV (comma-separated values) format or Excel is one of the most common ways to move data between applications, and tools. This functionality is not available yet, but we are planning to work on it in Q4 2024.  

-->

<!--
     

1. Data Flow  

Currently the metadata modelling in Workfront Planning is done by Ops Admins through adding various data points to the record type from the table view, including: 



* Fields added directly on the current record type 
* Connections with custom defined operational and taxonomical record types 
* Connections with execution work captured in Workfront 
* Connections with deliverables stored as assets in AEM 
* Any lookup fields captured in any of the above connections. 

Here is a summary of how you can define the data flow within Workfront Planning and other applications.  


     



* **Connections and Lookup fields. **Creating **connections** is one of the most powerful features of Workfront Planning. You can connect record types to one another or record types with object types from other applications like Adobe Workfront (connection to Project, Portfolios, Programs, Companies, and Groups) or Adobe Experience Manager Assets (connection to assets and folders).  Connections give you a full overview of how everything in your company is connected.  

    - e.g.: You have a Campaign record type, and a Tactics record type, then you can create a connection between these two record types to see to see which Tactics are associated to a specific Campaign. After defining the connection, all the people in the workspace can start adding values by double-clicking into the connection field that displays the tactic where they will see a list of all the Tactics available and you can quickly select the tactics to be associated with each campaign. 


    After you establish the connection between records or object types, you can connect individual records to one another, and display fields from the linked record or object types on a Workfront Planning record. The connected fields are called **Lookup fields**. You will reduce the number of places you have to update the same piece of information and ensure that they match perfectly.  


    - e.g.: Once you have a connection between a Campaign record type and a Tactics record type, you will see the primary field information when you add the tactic, but when you add lookup fields, you will be able to bring additional information from the tactic, like the Launch date for that Tactic. The data for these lookup fields is auto populated. Find more information in the Adobe Experience League documentation in the article about Connecting records.  


     

* **Planning (or Connections) tab** **in Workfront _-[ [E] Global Connect capability in Planning connections area](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6617d7760001e250f5ffb9ebf04baacc/overview?source-id=unifiedShareMFE)_** 

    When you go to the Planning section of Adobe Workfront objects, you can display both connections with linked records or any available connections with Planning record types. With that, you can view and edit any connection field without having to navigate away from the current section in Workfront to other areas. The Planning section is available for the following Workfront objects: Project, Portfolio and Program. For more information, see [Manage records in the Planning section of Adobe Workfront objects](https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-records/manage-records-in-planning-section).   


* Create new records within the connection fields - In-context creation of connected records https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6656c1a30026b903c6edf0210b8cbb23/overview?source-id=unifiedShareMFE  When you need to link records through a connection field but cannot find the required records in the connected record type, you can also create new records in the connected record type directly within the connection fields, with that you can efficiently establish necessary links without having to leave the current record type context. For more information, see Create records https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-records/create-records.   

     

* **Field on Customer Form** (CF)[ - [E] Make connected Planning data consumable through WF forms](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6641b040000b880ccd74aab6365c3361/overview?source-id=unifiedShareMFE) _(Planned completion date Sep 15, 2024 10:00 PM)._ Considering that the Workfront Project metadata modeling is done through forms, you are also able to add Planning connections to your custom forms. You can embed any lookup field value from the connected Planning record types within the custom form of your Workfront object. With that capability, when you are managing objects in Workfront, you can present any taxonomies or operational records connected to the Workfront object in custom forms, alongside other details, so that your teams can easily consume and update all the relevant information through a unified interface.  They should not need to navigate to different areas to view and update the information relevant for their work.  

     

* **Connection between Workspaces with Record types accessible from multiple workspaces** – ~~Epic – "[Connect to record types across workspaces](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/64dfad3100027190324dcc35b2176e76/overview?source-id=unifiedShareMFE)"~~ When you are creating a workspace in Planning, you can define certain record types once and then configure them to be accessible from multiple workspaces so you can create connections with them from anywhere. This way, you can streamline the data management process, eliminate duplicative work, and ensure data consistency across teams. As a result, your teams can tag their records with common taxonomies and unlock better visualization, filtering, grouping, and reporting of cross-team work.  For more information, see [Edit record types](https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-architecture/edit-record-types). 

     

* **Fusion connector – You can create a connection to your Workfront Planning account from inside a Workfront Fusion module. **With this connector, you can trigger a scenario when events occur in Workfront Planning. You can also create, read, update, and delete records, or perform a custom API call to your Adobe Workfront Planning account. More information in Experience League in[ Adobe Workfront Planning modules](https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-fusion/fusion-apps-and-modules/workfront-planning-moduleshttps:/experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-fusion/fusion-apps-and-modules/workfront-planning-modules) article.  

-->
