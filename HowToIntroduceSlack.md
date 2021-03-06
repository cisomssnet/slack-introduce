# Slackを導入する

### Slackって何？
Slackは企業向けのコミュニケーションツールです。  
LINE感覚でやり取りができるため、便利です。

### 何のためにこれやるの？
今現在使われているサイボウズライブがサービス終了するから別のツール探す必要があった。  
勤怠連絡などの連絡はもちろん、シフトを入れるようにできるプラグインなどを開発する予定なのでSlack上でシフト関連のすべての操作ができるようになる。

### Slackの導入方法
1. 管理者にメールアドレスを教えてSlackのワークスペースへ招待してもらう。  

2. メールアドレスにSlackからメールが来ているはずなのでリンクをクリックして参加する。

3. 氏名や表示名などの登録ページに飛ぶので入力して「次へ」を押す。  
\* もしかしたら利用規約などの確認ページに飛ぶかもしれないけど気にせず次へ

4. ほかのメンバーを招待するかどうか尋ねられるが、「後で」を押す。

5. Slackのメイン画面が表示されたらSlackへの登録は完了。  
\* メイン画面に行く前にチュートリアルがあるかもしれない  

6. 管理者に`# シフト`チャンネルに招待してもらう。

7. Slackには[デスクトップアプリ](https://slack.com/intl/ja-jp/downloads/windows)やスマートフォン向けアプリ([android](https://play.google.com/store/apps/details?id=com.Slack&hl=en)/[iOS](https://itunes.apple.com/jp/app/slack/id618783545?mt=8))などがあるので、  
自分のpcやスマートフォンにインストールしておく。（任意だけどあると便利だよ）

8. デスクトップアプリやスマートフォン向けアプリでSlackにサインインするとき、最初にワークスペースを聞かれるけど、`technofer`です。

9. 終わり

# それで、どうやってシフト管理するの？
当たり前ですが、Slackはシフト管理するアプリではないので、これ単体では意味がありません。  
SlackとGoogle Calendarを同期させてシフトを管理します。  

必然的にグーグルアカウントが必要になりますが、日本工学院の学生の方は学内メールアドレス(it-neec.jp)で既にグーグルアカウントが作られているのでそれを利用するとよいと思います。  

その他の方は、既存のアカウントを使うかなければ新しく作成してください。

### Google Calendarを作る
1. [Google Calendar](https://calendar.google.com/calendar/)にアクセスする。  

2. 画像を参照して新しいカレンダーを作る。  
カレンダー名は`technofer@[自分の苗字]`にしてください。  
例：technofer@峯島<br>  
<img src="img/bandicam_2018-08-31_16-39-52-689.jpg" width="300">

3. マイカレンダーに作ったカレンダーが表示されていることを確認してください。

4. 画像を参照して`設定と共有`を開きます。<br>  
<img src="img/bandicam_2018-08-31_16-54-34-588.jpg" width="300">

5. 特定のユーザーとの共有で、カレンダーを共有したい相手のメールアドレスを追加します。<br>  
ここで管理者であるc.isomss.net@gmail.comには`予定の変更権限`を与えます。  
それ以外のユーザーには`閲覧権限（すべての予定の詳細）`を与えてください。  
どのメールアドレスを追加すればよいかは管理者に問い合わせてください。<br>  
以下のようになっていればOKです。<br>  
<img src="img/bandicam_2018-08-31_17-12-53-011.jpg" width="300">

6. これでGoogle Calendarの作成は終了。

### SlackとGoogle Calendarを同期させる
これでSlackの導入、Google Calendarの作成が終わりました。  
あとは、これらを同期させるだけです。

1. Slackを起動し、どこか適当なチャンネルまたはDMで`/apps Google Calendar`とチャットを入力する。  

2. すると以下の画像のようなbotがアプリケーションを検索し、ヒットしたものを表示してくれるので一番上の`Google カレンダー`を選択する。<br>  
<img src="img/bandicam_2018-08-31_17-36-49-422.jpg" width="300">

3. SlackのAppディレクトリに遷移するので、 `Google Accountを接続する`を押す。

4. アカウントの選択画面に遷移したらSlackを登録したときに使用したメールアドレスをもつグーグルアカウントを選択する。  
日本工学院の学生ならば`it-neec.jp`のメールアドレス。

5. Slackがカレンダーにアクセスを求めることを許可するか問われるので許可する。

6. 以下の画像の画面に遷移したら、まず`Google アカウントを認証する`をクリックする。  
またグーグルアカウントを選ぶ画面に遷移するが、またかよとイライラせずに再度アカウントを選択する。  
選択後表示される画面で同じく、リクエストを許可するをクリック。<br>  
<img src="img/bandicam_2018-08-31_17-46-49-227.jpg" width="300">

7. 再度上記の画像と同じページへ遷移するが、いくつか項目が異なっている。  
下記の画像のようにカレンダーは`technofer@[苗字]`を選び、チャンネルは`# シフト`を選択する。<br>  
<img src="img/bandicam_2018-08-31_17-55-36-597.jpg" width="300">

8. 画面を下にスクロールするとイベントリマインダーなどいろいろな設定項目があるので、これを変更する。<br>  
イベントリマインダーを`15分前`から`2時間前`に変更する  
<img src="img/bandicam_2018-08-31_18-03-15-121.jpg" width="300">

9. 変更したら`インテグレーションを保存`をクリックする。

10. カレンダーが接続されました！という画面が表示されたら`完了する`をクリックしてください。

11. Slackの`# シフト`にインテグレーションが保存されたことが通知されていたらちゃんと同期されています。

12. これで作業は終了ですが、念のため作成したカレンダーに予定を書き込んでみてください。  
イベントが作成されたことがSlackに通知されなかったら作業に問題がある可能性があります。  
その場合は管理者に問い合わせてください。
