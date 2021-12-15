## robosys

## 用意するもの

・ラズパイ
・LEDライト
・ブレッドボード
・抵抗　(200Ω)
・ジャンパ線
・LANケーブル

## 方法

・インストール

'''sh
$ git clone https://github.com/KoukiNegi/robosys.git
$ cd robosys
$ make

・権限を与える

'''sh
$ sudo insmod myled.ko
$ sudo chmod 666 /dev/myled0

・アンインストール

'''sh
$ sudo rmmod myled
$ make ckean

・LED点灯

'''sh
$ echo 1 > /dev/myled0

・LED消灯

'''sh
$ echo 0 > /dev/myled0


## ライセンス
https://github.com/KoukiNegi/robosys/blob/main/COPYING
