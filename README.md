# TheUnusualSkyBlock-Datapacks
配布マップ「TheUnusualSkyBlock」のメインデータパックとライブラリデータパックの管理リポジトリ

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

> [!NOTE]  
> VSCodeのコマンドでgitクローンをした場合、ディレクトリ名が`TheUnusualSkyBlock-Datapacks`になる。  
> このリポジトリの中身はデータパックなので、手動で`datapacks`へと名前変更を行うことでワールドへ導入できる。


## 運用方法
mainブランチは空とする。  
例：製作に使用するMinecraftバージョンが1.19.4ならば`1-19-4`ブランチをmainブランチからチェックアウトする。  

メインデータパックとライブラリデータパックはgitサブモジュール機能を使ってこのリポジトリに導入する。