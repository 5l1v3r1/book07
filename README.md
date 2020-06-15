# 進捗大陸07

## セットアップ方法

```
git submodule update --init --recursive
make
```

## その他

### `.satysfi`について

まず、`.satysfi`は`SATySFi`のドキュメントルートである([ドキュメント](https://github.com/gfngfn/SATySFi/blob/master/memo-ja-how-to-use.md))。ライブラリやフォントはこのディレクトリに配置する。

このリポジトリでは`.satysfi`にライブラリやフォントをプリセットで用意しておき、dockerで`$HOME`にvolume mountすることで、コンテナ内でライブラリとして用いられるようにしている(hashの更新など手作業確実に忘れるので自動化したい)。

### フォントについて

上記の`.satysfi`以下に事前に準備しておく必要がある。`make`を走らせれば勝手にインストールされるので気にしなくて良い。
