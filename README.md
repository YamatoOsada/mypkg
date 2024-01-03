# mypkg
このリポジトリはロボットシステム学で使用しているリポジトリです。
このリポジトリはros 2のパッケージです。
[![test](https://github.com/YamatoOsada/robosys2023/actions/workflows/test.yml/badge.svg)](https://github.com/YamatoOsada/robosys2023/actions/workflows/test.yml)

## topicについて
* topicはノード間でやり取りするデータのことである。
* 送信にはパブリッシャ、受信や読み取りにはサブスクライバを使用する。
* 1対1の通信だけでなく、1対10のような多数がデータを受け取ることができる。

## talker.py
### 機能
* Int16のデータを送信している。
* 整数を0から順番にカウントしている。

## listener.py
### 機能
* Int16のデータを受信、表示している。
* カウントした数字のデータを取得して、標準出力で出力している。

## talker.pyとlistener.pyの実行例
別のターミナルを立ち上げ、下記の実行コマンドを入力する。

### talker側
```
$ ros2 run mypkg talker
```

### listener側
```
$ ros2 run mypkg listener
```

すると、listener側に以下のように出力される。

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
* ROS 2 humble

## テスト環境
* Ubuntu 22.04.3 LTS
* ROS 2

## 著作権, ライセンス
* このソフトウェアパッケージは，3条項BSDライセンスの下，再頒布および使用が許可されます．
* このパッケージのコードは，下記のスライド（CC-BY-SA 4.0 by Ryuichi Ueda）のものを，本人の許可を得て自身の著作としたものです．
     * [ryuichiueda/my_slides/robosys_2022/lesson8](https://github.com/ryuichiueda/my_slides/blob/master/robosys_2022/lesson8.md)
     * [ryuichiueda/my_slides/robosys_2022/lesson9](https://github.com/ryuichiueda/my_slides/blob/master/robosys_2022/lesson9.md)
     * [ryuichiueda/my_slides/robosys_2022/lesson10](https://github.com/ryuichiueda/my_slides/blob/master/robosys_2022/lesson10.md)
     * [ryuichiueda/my_slides/robosys_2022/lesson11](https://github.com/ryuichiueda/my_slides/blob/master/robosys_2022/lesson11.md)
* © 2023 Yamato Osada
