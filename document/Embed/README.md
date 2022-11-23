# 埋め込みメッセージ
![discord.js-v16.9.0](https://shields.io/badge/discord.js-v16.9.0-blue)
<br></br>


## 埋め込みメッセージの送信

## `/embed`に埋め込みメッセージを返すプログラム
```js
client.on("messageCreate", (msg)=>{
    if(msg.content==="/embed"){
        msg.reply({
            embeds:[
                {
                    title:"題名",
                    description:"説明文"
                }
            ]
        })
    }
})
```
![](https://github.com/kelp-of-truth/Discord-Document/blob/1b3409871b2606a31eb1af55aa805b9ef98efe4d/document/src/video/embed_1.mp4)
