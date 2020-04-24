# Signate COVID-19チャレンジ 向けのツール


## COVID-19チャレンジ（フェーズ1）
### PDF加工
#### 導入
* python をインストール
* 以下のコマンドでライブラリをインストール
```
pip install numpy
pip install pandas
pip install openpyxl
```
#### 使い方
1. PDFファイルを取得
    * 現在千葉のコロナウィルスの患者発生状況のサイトから取得
    https://www.pref.chiba.lg.jp/shippei/press/2019/ncov-index.html
    * https://www.pref.chiba.lg.jp/shippei/press/2020/ncov20200408-2.html
      のようなPDFにのみ対応しています。
1. ファイルの中身を全選択を行いテキストファイルにすべて貼り付ける。
1. 貼り付けた後患者の情報以外の部分を削除する。
    * ○患者（千葉県内XXX例目）の概要 と記載されている部分のみにする。
1. `readPdfText`を実行する。
    * 複数ファイルを配置しても実行できる。
1. `output` ディレクトリの下に症例番号、年齢、職業などがまとまった状態のエクセルが出力される。
1. 該当の症例について　__COVID-19チャレンジ（フェーズ1）__ の該当の箇所に転記する。
