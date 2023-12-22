# ros 2 mypkg
このリポジトリはros 2の勉強のため製作しました。

## topicについて
topicはデータをやり取りするもので、データを送信するものとデータを受信、表示するものがある。

## talker.py
Int16のデータを送信している。
ビルドをして実行し、ros2 topic echoで確認すると、1から順にデータを送信している。

## listener.py
Int16のデータを受信、表示している。

## talker.pyとlistener.pyの実行例
別のターミナルを立ち上げ、片方にros2 run mypkg talker、もう片方にros2 run mypkg listenerを入力する。すると、ros2 run mypkg listenerを入力した側に、以下のように出力される。
```
[INFO] [1703251791.477646568] [listener]: Listen: 0
[INFO] [1703251791.937011011] [listener]: Listen: 1
[INFO] [1703251792.467410111] [listener]: Listen: 2
[INFO] [1703251792.958938305] [listener]: Listen: 3
[INFO] [1703251793.465086073] [listener]: Listen: 4
[INFO] [1703251793.957176916] [listener]: Listen: 5

```

## 必要なソフトウェア
* Python
  * テスト済み: 3.7〜3.10

## テスト環境
* Ubuntu 22.04.3 LTS

## 著作権, ライセンス
* このソフトウェアパッケージは，3条項BSDライ>センスの下，再頒布および使用が許可されます．
* このパッケージのコードの一部は，下記のスラ>イド（CC-BY-SA 4.0 by Ryuichi Ueda）のものを>，本人の許可を得て自身の著作としたものです．
     * [ryuichiueda/my_slides/robosys_2022/lesson9](https://github.com/ryuichiueda/my_slides/blob/master/robosys_2022/lesson9.md)
* © 2024 Yamato Osada
<.md" 57L, 1658B
