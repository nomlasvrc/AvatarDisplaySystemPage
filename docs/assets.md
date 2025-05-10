# アセット解説

## 本体
#### AvatarDisplaySystem.prefab
プレイヤー自身を表示するのに特化したprefabです。動作が安定しており、処理が比較的軽いです。

#### AvatarDisplaySystem Local Variant.prefab
表示位置同期機能を削除したバリアントです。ネットワーク負荷を軽くすることが出来ます。

#### AvatarDisplaySystem Remote Player.prefab
インスタンス内の他のプレイヤーも表示できるprefabです。メニューから表示するプレイヤーを変更することが出来ます。このprefabの特性上、他prefabに比べて若干重い処理を行います。パフォーマンスを重視する場合は他のprefabをご利用ください。  
**注：** このprefabは現在開発中のβ版です。指定していないプレイヤーが映り込むなど、一部描画に問題があります。

### 各prefabの特徴
|  | AvatarDisplaySystem | AvatarDisplaySystem Local Variant | AvatarDisplaySystem Remote Player |
| - | - | - | - |
| 表示プレイヤー | 自分のみ | 自分のみ | インスタンス内全員 |
| 表示位置同期 | 〇 | × | 〇 |
| 表示プレイヤー同期 | × | × | 〇 |
| 描画安定度 | 〇 | 〇 | △ |

## メニュー
スケールやミラーモードなどを変更できます。本体prefabの下にあります。  
このprefabは完全に独立しているため、削除したり、ヒエラルキー上で移動したりしても動きます。

## 「Unpack prefab」について
このアセットの全てのプレハブ・プレハブ バリアントにおいて、Unpack prefabはバージョンアップ時にバグの原因となるため**非推奨**です。