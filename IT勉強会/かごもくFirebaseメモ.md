# かごもくFirebaseメモ


## Realtime Database, Firestore

## Auth

- 電話認証は色々ルールがあるので、ドキュメントを読んでルールを確認する　

## Firestore

- セキュリティ対策をちゃんとしないとまずい
- サブコレクションを使うのはあんまり良くない
- セキュリティルールを書けば弾けるが、フロントエンドだとうまく弾けない
- アクセス制御を考えないと本人しか見えてはいけない情報が見えたりする
- ここのテストがめんどくさい
- 参照型か、閲覧できるリストを作る
- 予約の状態をサブコレクションでもたせる方がよさそう
- 現在の状態は別途コレクションで持っている方が良さそう
- セキュリティルールのチェック方法はドキュメントに書いてあるので、そっちを見たほうが良さそう

## Functions


- ローカルエミュレーター
- AuthやFirestoreは本番のものを使ってしまう
- Firestoreへの書き込みをFunctionsを噛ませて行う
- Firestroeを秘匿して、Functionsから動かす　

