# training-scala
[VSCode Remote Development](https://code.visualstudio.com/docs/remote/remote-overview) 機能でScalaの開発環境を構築するためのレポジトリです。

## use-case
- `.devcontainer`をあなたのプロジェクトにコピーして、プロジェクト用の開発環境をチームに共有したりできる
- ハンズオンで環境構築がめんどくさい時に使えるのかも

## usage
1. vscodeでRemote Development機能を使ってコンテナ作成

https://user-images.githubusercontent.com/24284232/137709870-3df7e378-3fe2-4423-b808-7c4db049a209.mov

2. Giter8 templateを使って新しいsbtプロジェクトを作成

[コマンド例](https://github.com/shaw-papadino/training-scala#gitter8-template-example)

3. 作成されたプロジェクトを開く

https://user-images.githubusercontent.com/24284232/137710465-214d0a36-3016-4c82-abee-ed8aad2f20e6.mov

4. 上記で作成したプロジェクトにmetalsを適用させてIDEのような御加護を得る

右下の`Import build`をクリックする

<img width='640' src="https://user-images.githubusercontent.com/24284232/137710809-35dd9ebe-b0d8-4a73-84ec-a64f9960dbee.png" />

https://user-images.githubusercontent.com/24284232/137710739-75abfc2d-c757-4f31-947e-83f3e853674c.mov

## requirement

- [Remote - Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)

## Gitter8 template example

[scala-seed](https://github.com/scala/scala-seed.g8)
```
sbt new scala/scala-seed.g8
```

[akka-quickstart-scala](https://github.com/akka/akka-quickstart-scala.g8)
```
sbt -Dsbt.version=1.3.6 new akka/akka-quickstart-scala.g8
```
