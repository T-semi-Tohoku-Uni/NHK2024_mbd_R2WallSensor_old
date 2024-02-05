# NHK2024_R2CANIDList
R2 (Robot2) 用の基幹CANバスのCANIDをリストアップするところ
ヘッダファイルをインクルードしていい感じに使ってね

## submodule利用推奨
作成したローカルリポジトリで以下のコマンドを実行
```
git remote R2CANIDList git@github.com:T-semi-Tohoku-Uni/NHK2024_R2CANIDList.git
git subtree add --prefix=<任意のディレクトリ> --squash R2CANIDList main
git commit -m "add subtree R2CANIDList"
```

CANIDを変更or追記したら
```
git subtree push --prefix=<上記でsubtreeを置いたところのパス> R2CANIDList main
```

リモート (github上) の変更を取り込みたいときは
```
git subtree pull --prefix=<上記でsubtreeを置いたところのパス> R2CANIDList main
```

以下 例 ([NHK2024_mbd_R2CylinderDriver1](https://github.com/T-semi-Tohoku-Uni/NHK2024_mbd_R2CylinderDriver1) の場合)
```
git remote R2CANIDList git@github.com:T-semi-Tohoku-Uni/NHK2024_R2CANIDList.git
git subtree add --Core/R2CANIDList --squash R2CANIDList main
git commit -m "add subtree R2CANIDList"
```
