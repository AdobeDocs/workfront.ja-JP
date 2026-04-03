---
title: 導入に関するAdobe Workfront計画の推奨事項
description: マーケティング業務のリーダーとして、Adobe Workfront Planning を使用すると、すべてのチームのマーケティングライフサイクル全体の作業を整理できます。Workfront Planningを始める際にお勧めのベストプラクティスを以下に示します。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 6e039b80-e3bf-412c-8c86-8f801f5861e3
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '3405'
ht-degree: 2%

---

<!--drafted because Kari Woolf will write something for Field Readiness instead, nothing for ExL, public-facing documentation-->

# Adobe Workfront計画の導入に関する推奨事項

<!-- this used to be called Adobe WFP best practices, but the best practice piece was replaced by this folder of articles: [Adobe Workfront Planning best practices: article index](/help/quicksilver/planning/best-practices.md/best-practices-article-index.md) -->

>[!IMPORTANT]
>
>この記事の情報は、Adobe Workfront の追加機能である Adobe Workfront Planning に関するものです。
>
>Workfront Planning へのアクセス要件のリストについて詳しくは、[Adobe Workfront Planning へのアクセスの概要](/help/quicksilver/planning/access/access-overview.md)を参照してください。
> 
>Workfront計画の一般的な詳細については、[Adobe Workfront計画の基本を学ぶ](/help/quicksilver/planning/general/planning-overview.md)を参照してください。
>
>詳しくは、[Adobe Workfront計画のベストプラクティス：記事インデックス &#x200B;](/help/quicksilver/planning/best-practices.md/best-practices-article-index.md)の記事を参照することをお勧めします。

マーケティング業務のリーダーとして、Adobe Workfront Planning を使用すると、すべてのチームのマーケティングライフサイクル全体の作業を整理できます。

この記事では、Workfront Planningを開始する際に推奨される、よくある質問とベストプラクティスについて説明します。


## 設定のベストプラクティス

### ワークスペース

ワークスペースは、チームが作業を計画するための一元化された場所です。 ワークスペースは、チームが使用するレコードタイプのコレクションで、チームの作業ライフサイクルを表します。

次に、Workfront Planningの設定に関するよくある質問をいくつか示します。

#### どうすればよいですか？

* ✅初めてPlanningにログインするときは、Planningの価値を明確に伝え、製品を効果的に操作して利用する方法をガイドするアプリ内オンボーディングプロセスに従ってください。 これにより、その機能と作業を簡単に開始する方法を確実に理解できます。
* ✅まず、既存の類似したユースケースのアイデアを得るために、定義済みのワークスペース テンプレートを調べます。 テンプレートに含まれる定義済みのレコードタイプ、フィールドを使用するか、自分で追加することができます。
* ✅ Workfront Planningで解決する主なユースケースを特定します。 例えば、多くの企業は、より優れた「キャンペーンカレンダー」の構築を含め、戦略的アクティビティの可視性を改善したいと考えています。 その場合、まずいくつか質問に答えることから始めましょう。

   * 誰がそれを求めているのか。
   * カレンダーに入れたいものを何と呼ぶのでしょうか？
キャンペーン？ 戦術？ 取り組み？ アクティビティ？ イベント？
   * どのような質問に答えたいのでしょうか？
   * 同じオーディエンスを対象とした、重複するキャンペーンはありますか？
   * キャンペーン、戦術、アクティビティ、イベントの予算はどれくらいか？

  これらの質問に対する答えが、Workfront Planningの内部で何を構築する必要があるかを決めます。

  また、現在Workfront ユーザーではない他のプランナーが存在する場合もあります。 これらのプランナーは、Excel スプレッドシート、Word ドキュメント、PowerPoint プレゼンテーションなどで動作します。 Workfront Planningの個人情報へのアクセス方法を検討する。

* ✅ Workfront Planningを最大限に活用するには、Workfrontのポートフォリオとプログラムの使用を、Workfront Planningの他の上層構造に置き換えることを検討してください。

  今日、Workfrontのお客様は、ポートフォリオやプログラムを通じて、戦略的作業を表現しています。場合によっては、異なるタイプのプロジェクトを表現する場合もあります。 プランニングの導入により、このような戦略的作業はすべて、Workfrontプランニングのカスタムレコード型を通じて処理する必要があります。一方、Workfrontは、プロジェクトやタスクとして表される作業の実行フェーズを中心として扱います。

#### 新しいワークスペースを作成する場合と既存のワークスペースを変更する場合は、いつ作成すればよいですか？

* 最小数の組織レベルのワークスペース用に✅設計します。 特定の業務組織ユニット用のワークスペースを作成して、各ユニットのユニークな作業方法に合わせることができます。

  データ間の関係を容易に管理できるように、単一のWorkspaceにデータを保管する必要があります。

  例えば、あらゆるマーケティング施策に単一のワークスペースを使用できるようにします。

  業務構造が全く異なるチーム向けに、新しいワークスペースを作成することも可能です。

  例えば、**製品開発** ワークスペースは、**マーケティング** ワークスペースとは異なる必要があります。

* ⛔組織内のチームまたはプロセスごとに一意のワークスペースを作成しないでください。

  マーケティング部門は、単一のワークスペースを維持して、可視性を維持し、データをグローバル計画レベルでロールアップできるようにすべきです。

  同様のプロセスに従うチーム（EMEA マーケティングとAPAC マーケティングなど）向けに、類似したワークスペースや重複するワークスペースを作成することを避けます。特に、これらのチームが共通の戦略的キャンペーンに合わせて作業を行う場合は避けます。

#### Workspaceのセクションの使用方法を教えてください。

* ✅ セクションを作成してラベル付けし、ユーザーが運用ライフサイクルをどのように整理しているかを理解できるようにします。

  例えば、**コアレコード**&#x200B;というセクションを作成して、キャンペーン、戦術、成果物をワークスペースに配置します。
* ✅ 「いいね」レコードタイプを一緒にグループ化します。

  例えば、地域、国、都市などのレコードタイプを含む&#x200B;**地域**&#x200B;というセクションを作成できます。

### レコードタイプ

レコードタイプは、Workfront Planning Workspaceの構成要素です。 レコードタイプの相互接続方法を定義できます。

#### ワークスペースでレコードタイプを定義するにはどうすればよいですか？

* ✅追跡する必要がある情報（必要なレコードタイプ）と、この情報を接続する方法を特定するのに時間がかかります。 ワークスペースを使用してあらゆるニーズを検討する関係者と話し合いましょう。 また、様々なレコードタイプを持つカスタムセクションを作成して、情報を非常に消耗性の高い方法で表示することもできます。

* ⛔別の期間のレコードタイプを複製しないでください（例：**キャンペーン 2024**&#x200B;と&#x200B;**キャンペーン 2025**&#x200B;のレコードタイプを別々に作成しないでください）。

  異なるレコードタイプを作成すると、複数年にわたるデータを比較するたびに、データの流れが分断されます。 現在のビューはレコードタイプごとに表示されるため、年が終了するとすぐに、そのレコードタイプのビューに今後の項目が表示されなくなります。 作業タイプごとにひとつのレコードタイプを用意し、必要に応じてフィールドごとにフィルターを使用してデータをセグメンテーションしたり、アーカイブ化したりすることがベストプラクティスです。

#### リンクされたレコードタイプに対して、単一または複数選択のフィールドをいつ使用する必要がありますか？

* ✅ オブジェクトが他の複数のレコードタイプと関連付けて使用される場合は、新しいレコードタイプを追加します

  例えば、キャンペーンには複数のターゲットオーディエンスへの接続があり、戦術には単一のターゲットオーディエンスへの接続がある場合があります。 そのため、キャンペーン、戦術、オーディエンスは、複数選択フィールドではなく、レコードタイプである必要があります。

* ✅ オブジェクトが参照に役立つ可能性のある追加のメタデータ値を格納する必要がある場合は、新しいレコードタイプを追加します

  例えば、**Email**&#x200B;などのチャネルレコードタイプは、ネイティブメタデータとして、またはスタンドアロンの&#x200B;**成果物** レコードタイプへの接続として、サポートする成果物のリストを保存できます。
* ⛔保存するデータが1つのレコードタイプにのみ関連する場合、新しいレコードタイプを追加しないでください。

  例えば、**キャンペーン** レコードタイプには、**キャンペーンサイズ**&#x200B;という単一選択フィールドがあり、特定のキャンペーンに直接関連付けられている場合にのみ関連する場合があります。 代わりにフィールドを作成して、この情報をキャプチャします。

#### レコードタイプのラベル付け方法

* ✅単一の構成または名詞（**キャンペーン**&#x200B;など）を表すレコードタイプを作成してラベル付けします。
* ⛔ ビューとしてより適切に表現されたレコードタイプを作成しないでください。

  例えば、**カレンダー**&#x200B;はレコードタイプ自体ではなく、レコードのビューであるため、レコードタイプの選択肢としては不適切です。

### フィールド管理

フィールドはレコードタイプの属性で、テーブルビューに列として表示されます。 レコードタイプのカスタムフィールドを作成し、そのフィールドをWorkfront計画レコードに関連付けて、レコード情報を強化できます。

#### どのフィールドをプライマリフィールドとして定義することをお勧めしますか？

* ✅一意のプライマリ フィールド値を使用して、接続を行う際に、これらのレコードを簡単に検索して「選択」できるようにします。 

  接続を行う際に、プライマリフィールドの値で検索します。一意でない場合、どの値を選択すればよいかわかりません。 
* ⛔接続ピッカーメニューを使用する際にプライマリフィールドで検索する必要があるユーザーの混乱を引き起こす可能性があるため、一意でない値をプライマリフィールドとして使用しないでください。 

#### 数式の使用方法

* ✅数式フィールド型を使用して手動入力を減らします。 既にテーブルビューにあるデータに基づいて情報を入力する場合、数式を使用して情報を自動的に計算することで、労力を節約できる場合があります。

#### ワークスペース内のデータの接続を開始するにはどうすればよいですか？

* ✅接続の作成は、Workfront Planningの最も強力な機能の1つです。 レコードタイプを相互に接続したり、Adobe Workfront（プロジェクト、ポートフォリオ、プログラム、会社、グループへの接続）、Adobe Experience Manager Assets（アセットとフォルダーへの接続）、Adobe GenStudio for Performance Marketingなどの他のアプリケーションのオブジェクトタイプを使用してレコードタイプを接続したりできます。

  オブジェクトタイプとレコードタイプを接続することで、自社のあらゆるシステムがどのように連携しているのかを包括的に把握できます。

  例えば、**Campaign** レコードタイプと&#x200B;**Tactics** レコードタイプがあり、これら2つのレコードタイプ間に接続を作成して、どの&#x200B;**Tactics**&#x200B;が特定の&#x200B;**Campaign**&#x200B;に関連付けられているかを確認できます。

  接続を定義した後、ワークスペース内のすべてのユーザーは、利用可能なすべての&#x200B;**戦術**&#x200B;のリストが表示される接続フィールドをダブルクリックして、**キャンペーン**&#x200B;の値の追加を開始できます。 これにより、キャンペーンに関連付ける必要のある戦術を素早く見つけることができます。

#### 参照フィールドの使用方法を教えてください。

* ✅ レコードまたはオブジェクト タイプ間の接続を確立した後、個々のレコードを相互に接続し、リンクされたレコードまたはオブジェクト タイプのフィールドをWorkfront Planning レコードに表示できます。 これにより、同じ情報を更新する必要がある場所の数を減らし、完全に一致するようにします。

  例えば、**Campaign** レコードタイプと&#x200B;**Tactics** レコードタイプの間に接続すると、プライマリフィールド情報が表示されますが、ルックアップフィールドを追加すると、**戦術**&#x200B;の&#x200B;**開始日**&#x200B;など、そのレコードタイプから追加情報を取り込むことができます。 これらのルックアップフィールドのデータは、レコードが追加された後に自動的に入力されます。

#### URLにはどのようなフィールドタイプが推奨されますか？ 

* ✅ 1行のテキストフィールドを使用して、URL データをレコードに追加します。

### ビュー

#### ビューとレコードタイプの違いを判断するにはどうすればよいですか？

* ✅単一の構成または名詞（**キャンペーン**&#x200B;など）を表すオブジェクトの場合は、レコードタイプを作成します。 

* ⛔ ビューとしてより適切に表現されたレコードタイプを作成しないでください。

  例えば、**カレンダー**&#x200B;はレコードタイプ自体ではなく、レコードのビューであるため、レコードタイプの選択肢としては不適切です。 

#### 自分に関係のないフィールドを非表示にするか、削除するかを指定します。

* ✅同じレコードタイプを使用している別のユーザーにこの情報が関連する可能性がある場合は、列を削除せずに非表示にします。 特定のテーブルビューでフィールドを削除すると、このフィールドは、このレコードタイプがリンクされている他の場所だけでなく、このレコードの残りのビューでも削除されます。

#### テーブルおよびタイムラインビューでフィルターとグループ化を使用する方法を教えてください。

* ✅ フィルターとグループ化を使用して、表示する必要のある項目のスナップショットを表示します。 データをフィルタリングしてグループ化することで、何が計画されているのかを把握するための、より消耗品の方法を持つことができます。 レコードは、メタデータフィールドでグループ化できます。

  例えば、**キャンペーン** レコードタイプのタイムラインビューを作成できます。このレコードタイプは、**ターゲットオーディエンス**&#x200B;でグループ化し、**日付**&#x200B;でフィルタリングして、現在の年のみを表示できます。

#### タイムラインビューにすべてのレコードが表示されないのはなぜですか？

* ✅ レコードに2つの日付フィールドを定義することを忘れないでください。 タイムラインビューを作成できるのは、レコードタイプに関連付けられた日付フィールドが2つ以上ある場合のみです。 開始日または終了日、またはその両方に値がない場合、または開始日が終了日より後の場合、タイムラインビューに一部のレコードが表示されない場合があります。

#### タイムラインビュー設定の使用方法を教えてください。

* ✅ **棒スタイル**&#x200B;や&#x200B;**色**&#x200B;など、タイムラインビューの設定を定義して、より視覚的に見やすくします。 バーのスタイル **をカスタマイズするには、意味のある画像を含むサムネールを表示するか、バーに表示するフィールドをさらに追加するかを定義します（例：**&#x200B;所有者&#x200B;**または** ステータス **）。**

  デフォルトでは、プライマリフィールドのみが表示されます。 バーの色をフィールド値で定義することもできます（例えば、バーの色をステータス フィールドに一致させることでカスタマイズできます）。または、適用したグループ化で定義することもできます。 デフォルトでは、色はレコードタイプの色と一致します。

  レコードタイプの色または色に関連するオプションを含むフィールドのみが、タイムラインのレコードバーの色に影響を与えることができます。

### 権限と共有

共有機能を使用して、他のユーザーにビューとワークスペースに対する適切な権限を付与します。

#### ワークスペースに対する権限を管理するにはどうすればよいですか？

* ✅ **ワークスペース**&#x200B;を作成する場合、そのワークスペースは自分のみが使用できます。 システム管理者でないユーザーは、システム管理者を見つけることができません。 ワークスペースを定義し、チームにコラボレーションを開始する準備ができたら、それをチームと共有し、権限レベルを定義する必要があります。

  次の権限レベルから選択できます。

   * **管理**：ユーザーは、ワークスペースの編集、削除、共有、レコードタイプ、レコードの編集、削除、作成を行うことができます。
   * **Contribute**：ユーザーはレコードを作成、編集、削除できます。
   * **表示**：ユーザーはレコードを表示できます。

* ✅多くの顧客は、ワークスペースに&#x200B;**Manage**&#x200B;権限を付与すると考えていますが、**Manage**&#x200B;権限は、レコードタイプを誤って削除したり、不要なレコードタイプやフィールドを作成したりしない、信頼できるユーザーの選択グループに制限しないでください。 ワークスペースの編集、共有、削除も可能です。 この権限レベルでは、Workspaceへの完全な管理アクセス権が付与されます。

  ワークスペースに対する管理権限を持つユーザーには、標準ユーザーライセンスが必要です。

* ✅ ユーザーに&#x200B;**Contribute**&#x200B;権限を付与します。ユーザーがレコードを作成、編集および削除できるようにしたい場合は、ワークスペースの構造を変更する必要はありません。 **Contribute**&#x200B;権限では、レコードタイプを作成したり、既存のレコードタイプのフィールドを変更したりすることはできません。

  ワークスペースに&#x200B;**Contribute**&#x200B;権限を持つユーザーには、標準ユーザーライセンスが必要です。

* ✅ ユーザーに&#x200B;**表示**&#x200B;権限を付与します。ユーザーがレコードを表示する場合に使用します。

#### レコードタイプに対する権限を管理するにはどうすればよいですか？

* ✅ ワークスペースに対する管理権限を持つユーザーは、レコードタイプに対する権限を下げることができません。 また、レコードタイプに対する管理権限も継承します。 ユーザーにワークスペースの管理権限を与えることはできませんが、レコードタイプに対してContributeまたはView権限を与えることができます。
* ✅ ユーザーがワークスペースよりもレコードタイプの権限レベル （表示権限など）を低くしたい場合は、ユーザーにワークスペースへのコントリビュート権限を付与することをお勧めします。 その後、レコードタイプに表示権限を付与できます。
* レコードタイプの権限からユーザーを削除しても、少なくともワークスペースに対する表示権限が付与されます。

#### ビューに対する権限を管理するにはどうすればよいですか？

* ✅ ビューを編集、削除、共有するユーザーの&#x200B;**Manage**&#x200B;権限を予約してください。 つまり、フィルター、フィールドのグループ化、またはビューの一部の設定を変更できます。 これらの変更は、ビューを使用している他のすべてのユーザーのビューの主な設定に影響します。

  表示に対する管理権限を持つユーザーには、標準ユーザーライセンスが必要です。

* ✅ ユーザーに&#x200B;**ビュー**&#x200B;権限を付与して、ビューを適用できるようにします。 フィルターやグループ化や並べ替えを変更できますが、これらの変更は一時的なものに過ぎません。ビューにアクセスする他のすべてのユーザーに対して変更は保存されません。 これらの変更は、ビューを使用している他のすべてのユーザーのビューの主な設定には影響しません。  変更内容は、変更された設定を適用しているユーザーにのみ表示されます。 画面を更新すると、変更内容がデフォルトにリセットされます。

* ✅ ワークスペースを表示できるすべてのユーザーに、その特定のビューでレコードとそのフィールドを表示させるには、**ワークスペース内のすべてのユーザーが**&#x200B;権限を表示できるようにします。 これにより、ビューの共有権限ボックスに手動で誰かを追加する必要がなくなります。

  >[!NOTE]
  >
  >ビューが共有されておらず、そのビューへのリンクを他のユーザーと共有した場合、そのユーザーは&#x200B;**既定のテーブル ビュー**&#x200B;でレコードを表示できます。 標準Workfront ライセンスをお持ちの場合は、独自のビューを構築できます。

#### **Workspace sharing**&#x200B;と&#x200B;**View sharing**&#x200B;の違いとは？

* **Workspace共有**&#x200B;は、ワークスペース、そのレコードタイプ、レコード、およびそのフィールドへのユーザーのアクセスを定義します。

* **ビュー共有**&#x200B;は、ユーザーが作成したビューを表示できるかどうか、およびユーザーがフィルター、グループ化フィールド、またはビューの他の設定を変更できるかどうかを定義します。 ビュー内に表示されるレコードの表示は、ビュー共有ではなく、Workspace共有によって制御されます。

#### Workfrontのライセンスタイプは、Workfront Planningの権限にどのような影響を与えますか？

* **Workspace共有**&#x200B;の場合：LightおよびContribute ライセンスのユーザーは、ワークスペースへの表示アクセスのみを取得できます。 誰かにワークスペースへのContributeまたはManage権限を付与するには、標準ライセンスが必要です。

* **ビュー共有**：ワークスペースに対する管理権限を持つ標準ライセンスユーザーは、ビューを作成できます。 LightおよびContribute ライセンスのユーザーは、Standard ユーザーが作成して共有したビューのみを使用できます。 共有されていない場合、ユーザーは&#x200B;**既定のテーブル ビュー**&#x200B;を表示できます。

#### Workspace オーナーが変更されたときはどうすればよいですか？

* WorkfrontはWorkspace作成者を所有者として設定しますが、機能的に所有者は管理権限を持つ任意のユーザーと同じ権限を持ちます。
* 所有者が非アクティブ化されている場合、他のメンバーは中断することなくワークスペースで作業を続行できます。
* システム管理者は任意のワークスペースにアクセスできるため、所有者が管理権限を持つ唯一のユーザーである場合、管理者は別のユーザーを追加して、ワークスペースの管理を処理する管理権限を付与できます。

### Workfront Planningでのリクエストの送信

ユーザーがレコードタイプのページ外にレコードを追加する場合は、レコードタイプごとにリクエストフォームを作成できます。 フォームを送信すると、レコードタイプに新しいレコードが追加されます。

#### レコードタイプのリクエストフォームの作成は、いつ開始すればよいですか？

* ✅必要なフィールドをテーブルに追加して、最初にレコードタイプ構造を設定する必要があります。 これらのフィールドはレコードを表し、フォームビルダーからアクセスできます。

  理想的には、レコードタイプの構造が完成した後でリクエストフォームまたは受注フォームを作成し、キーフィールドが見落とされないようにします。

#### リクエストフォームは誰が作成できますか？

* ✅ ワークスペースへの管理アクセス権を持つユーザーは、レコードタイプのリクエストフォームを作成または編集できます。 この機能を許可するために、ユーザーの権限が適切に割り当てられていることを確認してください。

#### レコードタイプのリクエストフォームを作成または編集するにはどうすればよいですか？

* ✅ ワークスペースへの管理アクセス権を持つユーザーは、記事[Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)でリクエストフォームを作成および管理する手順に従うことができます。


#### リクエストフォームを使用して新しいレコードを提出できるのは誰ですか？

* ✅送信権限は、各フォームに設定する設定によって異なります。

  フォームビルダーでは、フォームを公開した後、リクエストを送信できるユーザーを制御する権限を管理できます。

  次の共有オプションから選択できます。

   * Workfrontのユーザーとの内部共有の場合：

      * **ワークスペースへの表示以上のアクセス権を持つユーザー：** ワークスペースへの表示以上の権限を持つすべてのユーザーが、レコードを作成するリクエストを送信できます。
      * **ワークスペースへの貢献度が高いユーザーまたは高いユーザー**:Contribute以上の権限を持つユーザーに対して、ワークスペースへの送信を制限します。
      * **招待されたユーザーのみがアクセスできます**: フォームにリクエストを送信できるユーザー、チーム、役割、グループ、または会社を追加します。
   * Workfront アカウントをお持ちでないユーザーとの外部共有の場合：
      * **公開リンクを作成**&#x200B;してから、これをコピーして誰とでも共有できます。Workfront アカウントを持たないユーザーでも、フォームリンクを持っている人なら誰でもリクエストを送信できます。
      * **リンクの有効期限：** セキュリティを強化するために、公開リンクの有効期限を必ず設定してください。

### リクエストフォーム管理のベストプラクティス

リクエストフォームを管理するための推奨事項を以下に示します。

* 事前の計画：フォームを作成する前に、依頼者に必要な情報や必要な情報を明確に定義し、後で過度な修正を避けることができます。
* 明確なラベルを使用する：フィールドラベルと説明が、すべてのユーザーにとって明確で理解しやすいものであることを確認します。
* フォームをテストする：新しいフォームをより多くのオーディエンスに公開する前に、フォームリンクとフォームのプレビューオプションを使用してテストし、すべてのフィールドとロジックが期待どおりに機能することを確認します。
* フォームを最新の状態に保つ：フォームを定期的に確認し、レコードタイプの構造や運用プロセスの変更に合わせて更新します。

<!--do we need to add anything for the Configuration tab of a request form?? -->

<!--
 this is hidden, per Andrea:  

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

    When you go to the Planning section of Adobe Workfront objects, you can display both connections with linked records or any available connections with Planning record types. With that, you can view and edit any connection field without having to navigate away from the current section in Workfront to other areas. The Planning section is available for the following Workfront objects: Project, Portfolio and Program. For more information, see [Manage records in the Planning section of Adobe Workfront objects](https://experienceleague.adobe.com/ja/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-records/manage-records-in-planning-section).   


* Create new records within the connection fields - In-context creation of connected records https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6656c1a30026b903c6edf0210b8cbb23/overview?source-id=unifiedShareMFE  When you need to link records through a connection field but cannot find the required records in the connected record type, you can also create new records in the connected record type directly within the connection fields, with that you can efficiently establish necessary links without having to leave the current record type context. For more information, see Create records https://experienceleague.adobe.com/ja/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-records/create-records.   

     

* **Field on Customer Form** (CF)[ - [E] Make connected Planning data consumable through WF forms](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6641b040000b880ccd74aab6365c3361/overview?source-id=unifiedShareMFE) _(Planned completion date Sep 15, 2024 10:00 PM)._ Considering that the Workfront Project metadata modeling is done through forms, you are also able to add Planning connections to your custom forms. You can embed any lookup field value from the connected Planning record types within the custom form of your Workfront object. With that capability, when you are managing objects in Workfront, you can present any taxonomies or operational records connected to the Workfront object in custom forms, alongside other details, so that your teams can easily consume and update all the relevant information through a unified interface.  They should not need to navigate to different areas to view and update the information relevant for their work.  

     

* **Connection between Workspaces with Record types accessible from multiple workspaces** – ~~Epic – "[Connect to record types across workspaces](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/64dfad3100027190324dcc35b2176e76/overview?source-id=unifiedShareMFE)"~~ When you are creating a workspace in Planning, you can define certain record types once and then configure them to be accessible from multiple workspaces so you can create connections with them from anywhere. This way, you can streamline the data management process, eliminate duplicative work, and ensure data consistency across teams. As a result, your teams can tag their records with common taxonomies and unlock better visualization, filtering, grouping, and reporting of cross-team work.  For more information, see [Edit record types](https://experienceleague.adobe.com/ja/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-architecture/edit-record-types). 

     

* **Fusion connector – You can create a connection to your Workfront Planning account from inside a Workfront Fusion module. **With this connector, you can trigger a scenario when events occur in Workfront Planning. You can also create, read, update, and delete records, or perform a custom API call to your Adobe Workfront Planning account. More information in Experience League in[ Adobe Workfront Planning modules](https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-fusion/fusion-apps-and-modules/workfront-planning-moduleshttps:/experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-fusion/fusion-apps-and-modules/workfront-planning-modules) article.  

-->