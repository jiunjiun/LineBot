# LineBot
A simple Sinatra(Ruby) LineBot Template and tutorial how to setup on Heroku for Line Bot API

圖文說明文章：[http://jiunjiun.logdown.com/posts/2016/10/06/linebot-with-sinatra](http://jiunjiun.logdown.com/posts/2016/10/06/linebot-with-sinatra)

Installation and Usage
=============

### 1. 註冊一個Line Messaging API

[https://business.line.me/zh-hant/services/bot](https://business.line.me/zh-hant/services/bot)

### 2. Deploy 到 Heroku

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

\* 記住你的 Heroku ID

### 3. 設定 Line Bot 參數

設定完基本資訊，可以到 Bot Developers 找到

- Channel Secret
- Channel Access Token

並且設定到 Heroku Config

```
heroku config:set LINE_CHANNEL_SECRET={YOUR_Channel_Secret}
heroku config:set LINE_CHANNEL_TOKEN={YOUR_Channel_Access_Token}
```

接著在 `Edit` 頁面，去修改你的 `Webhook URL`

- `Callback URL`: https://{YOUR_HEROKU_SERVER_ID}.herokuapp.com/callback

完成...

-

API 參考：
[https://devdocs.line.me/en/#imagemap-message](https://devdocs.line.me/en/#imagemap-message)

line-bot-sdk-ruby：
[https://github.com/line/line-bot-sdk-ruby](https://github.com/line/line-bot-sdk-ruby)

Inspired By
=============

- [LineBotTemplate](https://github.com/kkdai/LineBotTemplate)


License
---------------

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

