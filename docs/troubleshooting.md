# トラブルシューティング

## ビルド出来ない！
・v2.0.0以上ではSDK 3.8.1以上が必要です。

## 「SDK Callback」エラーが出る！
`Udon/Editor/VRCCameraBuildChecker.cs`を削除してください。

## アバターの断面図が見える！
・v2.0.0以上にアップデートしてください。

## アバターの一部パーツが消える！
・アバターのBoundsが統一されているかご確認ください。Modular Avatarの[Mesh Settings](https://modular-avatar.nadena.dev/ja/docs/reference/mesh-settings)などの一括設定ツールを使うと便利です。
