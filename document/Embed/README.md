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

<video style="width: 50vw;" controls playsinline muted="true" src="https://github.com/kelp-of-truth/Discord-Document/blob/kelp-of-truth-discord.js-document/document/src/video/embed_1.mp4?raw=true" >
ビデオを読み込めませんでした
</video>
