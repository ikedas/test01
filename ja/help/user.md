メーリングリスト - 利用する方むけの説明
---------------------------------------

### <span id="howitworks"></span>リストサービスのしくみ

当サイトでは、リストのサービスを**リスト管理ソフトウェア Sympa (サンパ)** によって提供しています。このソフトウェアでは、**リストごとにウェブインタフェースが設けてあります**。

**リストでなにかやりたいこと** (読者登録、個人設定を変える、など) があるのなら、2 つのやりかたがあります——

-   **リストサーバのウェブを使う**。
-   **電子メールでコマンドを送る**。Sympa の自動処理アドレス **{{conf.email}}@{{conf.host}}** へ送ります。

**Sympa にコマンドを送るには**、次のやりかたがあります——

-   **コマンドをひとつだけしか送らないのなら**、メッセージの表題 (Subject) に書き、メッセージの本文は空にしておきます。
-   **いくつかのコマンドを送るのなら**、メッセージの表題 (Subject) は空にしておき、メッセージの本文にコマンドを打ち込みます。**注意**: Sympa は、送ったメッセージの内容が厳密に規則通りになっていないと受け付けてくれません。たとえば——
    -   コマンドは一行ごとにひとつだけ。
    -   メッセージはテキスト形式で、HTML にしない (プレインテキスト) で送る。
    -   メッセージには、Sympa に理解できるコマンド以外はなにも書かない (署名を自動的に付けるようにしない)。

Sympa にメールで送れるコマンドすべての説明が[こちら](mail_commands.md)にあります。

### <span id="subscribe"></span>リストに読者登録する

リストへの読者登録のしかたは、とてもかんたんです——

1.  ****リストの読者登録につかう**アドレスを決める**。

    | Note |
    |------|
    | アドレスは、よくメールを読んでいて、十分な容量のあるものにしましょう。リストによっては、大量のメッセージや、ときには大きな添付ファイルがついたメッセージが流れることがあります。 |

    | Note |
    |------|
    | ひとつのリストに複数の異なったアドレスで読者登録してもかまいません。それには、メールクライアントで別のアドレスの設定を使って、読者登録の手順を繰り返さなければいけません。 |

2.  自分が読者登録したいアドレスから、**{{conf.email}}@{{conf.host}} に送るメッセージを**を作る。

    | Note |
    |------|
    | Sympa は人間ではなく、メーリングリストを管理するからくりです。ですから、甘い言葉を囁いても無駄ですよ ;-) |

3.  メッセージの表題 (Subject) に、**subscribe リスト名 自分の名前** (「リスト名」を自分が読者登録したいリストの名前に置き換え、半角の空白を空けて、その後に自分自身の名前を書きます) と書く。
4.  **メッセージの本文は空にしておき**、メッセージを送信する。

    | Note |
    |------|
    | ひとつのメッセージの中に複数のコマンドを書いて送れば、手間をはぶけます。それには、[リストサービスのしくみ](#howitworks)の節で説明した手順でやってください。 |

**この後、あなたの申込が受け付けられたか、認められなかったかを知らせるメッセージが届きます**: リストへの登録に承認が要るようになっているときは、オーナーがあなたを読者登録させないと決めることもありえます。そういうときに何度も読者登録の申込を送っても、無駄です。結果は変わりません。それよりも、リストのオーナー (リスト名-request@{{conf.host}}) に直接メールを送って、自分が読者登録の申込をした理由を説明してみましょう。

| Note |
|------|
| なお、あなたの確認がないと読者登録を実施しないリストもあります。そういうときは、届いたメッセージに手順が書いてありますから、それに従って確認をしてください。 |

リストの種類 (リストへの登録に条件があるかないか) によって、またはオーナーが休みをとっていたりすると、**お知らせが届くまで少々時間がかかることもあります**。何度も申込を送っても無駄です。

**申込が受け付けられると、リストへの登録を確認するメッセージが届きます。このメッセージ** (リストの読者の約款) **には、とても重要な情報が書いてあります。次のようなことです。**

-   あなたの**リスト用パスワード**。このパスワードは、あなたがあるアドレスで読者登録しているすべてのリストで共通です。リストのウェブサイトに接続して[個人設定のリンク](#global_pref "Comment modifier son mot de passe")で変えることができます。
-   **リストについての詳しい案内**<span lang="ja" lang="ja">——</span>内容、投稿保管庫のウェブアドレスなど。
-   **リスト利用の条件**<span lang="ja" lang="ja">——</span>扱える話題や扱わない話題、ネチケット、法的な情報、情報保護指針など。

**登録確認のお知らせは大事にとっておきましょう**。後で、パスワードを忘れてしまったり、Sympa になにか特別なコマンド (例えば、登録解除のコマンド) を送りたくなったりするかもしれませんから。一般的に言うと、**リスト登録確認のお知らせはすべてとっておくことをお勧めします**。

リストのサーバの**ウェブインタフェースから読者登録することもできます**。これをするには、次のようにしてください——

1.  リストのウェブサイトの**[ホームページ](%7B%7Bpath_cgi%7D%7D/home)**へ行き、**ログイン**します。
2.  自分が読者登録したい**リストの案内ページへ行きます**。
3.  左側のメニューで、**「読者登録」のリンクをクリックします**。

### <span id="sympa_auth"></span>リストのウェブサイトに接続する

リストのウェブサイトに接続するには、ウェブインタフェースの左側 (上のほう) のログイン用のエリアを使います。すでに本人確認がすんでいれば、ここに自分の電子メールアドレスと権限 (読者か、モデレータか、オーナーか) がでています。そうでなければ、本人確認用のフォームがでているはずです。

ひとりひとりの状況に応じて、ログインのしかたは変わってきます——

-   **メーリングリストサービスを提供する組織が一括認証技術** (サービスによらない共通のアカウントと本人確認手順。SSO *シングルサインオン* ともいいます。たとえば CAS システムなど) **を採用しているとき**は、自分用のアカウントを使ってログインします。そのためには、「**\[使っているシステムの名前\] 認証**」と書いてあるあとの「ログイン」ボタンをクリックします。そして自分のユーザ名とパスワードを打ち込み、認証サーバにログオンします。

    | Note |
    |------|
    | 一括認証のシステムでは、すでにほかのサービスでログインをすませていれば、あらためて本人確認をする必要はありません。必要ならページの再読み込み (リロード) をしてください。 |

-   **一括認証の手続きがなければ、あなたのリスト用のパスワードを使います**。この場合、普通のやりかたでログインをします。つまり、**自分が読者登録している電子メールアドレス**と、**リスト用のパスワード**を打ち込みます。

    | Note |
    |------|
    | 自分のリスト用パスワードが思い出せないときは、「パスワードを忘れた」をクリックします。そして、自分の電子メールアドレスを入力します。そのアドレスに確認用 URL の入った電子メールが送られてきます。 |

-   **一括認証の手続きがなく、リストのパスワードもまだない**、というときは、「**まだログインしたことがない**」をクリックし、自分の電子メールアドレスを打ち込みます。すると、確認用 URL の入った電子メールがそのアドレスに届きます。そこで、パスワードを決めることができます。

| Note |
|------|
| 備考: リスト用のパスワードは、メーリングリストのサービスだけで通用する特別なパスワードです。 |

### 読者登録状況を見る

読者登録しているリストの一覧を見るには、まず[ログイン](#sympa_auth)しなければいけません。すると、左側の「あなたの関わっているリスト」にリストとその簡単な説明の一覧が出ます。

**リストの案内ページを見るには、リスト名をクリックします**。案内ページにはリストの説明 (目的、メッセージを送るときのきまりなど) があります。説明文の長さはリストによってまちまちです。

この案内ページでは、次のようなことができます——

-   自分の[読者登録の設定](#options)を変える、
-   [リストの投稿保管庫](arc.md)を見る、
-   [投稿保管庫にあるメッセージを探す](arc.md#arcsearch)、
-   [新たにメッセージを送る](sendmsg.md)、
-   共有文書置き場から[文書をダウンロードする](shared.md#shared_read)、
-   共有文書置き場に[文書をアップロードする](shared.md#shared_upload)。
-   リストの[読者一覧を見る](#subscribers) (見られるようになっていれば)、
-   リストごとに受け取りを[休止したり再開したりする](suspend.md)。
-   リストの[登録解除](#unsubscribe)をする。

<span id="subscribers"></span>リストに**読者登録している人の数**が、つねに**左側のメニュー**に出ています。**読者一覧を見るには、**左側のメニューの**「読者一覧」のリンクをクリックします** (リストのオーナーが読者一覧を閲覧できないようにしているときは、このリンクは使えません)。読者一覧を出すと、読者ひとりひとりの**電子メールアドレス**と**名前**を見ることができます (読者登録のやりかたによっては、名前が出ないこともあります)。

| Note |
|------|
| 最初は、一ページに 25 名ずつ表示するようになっています。矢印のリンクで他のページを見たり、一ページに表示する人数を変えたりできます。また、項目の見出しをクリックすれば、読者を電子メールアドレス、ドメイン名、名前で並べ替えることができます。 |

**リストのオーナーとモデレータの名前も、左側のメニューに出ています**。しかし、それぞれのオーナーやモデレータに直接メールを送ってはいけません。なにか質問や意見があれば、次のアドレスに送るようにしてください: **リスト名-request@{{conf.host}}** (「リスト名」のところを、対象のリストの名前に読み換えます)。

自分が**いつ読者登録したか**や、**最後に読者登録の設定を変えたのはいつか**を知りたいときは、左側のメニューの**「読者登録の設定」のリンクをクリックします**。

### <span id="pref"></span>個人設定

いろいろな**個人設定を変える**ことで、**リストがもっと使いやすくなります**。変えることのできる個人設定は、大きく 2 種類に分かれます。

-   **読者登録の設定** (リストごとに異なる)、
-   **個人設定** (Sympa のメーリングリストウェブサイト全体で共通)。

#### <span id="options"></span>読者登録の設定を変える

**読者登録の設定は、リストごとに違っていてもかまいません**。変えるには、次のようにします。

1.  リストのウェブサイトの**[ホームページ](%7B%7Bpath_cgi%7D%7D/home)**へ行き、**ログイン**します。
2.  **リストの案内ページへ行きます**。ここで読者登録の設定を変えられます。
3.  左側のメニューで、**「読者登録の設定」のリンクをクリックします**。
4.  <span id="deliverymode"></span>**受け取りモードを決める** (モードは一度にひとつしか選べません。複数のモードは選べません)。次のようなモードがあります。
    -   **まとめ読み (MIME)** (digest): メッセージを普通に受け取るのではなく、ある期間ごとにまとめて受け取ります。リストのメッセージを multipart/digest MIME 形式でまとめてあります。どのくらいの間隔でまとめ読みを送るかは、リストのオーナーが設定して決めます。
    -   **まとめ読み (プレインテキスト形式)** (digestplain): メッセージを普通に受け取るのではなく、ある期間ごとにまとめて受け取ります。リストのメッセージをプレインテキスト形式でまとめてあります。どのくらいの間隔でまとめ読みを送るかは、リストのオーナーが設定して決めます。
    -   **メッセージの一覧** (summary): メッセージを普通に受け取るのではなく、ある期間ごとにメッセージの一覧を受け取ります。メッセージを実際に読むには、ウェブの投稿保管庫を見にいかなければなりません。
    -   **表題 (Subject) のみ** (notice): このモードでは、メッセージの中身は受け取りません。メッセージが届いたことがすぐにわかり、メールボックスが満杯になってしまう心配はありません。
    -   **なにも受け取らない (休暇などのときに便利)** (nomail): このモードにすれば、リストのメッセージを受け取らないようにできます。これは特に、メールボックスに長期間アクセスできないがリストには読者登録したままでいたい、というときに便利です。
    -   **テキストのみ** (txt): このモードでは、メッセージに 2 種類の形式 (プレインテキストと HTML) の同じ内容が含まれているときも、プレインテキスト版 (text/plain) のみを受け取れます。
    -   **HTMLのみ** (html): このモードでは、メッセージに 2 種類の形式の同じ内容が含まれているときも、HTML 版 (text/html) のみを受け取れます。
    -   **添付ファイルを URL にする** (urlize): このモードでは、添付ファイルを受け取らなくてすみます。その添付ファイルのかわりにメッセージには URL が入っているので、それを使えば投稿保管庫で読めます。
    -   **自分が投稿したものは受け取らない** (not\_me): このモードにすると、自分が投稿したものの写しを受け取らないようになります。
    -   **標準 (直接受け取る)** (mail): 最初はこの受け取りモードになっていて、ほかのモードははたらきません。
    -   **休止中**: このモードにすると、あるリスト (複数可) からのメッセージの受け取りを一定の期間休止できます。再開もできます。登録解除とはちがって、読者登録はしたままで「受け取りを休止/再開」からいつでも受け取りだけを休止したり再開したりできます。
5.  読者一覧での**見えかた**を決められます。
    -   **読者一覧に載せる** (noconceal): 自分の名前と電子メールアドレスが読者一覧に載ります (ただし、リストのオーナーが、読者一覧を読者が見られるようにしている場合)。
    -   **読者一覧では隠す** (conceal): 自分の名前と電子メールアドレスを読者一覧に載せません。ただし、メッセージを送れば投稿保管庫には電子メールアドレスが残ります。
6.  **「更新」ボタンをクリックします**。

#### <span id="global_pref"></span>個人設定を変える

個人設定は、読者登録しているすべてのリストと、Sympa のウェブインタフェースでの表示にたいしてはたらきます。設定を変えるには次のようにします。

1.  リストのウェブサイトの**[ホームページ](%7B%7Bpath_cgi%7D%7D/home)**へ行き、**ログイン**します。
2.  画面の上のほうの**「個人設定」のリンクをクリックします**。
3.  **設定を変えます**。
4.  **「設定」をクリックする**と、オプションがすべて変わります。

次のものを変えられます。

-   自分の**名前**。メーリングリストサーバのウェブインタフェースでリストに読者登録すると、登録したリストでの「名前」欄に自動的にこの名前が入ります。
-   **Sympa のウェブインタフェースで表示に使う言語** (ページを見ている途中で言語を変えることもできますが、「個人設定」ページで変えた言語の設定は残ります)。
-   **Sympa が自分のコンピュータに入れるクッキーの有効期間** (「接続の有効期間」)。最初は、ブラウザを終了するとセッションの期限が切れるようになっていますが、メーリングリストサービスをよく利用する方は、長い期間にしておくことをおすすめします。

    | Note |
    |------|
    | クッキーは、ウェブサーバがあなたのコンピュータのハードディスクに (ほとんどの場合は一時的に) 書き込む小さなファイルです。これによって、あなたがそのサーバのサービスの利用者であることを識別します。これにはあなたに関する若干の個人情報 (名前、電子メールアドレス、最後にログインした時刻など) が入っています。 |

-   リストに**読者登録した電子メールアドレス** (読者登録に複数のアドレスを使っているときは、ログインしているアドレスのみが変わります)。

    | Note |
    |------|
    | 注意: 登録しているリストすべてのアドレスが変わります。特定のメーリングリストでだけアドレスを変えたいのでしたら、いったんそのリストを登録解除し、正しい電子メールアドレスで読者登録しなおすとよいでしょう。 |

-   自分の**メーリングリストのパスワード**。

「**他の電子メールアドレス**」の項目で、アドレス変更と同じようなことができます。

### リストを探す

メーリングリストを探したいこともあるでしょう。これには 3 つのやりかたがあります。

-   ウェブインタフェースの**[ホームページ](%7B%7Bpath_cgi%7D%7D/home)のリンクから探す**、
-   ホームページの**「リストを探す」を使う**。探す条件に打ち込んだテキストがリストの名前か説明に入っているものが、すべて出ます (リストの説明は、ふつうは簡単な文です)。
-   ページ上部の「[リスト一覧](%7B%7Bpath_cgi%7D%7D/lists)」タブをクリックして**利用できるリストすべてを表示する**。

| Note |
|------|
| 自分の電子メールアドレスのドメイン (たとえば *cru.fr*、*fai.com* など) や、どこからログインしたかによって、同じリストでも一覧に表示されたりされなかったりする場合があります。ですが、表示されないリストでもリスト名を知っていれば読者登録できます。[電子メールクライアントを使う](#subscribe)やりかたを見てください。 |

### <span id="archives"></span>ウェブで投稿保管庫の投稿を読む

やりかたは[**投稿保管庫の説明**](arc.md)を見てください。

### <span id="sendmsg"></span>メッセージを送る

やりかたは[**メッセージの送りかたの説明**](sendmsg.md)を見てください。

### <span id="shared"></span>共有文書置き場を使う

やりかたは[**共有文書置き場の説明**](shared.md)を見てください。

### <span id="suspend"></span>リストごとに受け取りを休止したり再開したりする

やりかたは[**受け取り休止/再開の説明**](suspend.md)を見てください。

### <span id="unsubscribe"></span>リストの登録解除をする

リストの登録解除をするには、次のようにしてください——

1.  リストに読者登録していたアドレスを解除するには、**{{conf.email}}@{{conf.host}} にメッセージを**送ります。
2.  メッセージの表題 (Subject) に、次のように書きます: **unsubscribe リスト名** (「リスト名」を、登録解除したいリストの名前で置き換えます)。
3.  **メッセージの本文は空にしておき**、メッセージを送信する。

    | Note |
    |------|
    | ひとつのメッセージの中に複数のコマンドを書いて送れば、手間をはぶけます。それには、[リストサービスのしくみ](#howitworks)の節で説明した手順でやってください。 |

リストのウェブインタフェースで登録解除することもできます (登録解除したいリストごとに同じ手順を繰り返されければいけません) ——

1.  リストのウェブサイトの**[ホームページ](%7B%7Bpath_cgi%7D%7D/home)**へ行き、**ログイン**します。
2.  登録解除したい**リストの案内ページへ行きます**。
3.  **左側のメニューで、「登録解除」のリンクをクリックします**。

------------------------------------------------------------------------
