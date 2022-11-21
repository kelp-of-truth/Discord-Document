# スラッシュコマンド
<br></br>


![](https://github.com/kelp-of-truth/Discord-Document/blob/kelp-of-truth-discord.js-document/document/src/img/slashCommand.jpg?raw=true)
＊スラッシュコマンド
<br></br>


## スラッシュコマンドの読み込み
```js
const data=[
    {
        "name":"hello",
        "description":"こんにちは"
    }
];

client.on("ready", ()=>{
    client.application.commands.set(data);
});



```

- `name`： コマンドの名前
- `descroption`：コマンドの説明文
<br>

**注意：`description`はアルファベットの大文字が使えない**
<br></br>

## コマンドの項目の追加

コマンドの項目を追加する場合は、JSONを次のように書き、それを読み込む。


```json
[
    {
        "name":"buy",
        "description":"アイテムを購入します",
        "options":[
            {
                "name":"item_name",
                "type":3,
                "description":"購入するアイテムの名前",
                "required":true,
                "choices":[
                    {
                        // りんご
                        "name":"apple",
                        "value":"apple"
                    },
                    {
                        // ぶどう
                        "name":"grapes",
                        "value":"grapes"
                    }
                ]
            }
        ]
    }
]
```
　
[data.json](https://github.com/kelp-of-truth/Discord-Document/blob/a47d2317bd3b70d071fc1af5934383d5cb9fcefd/document/SlashCommand/data.json)

**options**<br>
- ``name``：オプションの名前
- ``description``：オプションの説明（これも大文字の使用ができない）
- `type`：オプションのタイプ
- `required`：オプションの入力が必須かどうか　`true`で、必須・`false`で任意
- `choices`：入力の候補
    - `name`：候補名
    - `value`：候補の取得時の値

<br>

## `type`の数値ごとの説明
|名前|数値|説明|
|:-|:-|:-|
|SUB_COMMAND|1|サブコマンド|
|SUB_COMMAND_GROUP|2|サブコマンドグループ|
|STRING|3|文字列|
|INTEGER|4|-2<sup>53</sup>から2<sup>53</sup>までの任意の整数|
|BOOLEAN|5|`ture` または `false`|
|USER|6|サーバーにいるユーザーが候補として表示される<br>**`choices`を書く必要は無い**|
|CHANNEL|7|サーバーにあるチャンネルが候補として表示される<br>**`choices`を書く必要は無い**|
|ROLE|8|サーバーにあるロールが候補として表示される<br>**`choices`を書く必要は無い**|
|CHANNEL|9|サーバーにあるロールとサーバーにいるユーザーが候補として表示される<br>**`choices`を書く必要は無い**|
|NUMBER|10|-2<sup>53</sup>から2<sup>53</sup>までの任意の数（`double型`）|
|ATTACHMENT|11|アタッチメント|

---


### 参考にしたサイト
- [Discord Developer Document](https://discord.com/developers/docs/)
