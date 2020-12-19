# robokadai1
## 作成者
嶋田　雅
## 内容
https://github.com/ryuichiueda/robosys_device_drivers/blob/master/myled.c 左のURLを改変しデバイスドライバを作成した。
## 必要なもの
ラズベリーパイ　４　モデルＢ　４ＧＢ　ＲＡＭ、ブレッドボードSAD-101、ワイヤージャンパ（オスオス）ｘ２（オスメス）ｘ３、LEDｘ２
## 実装機能 
echo m > /dev/myled0　右点滅ｘ３、左点滅ｘ３
echo y > /dev/myled0　右左の順番で交互に点滅ｘ３、両方点滅ｘ２、左右の順番で交互に点滅ｘ３
## 動作方法
make
sudo insmod myled.ko
sudo chmod 666 /dev/myled0
echo m > /dev/myled0
echo y > /dev/myled0
## 協力者
加藤舞子、小村岳都、西廣巧
## YouTube　URL
https://youtu.be/a5FOhhGdUm8

## ライセンス
GNU General Public License v3.0
