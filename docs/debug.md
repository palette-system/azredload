## 赤外線キーボードが反応しない
<br><br>

<b>太陽光があたっている</b><br>
カーテンがかかっている部屋程度ならば大丈夫ですが、部屋に太陽光が直射していると太陽光に含まれている赤外線に反応してしまいうまく動かない事があります。<br>
カーテンをかけるか、夜に動作するか確認してください。<br>
<br><br>


<b>センサーからの角度と距離</b><br>
使用する赤外線LEDによって、照射角度が10～20度程度しかない物や、明るさが足りないLEDがあります。<br>
赤外線LEDをAZSENSORの方へ向けたり、距離を2～30cm程度に近づけたり遠ざけたりして確認してみて下さい。<br>
※ 近くでは反応しないけど遠ざけると反応するという場合もあります。<br>
<br><br>


<b>赤外線LEDの接続向き</b><br>
赤外線LEDは向きがあります。足が長い方をVCC、短い方をIRに接続します。<br>
向きを間違えると赤外線LEDが光りません。スマホのカメラなどで撮影すると赤外線が光っているのが見えるので、キーを押した時赤外線LEDが光っているか確認しましょう。<br>
<br><br>

<b>AZSENSORのはんだ付けミス</b><br>
AZSENSORとESP32S3の接続部分のはんだ付けと、AZSENSORに付けている抵抗のはんだ付けを確認しましょう。<br>
赤外線センサーの方ははんだ付け失敗していてもどれかが動いていれば大丈夫なのですが、抵抗は1つでも失敗しているとうまく動きません。<br>
抵抗とESP32S3を重点的に確認して下さい。<br>
<br><br>


## AZSENSER のファームウェア
<br><br>

<b>使用するUSBケーブル</b><br>
AZSENSORにファームウェアが書き込めない、キーボードとして認識しない場合、USBケーブルによってはうまく認識しない事があります。<br>
別のUSBケーブルを使ってみる、USBハブを使っていればハブを使わず直接PCに接続してみる、別のPCで試してみる、などを試してみて下さい。<br>
<br><br>

<b>ドライバがインストールできていない</b><br>
AZSENSORのファームウェア書き込み時に「対応デバイスが見つかりませんでした」と表示される場合は、ドライバが正常にインストールされていないか、ESP32S3が書き込みモードで起動できていない可能性があります。<br>
BOOTボタンを押したままRESETボタンを押すか、BOOTボタンを押したままUSB接続するとESP32S3が書き込みモードで起動します。<br>
その辺りを再度確認してみて下さい。<br>
<br><br>





