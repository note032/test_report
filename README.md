# robosys_2019

このプログラムはLEDを点灯、消灯、点滅させるプログラムである。
このプログラムを実行するために必要なもの
・LED
・抵抗
・raspberrypi 3
・ジャンプワイヤー
・c言語

LEDを点灯させるためにデバイスドライバを作成する.参考にしたページは次のリンクを参照.
https://ryuichiueda.github.io/robosys2019/lesson7.html

コマンドの手順は以下のとおりである.
make  
sudo insmod myled.ko  
sudo chmod 666 /dev/myled0  
echo 0 /dev/myled0 で消灯  
echo 1 /dev/myled0 で点灯  
echo 2 /dev/myled0 で点滅する  

これの実行結果はyoutubeにアップロードされている.
youtube（デモ動画）のリンクはこちら
https://www.youtube.com/watch?v=SmiLRucGogU

