# Macの設定
## 音量
0 にする。

## マウス、カーソル、タッチパッド
[システム環境設定] - [トラックパッド]
基本的に全部にチェック

## カーソルサイズ
カーソルを探す時間は無駄なので、大きくする
[システム環境設定] - [アクセシビリティ] - [ディスプレイ] [カーソルのサイズ] スライダを右に移動

## 時計
いつでも事象の発生時刻を押さえられるようにしておくのが運用管理の鉄則
[システム環境設定] - [日付と時刻] - [時計]　で　[日付のオプション] の [日付を表示] にチェックを入れる

### キーボード
引用符（シングルクオートを開き引用符と閉じ引用符に変換しないようにする）

シングルクオートでくくったつもりが
開き引用符と閉じ引用符に変換される。
テキストに書いてあったコマンドをコピペして実行しようとすると実行できない、とか
プログラム書くとき面倒だったりするので直す。

[システム環境設定] - [キーボード] -[ユーザー辞書]
[スマート引用符とスマートダッシュを使用] のチェックを外す

# Macの設定
## Xcode & homebrew
`$ ./setup_dev_env_mac_1.sh`

## brew-file
`$ ./setup_dev_env_mac_2.sh`

## brew-file の取得
`$ ./setup_dev_env_mac_3.sh`

## brew-file からのインストール
`$ ./setup_dev_env_mac_4.sh`


## homebrew 後の設定

Touch Bar 搭載の MacBook Pro でファンクションキーを使う方法
- システム環境設定で、「キーボード」を選択します。
- 「ショートカット」をクリックします。
- 左側のサイドバーから、「ファンクションキー」を選択します。
- 「+」記号をクリックして、App を探して、Terminal/iTerm2 を選択します。

## VisualStudioCode インストール後の設定

PathにCodeコマンドをインストール
ターミナルで次の入力をすれば、指定したファイルがVSCodeで開きます。

code hogehoge.md
また、次の入力をすれば、現在のフォルダがVSCodeで開きます。

code .
設定方法ですが、VSCodeを起動してコマンドパレットを開き、pathと入力して以下を選択します。

## VisualStudioCode の拡張機能

| 拡張機能名称 | 概要 |
|:-----------|:-----------|
| Bracket Pair Colorizer | 対応する括弧を色で識別できる |
| JSON Tools | JSON整形（pretty / minify） |
| Paste JSON as Code | JSONに対応するコードを作成 |
| Log File Highlighter | ログファイルを色分けして表示 |
| Markdown All in One | Markdownの記述をサポート |
| markdownlint | Markdown用のLint |
| PlantUML | PlantUMLが使える |
| REST Client | VSCodeがRESTクライアントになる |
| Text Marker (Highlighter) | 任意のテキストにマーカーが引ける |
| vscode-icons | アイコンで分かりやすくなる |
| テキスト校正くん | 日本語の文章チェック |
