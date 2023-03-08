# Dharma とは

カバディは日本国内ではまだまだ発展途上の状態にある．
有志の努力によって公式戦がLIVE配信される中，スコアラおよびスタッツデータの集計といったソリューションは未だ登場していない．
Dharmaは，試合中にレイド結果を記録することで得点表とスタッツ集計を同時に実現する．

## 開発環境の構築

マシンのOSは不問だが，仮想環境の構築にDockerが必要となっている．
また，IDEは"Dev Container"を使用したいのでVS Codeに限定する．

実際の工程は以下に従う．

1. devcontainer.jsonを開く
1. コマンドパレット(F1)で「reopen in container」
1. git 権限

`sudo chown -R qq.qq .git`

1. ビルド

`yarn tauri build`

1. 立ち上げ

`yarn tauri dev`

## データの取り扱い

開発用のsqlite をそのままリポジトリに上げているが、これはいつかやめる。
