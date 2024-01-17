# TheUnusualSkyBlock-Datapacks
配布マップ「TheUnusualSkyBlock」のライブラリデータパックの管理リポジトリ

> [!IMPORTANT]  
> このブランチはMinecraft 1.19.4で開発するためのライブラリ環境です。

## 導入方法
git bash もしくはコマンドプロンプトで以下を実行する。

```bash
cd <world>
```
ここで、`<world>`は製作ワールドへのパスを指す。
```bash
git clone -b 1-19-4 --recurse-submodules https://github.com/TUSB/TheUnusualSkyBlock-Datapacks.git datapacks
```
このリポジトリを`datapacks`ディレクトリへクローンする。  
`--recurse-submodules`のオプションは、サブモジュールも一緒にクローンすることを示している。  
`-b 1-19-4`のオプションは、このブランチをクローンすることを示している。

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
メインデータパックには2つのでライブラリデータパックが組み込まれている。

* [ChenCMD/MCCMD-ScoreDamage](https://github.com/ChenCMD/MCCMD-ScoreDamage)  
  tag: [`3.3`](https://github.com/ChenCMD/MCCMD-ScoreDamage/releases/tag/3.3)  
  commit: [`91ff473`](https://github.com/ChenCMD/MCCMD-ScoreDamage/tree/3.3)
* [Irohamaru/SmartMotion](https://github.com/Irohamaru/SmartMotion)  
  tag:  
  commit: [`78a7c70`](https://github.com/Irohamaru/SmartMotion/tree/78a7c70401a6a4a76bacc1a253aaaec15d045a16)

## 1-19-4へのお知らせ
1-19-4では未配布のライブラリデータパックが4つ必要である。

* Popup  
  制作関連カテゴリ → 制作フォーラム → 例のダメージ表示のもの  
  フォーラム内からダウンロードして配置する。  
  リソースパックの導入も必要。
* MineChachat  
  制作関連カテゴリ → 制作フォーラム → 例の吹き出し表示のもの  
  フォーラム内からダウンロードして配置する。
* MineChachatHelper  
  MineChachatと同様のフォーラム内からダウンロードして配置する。
* zPatch  
  [TUSBドライブ](https://drive.google.com/drive/folders/1d4JiXgHc7Q3TGVU5mp3r5sP5WDEnPKz6)からダウンロードして配置する。  
  TUSBドライブへは製作者のみアクセス可能
