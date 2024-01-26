# robosys2023
ロボットシステム学の課題2
* ![test](https://github.com/numashuto/mypkg/actions/workflows/test.yml/badge.svg)

このレポジトリはロボットシステム学第二回課題提出のため作成、使用したものです。

## ノード
 * talker
    * 0.5秒ごとに0から1ずつカウント。
 * listener
    * talkerからメッセージを受け取り、画面に数字として表示させる。

##使用方法
### talker.py

以下のコマンドを実行する。

```
$ ros2 run mypkg talker
```

実行結果は表示されていない

### listener.py

talkerとは別のターミナルを使用し以下のコマンドを実行する。
```
$ ros2 run mypkg listener
```
以下のように実行結果が表示される。
```
[INFO] [1706238027.815740169] [listener]: Listen: 91
[INFO] [1706238028.315194637] [listener]: Listen: 92
[INFO] [1706238028.818692847] [listener]: Listen: 93
[INFO] [1706238029.315408482] [listener]: Listen: 94
```

### talk_listen.launch.py
以下のコマンドを実行する。
```
$ ros2 launch mypkg talk_listen.launch.py

```
以下のように実行結果が表示される。
```
[listener-2] [INFO] [1706238139.984527399] [listener]: Listen: 0
[listener-2] [INFO] [1706238140.455697536] [listener]: Listen: 1
[listener-2] [INFO] [1706238140.995620690] [listener]: Listen: 2
[listener-2] [INFO] [1706238141.453178863] [listener]: Listen: 3
[listener-2] [INFO] [1706238141.955483744] [listener]: Listen: 4
[listener-2] [INFO] [1706238142.455281722] [listener]: Listen: 5
[listener-2] [INFO] [1706238142.953555368] [listener]: Listen: 6
[listener-2] [INFO] [1706238143.455437571] [listener]: Listen: 7
[listener-2] [INFO] [1706238143.953839029] [listener]: Listen: 8
[listener-2] [INFO] [1706238144.454314172] [listener]: Listen: 9
[listener-2] [INFO] [1706238144.954094599] [listener]: Listen: 10
```

## 開発環境

 * Python
  * テスト済み: 3.10
 * ROS2

## テスト環境

  * Ubuntu22.04 LTS

## ライセンス
* このソフトウェアパッケージは，3条項BSDライセンスの下，再頒布および使用が許可されます．
* このパッケージのコードは，下記のリポジトリ（CC-BY-SA 4.0 by Ryuichi Ueda）のものを，本人の許可を得て自身の著作としたものです．
* https://github.com/ryuichiueda/robosys2023/tree/main
* © 2023 Shuto Numata
