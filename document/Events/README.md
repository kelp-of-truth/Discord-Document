# discord.jsのイベント一覧
<br></br>


## client.onの書き方
```javascript
client.on("イベント名", (変数)=>{
  //処理
})
```
<br><br>


## イベント一覧
|イベント名|発火条件|
|:-|:-|
|channelCreate|新しくチャンネルが作成されたとき|
|channelDelete|チャンネルが削除されたとき|
|guildBanAdd|BANしたとき|
|guildBanRemove|BANを解除したとき|
|guildUnavailable|サーバーが削除などされて、利用できなくなったとき|
|guildDelete|BotがサーバーからBAN、またはキックされたとき|
|emojiCreate|新しく絵文字が作成されたとき|
|emojiDelete|絵文字が削除されたとき|
|emojiUpdate|絵文字が更新されたとき|
|guildIntegrationsUpdate|サーバーが統合（？）されたとき|
|guildMemberRemove|サーバーからメンバーが退出したとき|
|guildMemberUpdate|ロールの付与、削除、ニックネームが変更されるなどして、メンバーの情報が更新されたとき|
|guildMemberAvailable|メンバーが利用可能（？）になったとき|
|roleCreate|新しくロールが作成されたとき|
|roleDelete|ロールが削除されたとき|
|roleUpdate|ロールが更新されたとき|
|stickerCreate|新しくスタンプが作成されたとき|
|stickerDelete|スタンプが削除されたとき|
|stickerUpdate|スタンプが更新されたとき|
|guildUpdate|サーバーが更新されたとき（サーバー名の変更、など）|
|interactionCreate|インタラクションしたとき（メンバーがコマンドを送信したときや、コンポネートにインタラクションしたとき、など）|
|inviteCreate|新しく招待コードが作成されたとき|
|inviteDelete|招待コードが削除されたとき|
|messageCreate|メッセージが送信されたとき|
|messageDelete|メッセージが削除されたとき|
|messageDeleteBulk|メッセージが一括削除されたとき|
|messageReactionAdd|メッセージがリアクションされたとき|
|messageReactionRemove|メッセージからリアクションが取り消されたとき|
|messageReactionRemoveAll|メッセージからすべてのリアクションが取り消されたとき|
|messageReactinRemoveEmoji|メッセージから絵文字リアクションが削除されたとき|
|presenceUpdate|ユーザーのオンラインステータスが変更されたとき|
|stageInstaceCreate|新しくステージインスタンスが作成されたとき|
|stageInstanceDelete|ステージインスタンスが削除されたとき|
|stageInstanceUpdate|ステージインスタンスが更新されたとき|
|threadCreate|新しくスレッドが作成されたとき|
|threadDelete|スレッドが削除されたとき|
|threadListSync|メンバーがスレッドを含むチャンネルにアクセスしたとき|
|threadMembersUpdate|メンバーがスレッドに追加、削除されたときに|
|threadMemberUpdate|ユーザーが更新されたとき|
|typingStart|「入力...」になったとき|
|userUpdate|ユーザーの情報が更新されたとき（サーバープロフィールではない）|
|voiceStateUpdate|ユーザーがミュートのON / OFFを切り替えたときや、ボイスチャンネルに参加したとき|
|debug|**情報なし**|
|webhookUpdate|WebHookが更新されたとき|
|warm|警告（？）|
|channelPingsUpdate|ピンどめが追加、削除されたとき|
|channelUpdate|チャンネルが更新されたとき（チャンネル名が変更されたときなど）|
|guildUpdate|Botがサーバーに追加されたとき|
|guildMemberAdd|サーバーに新しくメンバーが参加したとき|
|guildMemberChunk|メンバーのチャンクを受信したとき|
|messageUpdate|メッセージが編集されたとき|


<br></br>

---
参考リンク
- [DISCORD.JS.ORG](https://discord.js.org/#/)

