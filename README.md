# YamaLabo Project2019
情報学プロジェクトのプロジェクト管理用リポジトリです。  
タスク管理および進捗確認はすべてここで行います。

- [プロジェクト管理表](https://github.com/moririn772/yamalabo-project-2019/projects/1)
- [タスクを追加するページ](https://github.com/moririn772/yamalabo-project-2019/issues/new)

<br>

## ドキュメント類

- [先生が書いたドキュメント](https://github.com/ShigeichiroYamasaki/yamalabo)
- [MacOSでbitcoinの開発環境をセットアップする(1)](https://gist.github.com/moririn772/e75d57a1d1ea9b6a35c5bd4bb188b1ba)
- [bitcoin-ruby ハンズオン](https://github.com/ShigeichiroYamasaki/yamalabo/blob/master/bitcoin-ruby.md)

<br>

## 進め方と担当分け

| 役割  | メンバー | やること   |
| ---- |------- | -------- |
| UI設計 | Suga, Fujiwara | 画面設計とか |
| アプリケーションA | Mori, Iseki, Ishimoto | Railsアプリケーションの実装 |
| アプリケーションB | Yoshida, Yamauchi, Yunoki | Railsアプリケーションの実装 |


<br>

## スケジュール

| 回数 | 日付   | やること／やったこと   |
| ---- |----- | -------- |
| 09 | 11/19  | Bitcoin Core をインストール確認。bitcoin-rubyでRPCを用いた操作の確認 |
| 10 | 11/26  | アセットの発行をやってみる |
| 11 | 12/03  | -     |
| 12 | 12/10  | -     |
| 13 | 12/17  | -     |
| 14 | 1/14   | -     |
| 15 | 1/21   | 予備日 |
| 16 | 1/28   | 予備日 |

<br>

## 使い方

### Issues
新しいタスクに取り掛かるとき or あとでやるタスクを思いついたときなど、新しいIssueを立ててください。  
必要であれば "たすけて","バグ","質問" のラベルを活用して、Issueを立ててください。誰かが助けにいきます。

### Projects
カンバン方式で誰が何のタスクに取り組んでいるのかを可視化します。  

### Pull requests
ここでは使いません。

<br>

## こんなときどうする？

### やることリストに取り掛かるぞ！
やることリスト の該当のタスクを 進行中 に移動します。  
その際に、Assignee が自分になっているか確認してください。  
既にアサインされている人が自分以外の場合は変更してください。

### 進行中のタスクが終わった！
該当のタスクを 完了 に移動してください。
 
### 新しいタスク思いついた
Issue > New Issue から、新しくIssueを作成してください。  
この際に以下のことをやります。    
・必要があればラベルをつける  
・Projectは YamaLabo2019 を選択する（自動でToDoリストに追加される）   
・Assinee(そのタスクを担当する人) が決まっていれば、適切な人を設定する  
・説明文は書いても書かなくてもいいです（できれば書いてね★）

<br>

## 使い方

### はじめに

```
git clone https://github.com/moririn772/yamalabo-project-2019.git
cd yamalabo-project-2019
rbenv install 2.5.7
rbenv rehash
rbenv local 2.5.7
ruby -v
# => 2.5.7が出たらOK

gem install bundle
bundle install --path=vendor/bundle
bin/rails db:create
bin/rails db:migrate
bin/rails s
# localhost:3000で見れたらOK
```

## openassets-rubyをrails　に組み込む

* rails 5.2.3
* ruby  2.6.3

gemのopneassets-rubyとbitcoin-rubyとのversionを合わせるため

gem 'ffi', '1.9.18'

を追加

Refer: [https://y-nakajo.hatenablog.com/entry/2017/11/02/120529](https://y-nakajo.hatenablog.com/entry/2017/11/02/120529)

