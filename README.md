# TheUnusualSkyBlock-Datapacks
配布マップ「TheUnusualSkyBlock」のライブラリデータパックの管理リポジトリ

## 導入方法
git bash もしくはコマンドプロンプトで以下を実行する。

```bash
cd <world>
```
ここで、`<world>`は製作ワールドへのパスを指す。
```bash
git clone --recurse-submodules https://github.com/TUSB/TheUnusualSkyBlock-Datapacks.git datapacks
```
このリポジトリを`datapacks`ディレクトリへクローンする。  
`--recurse-submodules`のオプションは、サブモジュールも一緒にクローンすることを示している。

すでにワールドに`datapacks`ディレクトリが存在するときはこのコマンドは失敗する。  
そのときは`datapacks`ディレクトリを削除してから再実行をする。

> [!WARNING]  
> VSCodeのコマンドでgitクローンをすることができるが、  
> ディレクトリ名に決まりがあること、サブモジュールの導入が必要なことから  
> git bash もしくはコマンドプロンプトでの実行を推奨する。


## 運用方法
mainブランチは空とする。  
例：製作に使用するMinecraftバージョンが1.19.4ならば`1-19-4`ブランチをmainブランチからチェックアウトする。  

ライブラリデータパックはgitサブモジュール機能を使ってこのリポジトリに導入する。  
メインデータパックはこのリポジトリで管理されることは無いが、同じ`datapacks`の中へクローンする。

## 組み込みライブラリのコミットハッシュ
メインデータパックには1つのライブラリデータパックが組み込まれている。

* [Irohamaru/SmartMotion](https://github.com/Irohamaru/SmartMotion)  
  tag:  
  commit: [`template`](https://github.com/Irohamaru/SmartMotion/tree/)
