requor
======

## 概要

お産でつくるアプリ、「REQUOR」のリポジトリです。

### 名前

「REQUOR」 = LIQIOR + REQUEST の造語です。

### どんなアプリ？

「今日飲みたい」と思った時に今夜暇で一緒に飲みに行ってくれる人を見つけたい  
酒好き飲み会好きの社会人向けの、  
REQUOR（リカー）というプロダクトは、  
シンプルな酒飲み用コミュニケーションアプリです。  
これは今日一緒に飲める人をひと目で知ること、簡単に飲みに誘えることができ、  
sakebii（ http://www.sakebii.com/ ）とは違って、  
ごくシンプルな操作で飲み会までこぎつける機能が備わっている。  

飲み会の場所とか誰が幹事するかとかは適当に他のアプリで決めてください。

### 問題意識

* 急にお酒が飲みたくなったのに、今日誰が暇で一緒にお酒を飲んでくれそうかわからない
* Twitterとかで「お前ら飲みに行くぞ！」って書かれてても見逃してしまう
* LINEやIRCで飲みに誘うのがめんどくさい

### 解決策

* 今日自分と同じように飲みに行きたい人をすぐに見つけることができる
* 飲みに誘ったり誘われたりすることがもっと簡単にできるようになる

## 仕様

http://gyazo.com/b38613b96436434d928ae4106bf6145f

基本的に最初は4画面内で遷移させます。操作はタップのみです。

* 起動画面
* ログイン画面
* 飲みたいステータス一覧
* バディ追加画面

### 起動画面

アプリを起動したときに表示されます。
その後にログイン画面へ移行します。

### ログイン画面

facebookでログインします。
理由はFacebookのほうがリアル知人の友達数が多そうだからです。

### 飲みたいステータス一覧

ここでできるのは以下の行動です

* 自分の飲みたい/飲みたくないステータスの変更
* 友達の飲みたい/飲みたくないステータス確認
* 飲みたいステータスになっているひとを誘う

自分のステータスもここで変えることができます。
操作はタップのみです。タップすることで飲みたい/飲みたくないというステータスに変えることができます。
飲みたいステータスになっている人のセルをタップすると「LET'S DRINK!」になります。
アカウントのサムネとステータスの表示だけです。
テーブルビューを使えばいいと思います。

### バディ追加画面

この人を飲みに誘ってみたいとか、いつも飲みに行く人なんかをフォローすることができます。
Twitterのフォロー/フォロワーではなく、LINEの友達のような感じで誰でも追加できて、誰にでも通知が送れます。
こちらも友達か友達じゃないかのステータスと、アカウントのサムネが表示されています。
テーブルビューを使えばいいと思います。

### 必要な機能

- [ ] facebookログイン（サインアップ）/ログアウト機能（ログアウト機能つけるのわすれてた）
- [ ] 飲みたい/飲みたくない/飲みに行こうステータス
- [ ] 友達追加
- [ ] プッシュ通知（飲みたいステータスの人を誘った際に、その人に通知を飛ばす）
- [ ] facebookの友達でアプリを使っている人を表示する
- [ ] 朝の6時を過ぎたら自動的にステータスがリセットする

### つけたい機能

- [ ] 何が飲みたいかのステータス（BEERやWINE、WHISKYやSAKEなどなど）
- [ ] プッシュ通知（夕方くらいに「お疲れ様！今日も一杯いっとく？」みたいなこと表示させたい）
- [ ] 友達をアプリに誘致する機能
- [ ] 友達を候補から消す機能
- [ ] 友達設定を解除する機能
