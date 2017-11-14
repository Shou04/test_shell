■制限
・環境変数のpathにjavaがあること(javaコマンドが実行可能)。
・Java6以上で動作可能。
・Java5以下の場合はクラスパス設定の部分で修正が必要。
  (「%BATCH_LIBRARY_PATH%/*」のアスタリスクでの指定が使用できない)

■実行
Windows上でsample.batを実行します。
Linux上でsample.shを実行します。

■引数
引数がなければ正常終了(0)を返却する。
引数があれば異常終了(1)を返却する。

■ディレクトリ構成
batch
├bin 実行フォルダ
│ ├sample.bat
│ └sample.sh
│
├conf
│ ├logback.xml ログ設定
│ ├batch.conf Linux用設定ファイル
│ └batch.ini Windows用設定ファイル
│
├lib ライブラリ
│ ├logback-classic-0.9.18.jar
│ ├logback-core-0.9.18.jar
│ ├slf4j-api-1.5.11.jar
│ └sample.jar
│
├log ログフォルダ
│ └batch.log
│
└src
   └jp
     └co
       └test
          └Sample.java
