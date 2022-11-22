# 絵文字
![](https://shields.io/badge/discord.js-v16.9.0-blue "discord.js-v16.9.0")
<br></br>


## 既存の絵文字の送信

### `/emoji`と送信されたときに`🔰`を返すプログラム
```js
client.on("messageCreate", (msg)=>{
  if(msg.content==="/emoji"){
    msg.reply(":beginner:");
  };
})
```
既存の絵文字を送信する場合は、絵文字の名前を`:`で囲う
<br></br>

## カスタム絵文字の送信
### `/emoji`と送信されたとき`custom_emoji`という名前のカスタム絵文字を返すプログラム
```js
client.on("messageCreate", (msg)=>{
  if(msg.content==="/emoji"){
    const emoji_id=msg.guild.emojis.cache.find((emoji)=>emoji.name==="custom_emoji");
    msg.reply(`:custom_emoji:emoji_id`);
  };
})
```
カスタム絵文字を送信する場合は、絵文字の名前を`:`で囲い、その後ろにidを入れる
 
**注意：アニメーション絵文字はNitoroを購入していないと使えません**



---
### 関連リンク


---
### 参考リンク
- [DISCORD.JS.ORG](https://discord.js.org/)
