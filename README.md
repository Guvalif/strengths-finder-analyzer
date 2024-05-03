Let's Analyze a Team Themes to Unleash the Potential!
===============================================================================

## What's This?

[『チーム理解のためのストレングスファインダー®可視化手法』](https://creators-note.chatwork.com/entry/2023/12/07/110000)で紹介した内容を、Python のライブラリとして公開したものです。


## How to Use

`sample_table.json` の要領で、チームメンバーの **名前** と **資質の順位づけ** の組を記述します。

ライブラリとして用いる場合は、事前にデータをメモリ内に展開した上で、以下の公開メソッドを用います (詳細は docstring に記載)：

- `histogram` : 強み，および弱みのヒストグラムを計算する
- `distance_gen` : 各チームメンバー間の、資質の順位づけに基づく距離を計算する
- `specific_gen` : 各チームメンバーの、固有な強みを計算する

※ 本実装では、ビジュアライゼーションは利用者側で設計することを想定しています (e.g. [matplotlib](https://matplotlib.org/))

モジュールとして実行する場合は、以下のコマンドラインが一例です：

```sh
cat sample_table.json | python lib.py
```


## Copyright (C) 2024,

- [TAKASE Kazuyuki](https://github.com/Guvalif)

This software is released under [the MIT License](http://opensource.org/licenses/mit-license.php).
