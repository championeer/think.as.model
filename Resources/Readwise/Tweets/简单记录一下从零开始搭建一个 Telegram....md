# 简单记录一下从零开始搭建一个 Telegram...

![rw-book-cover](https://pbs.twimg.com/profile_images/1537801286459961350/Y7xOUGr6.jpg)

## Metadata
- Author: [[@tufook on Twitter]]
- Full Title: 简单记录一下从零开始搭建一个 Telegram...
- Category: #tweets
- URL: https://twitter.com/tufook/status/1632099875306504192

## Highlights
- 简单记录一下从零开始搭建一个 Telegram ChatGPT bot 的过程，希望对有需要的朋友有帮助。 ([View Tweet](https://twitter.com/tufook/status/1632099875306504192))
- ChatGPT 的网页版本已经把中国大陆的 IP 以及各大机房 IP 都屏蔽了，包括我日常使用的代理服务器。因此我基本无法使用官方版本的 ChatGPT。而自行搭建的 Telegram bot 可以规避这个问题，并且它是你私有的，比如历史记录可以一直保留。 ([View Tweet](https://twitter.com/tufook/status/1632099877168758784))
- 我的流程分为七步：
  1. 在甲骨文免费服务器上搭建 v2ray 节点 
  2. 使用 Cloudflare 的 WARP 代理以伪装成原生 IP
  3. 注册 ChatGPT 账号使用接码平台接受短信验证码
  4. 获取 ChatGPT API key
  5. 新建一个 Telegram bot，获取 bot token
  6. 在另一台服务器上运行 bot 代码，完成搭建 ([View Tweet](https://twitter.com/tufook/status/1632099879005863936))
- 1. 甲骨文的免费服务器每个账号有两台，虽然性能一般，但运行 v2ray 和 bot 绰绰有余，而且贵在终身免费。
  我参考的教程是 https://t.co/6DvsWOUs8G
  这一步结束后，你得到一个 v2ray 节点。 ([View Tweet](https://twitter.com/tufook/status/1632099881446969344))
- 2. 光有节点还不够，因为 OpenAI 知道你是节点。Cloudflare 的 WARP 是个非常神奇的东西，它可以帮我的节点伪装成原生的 IP。如果你想解锁 Netflix 也适用。
  我参考的教程是 https://t.co/LdKxoh9w3M
  这一步结束后，你就可以正常访问 ChatGPT 了。 ([View Tweet](https://twitter.com/tufook/status/1632099883468591104))
- 3. 注册一个 ChatGPT 账号，然后验证手机号。我用的接码平台是 sms-activate https://t.co/dTNKV3uymZ （含 affiliate）
  它似乎涨价了，并且支付宝付款最低 1 美元。我选了英国的手机号，验证成功。 ([View Tweet](https://twitter.com/tufook/status/1632099885850984448))
- 4. 注册 ChatGPT 的账号后，可以生成一个 API key，因为只会给你看一次，所以务必保存起来。
  5. 新建 Telegram bot 的流程很简单，搜索 botfather 这个官方 bot 就能按照指引完成。 ([View Tweet](https://twitter.com/tufook/status/1632099888241467395))
- 6. 目前 Telegram bot + ChatGPT 的教程还不多，我找到的是这个 https://t.co/i8WZWPPAQz 
  这个教程的问题是对新手很不友好，在使用这个仓库的代码之前需要：
  a. 在服务器上装好 Docker 和 Docker compose
  b. 将仓库代码下载到服务器
  但不得不说，最后搭建出来的 bot 很好用。 ([View Tweet](https://twitter.com/tufook/status/1632099890334691328))
- 感谢互联网。至少还有互联网能让我们不是孤立无援的。 ([View Tweet](https://twitter.com/tufook/status/1632099892486348800))
# 简单记录一下从零开始搭建一个 Telegram...

![rw-book-cover](https://pbs.twimg.com/profile_images/1537801286459961350/Y7xOUGr6.jpg)

## Metadata
- Author: [[@tufook on Twitter]]
- Full Title: 简单记录一下从零开始搭建一个 Telegram...
- Category: #tweets
- URL: https://twitter.com/tufook/status/1632099875306504192

## Highlights
- 简单记录一下从零开始搭建一个 Telegram ChatGPT bot 的过程，希望对有需要的朋友有帮助。 ([View Tweet](https://twitter.com/tufook/status/1632099875306504192))
- ChatGPT 的网页版本已经把中国大陆的 IP 以及各大机房 IP 都屏蔽了，包括我日常使用的代理服务器。因此我基本无法使用官方版本的 ChatGPT。而自行搭建的 Telegram bot 可以规避这个问题，并且它是你私有的，比如历史记录可以一直保留。 ([View Tweet](https://twitter.com/tufook/status/1632099877168758784))
- 我的流程分为七步：
  1. 在甲骨文免费服务器上搭建 v2ray 节点 
  2. 使用 Cloudflare 的 WARP 代理以伪装成原生 IP
  3. 注册 ChatGPT 账号使用接码平台接受短信验证码
  4. 获取 ChatGPT API key
  5. 新建一个 Telegram bot，获取 bot token
  6. 在另一台服务器上运行 bot 代码，完成搭建 ([View Tweet](https://twitter.com/tufook/status/1632099879005863936))
- 1. 甲骨文的免费服务器每个账号有两台，虽然性能一般，但运行 v2ray 和 bot 绰绰有余，而且贵在终身免费。
  我参考的教程是 https://t.co/6DvsWOUs8G
  这一步结束后，你得到一个 v2ray 节点。 ([View Tweet](https://twitter.com/tufook/status/1632099881446969344))
- 2. 光有节点还不够，因为 OpenAI 知道你是节点。Cloudflare 的 WARP 是个非常神奇的东西，它可以帮我的节点伪装成原生的 IP。如果你想解锁 Netflix 也适用。
  我参考的教程是 https://t.co/LdKxoh9w3M
  这一步结束后，你就可以正常访问 ChatGPT 了。 ([View Tweet](https://twitter.com/tufook/status/1632099883468591104))
- 3. 注册一个 ChatGPT 账号，然后验证手机号。我用的接码平台是 sms-activate https://t.co/dTNKV3uymZ （含 affiliate）
  它似乎涨价了，并且支付宝付款最低 1 美元。我选了英国的手机号，验证成功。 ([View Tweet](https://twitter.com/tufook/status/1632099885850984448))
- 4. 注册 ChatGPT 的账号后，可以生成一个 API key，因为只会给你看一次，所以务必保存起来。
  5. 新建 Telegram bot 的流程很简单，搜索 botfather 这个官方 bot 就能按照指引完成。 ([View Tweet](https://twitter.com/tufook/status/1632099888241467395))
- 6. 目前 Telegram bot + ChatGPT 的教程还不多，我找到的是这个 https://t.co/i8WZWPPAQz 
  这个教程的问题是对新手很不友好，在使用这个仓库的代码之前需要：
  a. 在服务器上装好 Docker 和 Docker compose
  b. 将仓库代码下载到服务器
  但不得不说，最后搭建出来的 bot 很好用。 ([View Tweet](https://twitter.com/tufook/status/1632099890334691328))
- 感谢互联网。至少还有互联网能让我们不是孤立无援的。 ([View Tweet](https://twitter.com/tufook/status/1632099892486348800))
