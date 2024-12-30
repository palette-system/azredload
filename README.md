# 概要
<img src="/images/gaiyo.png"><br>
<br>
azir（エーゼット、アイアール）は自作の赤外線キーボードを誰もが作れるようにするためのプロジェクトです。
<br><br>

<b>簡単に作れる</b><br>
プログラムを書いたり利用の申請も出す必要が無く、ファームウェアを書き込んでGUI上で2～3分操作すれば自前の赤外線キーボードが作れる。<br>
<br>

<b>長時間動作</b><br>
BLEや電波を使用せず赤外線LEDを光らせるだけなのでボタン電池で長時間動作します。<br>
<br><br>

## AZTOOL
AZシリーズのキーボードの設定ツールです。<br>
REMAPやVIALのような位置づけで、自前で作成したキーボードのキー配列の登録やキーマップの設定を行えます。<br>
新しいキーボードを作った場合に申請は必要なくキー配列の設定も含めてキーボード本体(ESP32S3内)に保存します。<br>
作成者は自分が作成したキーボードの情報を設定後、AZTOOL内から「設定をエクスポート」してZIPファイルとして保存する事ができるので、ZIPファイルを配布する事で自作したキーボードの設定を共有できます。<br>
購入者はAZTOOL内から「設定のインポート」でZIPファイルを指定すると、作成者のキーボードを使えるようになります。<br>
<br>
リンク： <a href="https://palette-system.github.io/aztool/">AZTOOL</a><br>

<br><br>

## AZ-CORE ファームウェア
AZシリーズのキーボードファームウェアです。<br>
QMKやPRKのような位置づけになりますが、コードを書いたりコンパイルする必要はありません。<br>
ファームウェア書き込みサイトからESP32S3に書き込みを行うだけで使用できます。<br>
COL、ROWなどのピン設定はAZTOOLから行います。<br>
<br>
リンク： <a href="https://palette-system.github.io/az-core/index_s3.html">AZ-COREファームウェア</a><br>

<br><br>

## AZSENSOR
AZSENSOR（エーゼット、センサー）は赤外線キーボードの信号を受け取るためのセンサーです。<br>
中身はただの赤外線センサーで、より広範囲の赤外線信号を受け取るためのセンサーです。<br>
これを使用しなくても赤外線用のフォトトランジスタをESP32S3に接続するだけでも赤外線キーボードとして使用する事ができます。(ただし受光角度が30°しかなかったり制限が入ります)<br>

<br><br>

## AZIR50
AZIR50（エーゼット、アイアール、フィフティ）は接続されたスイッチをキースキャンしてボタンが押されたら押下データを赤外線で送信するマイコンボードです。<br>
ProMicroやRP2040ボードのような位置づけです、ファームウェアを書き込む必要はありません。<br>
あらかじめファームウェアが書き込まれているので開封して電池を接続するだけで動作します。<br>
COL、ROWなどのピン設定は無くあらかじめCOL1～5、ROW1～5のピンがあるのでそのピンを使用して下さい。<br>
電池は1.8V～5.5V内の電池を接続して下さい。ボタン電池（CR2032）1つで連続稼働10日以上動作しました。<br>

<br><br>

# ライセンス
MIDライセンスとします。<br>
ドキュメント、ファームウェア、Github上にあるソースは好きに使って頂いて大丈夫です。<br>
ただし発生した問題、不具合は自己責任とし、パレットシステムはいかなる責任も持ちません。<br>

