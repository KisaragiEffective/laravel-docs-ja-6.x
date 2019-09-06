# Laravel6.0LTS公式ドキュメント翻訳リポジトリ

このリポジトリはPHP Webアプリフレームワーク、Laravel6.0LTSの公式英文ドキュメントを日本語へ翻訳しています。

This is a Japanese translation repository for Laravel 6.0LTS official documentations.

翻訳内容は、<https://readouble.com/laravel/6.0LTS/ja>で公開しています。

> 注意：Laravel開発者のTaylor Otwell氏は、英語のネイティプスピーカーです。英語しか理解できません。
> 自分の理解できないものには責任が持てないと言う理由から、
> 公式ドキュメントは英語のみです。そのため、日本語翻訳を「公式」と呼ばないでください。
> 「日本語ドキュメント」、「和訳翻訳ドキュメント」など適切にお呼びください。

### 誤訳／タイポなどの報告

* 誤訳やタイポ、未翻訳部分などを報告する場合、以下の内容を含めてください。
    * ページ（章） GitHubのリポジトリやreadouble.comのURL、もしくはページのタイトル（「キュー」、「認証」）など。ページの特定が容易であれば形式はかまいません。（報告に手間がかかるので、行番号を含めたリンクをわざわざ張る必要はありません。）
    * 問題のある和文と正しいと思われる和文（エディターで検索して該当箇所を見つけます。）
* 専門用語（訳語）の不統一に関しては、プロジェクト全体を検索しますので、特定のページを指定する必要はありません。それ以外の表記揺れに関しては、該当ページが分かるようにしてください。（表現上の揺れなどは、一度に変更できません。少しづつ、気がついた時点で修正します。）
* 日本語ドキュメントを利用するのは日本人です。そのため、報告やコメントは日本語で記述してください。
* このリポジトリでは6.0LTSの翻訳和文のみ管理しています。readouble.comで公開している他のバージョンの和文に関しては、@HiroKwsにツイートいただくか、hirokws@gmail.comへご連絡ください。なお、メンテナンス期間をフレームワーク本体と合わせているため、readouble.comで公開している日本語翻訳の旧バージョンは更新していません。バージョン6.0LTSリリース時点で、メンテ対象の和文バージョンは6.0LTSのみです。

#### issueで報告する場合

Issueで報告していただくのが、一番簡単です。

<https://github.com/laravel-ja/ja-docs-6.0LTS/issues>のページで、"New issue"ボタンをクリックし、issueを発行してご報告ください。

#### プルリクエストで報告する場合

* translation-jaディレクトリ下の日本語翻訳Markdownファイルのみを変更してください。それ以外のファイルは変更しないでください。
* 翻訳対象となるバージョンの原文は、original-enディレクトリ下にあります。Laravelのドキュメントリポの最新版ではないことに注意してください。
* ディレクトリ／ファイル構造を変更しないでください。
* 原文と翻訳の文章構造は一致させてください。原文と翻訳は、空行・タイトル行など行ごとの構造を同一に保っています。これにより、翻訳が原文のどの箇所であるかを簡単に見つけることができます。また、原文の変更を翻訳へ反映させる処理を自動化するにも役立てています。
* 原文／翻訳間のファイル構成の一致のチェック、原文／翻訳間の各ファイルの行構成の一致のチェック、用語の不一致のチェックを行うスクリプトが、scripts/pre-commitです。可能であればこれをコミット前に実行し、確認してください。実行にはgawk、awk、sed、bashなどが必要です。
* pre-commitは、プルリクエスト時にCIでも実行されています。エラーになるものはマージしません。

### ディレクトリ構造

| ディレクトリ／ファイル  | 内容                               |
| ----------------------- | ---------------------------------- |
| original-en    | 翻訳対象原文ブランチの内容                  |
| translation-ja | 日本語翻訳Markdownファイル                  |
| scripts        | 用語統一、文章構造確認などの補助スクリプト   |


### タグ

| タグ形式               | 内容                                                       |
| ---------------------- | -----------------------------------------------------------|
| published.YYMMDD.HHMM  | readouble.comへ公開したコミット                            |

`published.YYMMDD.HHMM`形式のタグは、readouble.comなどで翻訳文を読む利用者向けのタグです。この形式のタグ間でdiffを確認してもらうことで、前回のリリース時の原文／翻訳文と次回の変更点／差分を確認できます。

### メンテナンス期間

原則、Laravel6.0LTSのメンテ期間である半年間。次回のバージョンのリリースまで。２０１９年８月頃までの予定です。

メンテ作業が煩雑になった場合は、期間途中でもリポジトリを閉じます。予めご了承ください。

### メンテナンス方針

日本語翻訳の構造は英語と一致させています。行数も変更していません。これにより、原文の変更点の和文への適用などを自動化しています。また、行で対応することで、日本語訳に対する英文を見つけ出しやすくしています。

重大な原文の間違いがない限り、和文に情報を付け加えません。LaravelメンテナのTaylor Otwell氏は、「ドキュメントに何もかも詰め込んでしまうと、メンテしづらく、読み手にも負担になる」という方針です。その方針を基準に現在の情報量となっています。それを尊重しています。

また、以前は日本語訳にいろいろと注釈を付け加えていましたが、長期間のメンテナンスでは管理が負担になります。作業をシンプルに保たないと長期間のメンテナンスは困難です。その理由でも、原則注釈は付け加えていません。

日本語訳に足りない部分は、原文に足りない部分です。公式ドキュメントに足りない部分を追加するPRを行うか、もしくはブログ記事を書き、内容を補ってください。また、原文の間違っている箇所、わかりづらい箇所に付きましては、原文のリポジトリへの報告や修正依頼をお願いします。

### 翻訳方針

翻訳が必要なのは、英語が苦手な方です。「英語を読むことが苦手な技術者」をターゲットとして翻訳しています。そのため、訳語が日本のコミュニティで定まった用語は、それを尊重しています。英単語が技術用語として定着している言葉は、日本語読みを採用しています。（リクエスト、イベントなど）また、まだ適切な用語が存在しない部分についても、米語発音を基本に訳語として採用しています。

初学者に対して読みやすくすることは、学習を終えたレベルの技術者にとって冗長になります。そのため、初心者に優しくするよりは、ある程度のレベルの技術者であれば親しんでいる、もしくは調べれば意味の取れる専門用語レベルを選んでいます。

バリデーションの一覧表記などは、原文のままが良いと言う意見があります。私も翻訳し直す機会ごとに、訳すのか原文のままにするか判断しています。現時点の判断では、基本的な方針に従い、専門的（コンピューター／数学分野／ソフト開発業界用語）な用語に訳しています。なぜならば、英文のままでは苦手な方にとって意味が分かりませんが、和文であれば必要に応じて意味を調べられるからです。

訳出の変更などのissueは、「英語を読むのが苦手な技術者」の視点で検討してください。issueを発行してくださる方は英語が読める方が多く、翻訳を公式ドキュメントの補助として利用している方も多いでしょう。私自身もそう利用していますが、原則は補助として利用する目的でなく、英語の公式ドキュメントを読解するのが困難な技術者の手助けにしていただくのが方針です。
