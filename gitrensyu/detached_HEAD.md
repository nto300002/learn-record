## detached HEADとは「ブランチがない状態」です。もう少し詳しく言うと「HEAD がコミットIDを直接指し示している状態」です。
https://www.r-staffing.co.jp/engineer/entry/20201225_1

## これを抜け出すには
また、この状態で行ったコミットを破棄することもできます。
ブランチに戻ることで、どのブランチにも影響を与えずにコミットを破棄することができます。

新しいブランチを作成して自分のコミットを保持したい場合は、次のようにします。
switch コマンドで -c を指定することで、(今からでも) ブランチを作成することができます。例

  git switch -c <新しいブランチ名> とします。

あるいは、この操作を元に戻すには

  git switch - を実行すると、この操作を取り消すことができます。

