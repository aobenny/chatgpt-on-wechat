<p align="center"><img src= "https://github.com/user-attachments/assets/31fb4eab-3be4-477d-aa76-82cf62bfd12c" alt="Chatgpt-on-Wechat" width="600" /></p>

<p align="center">
   <a href="https://github.com/zhayujie/chatgpt-on-wechat/releases/latest"><img src="https://img.shields.io/github/v/release/zhayujie/chatgpt-on-wechat" alt="Latest release"></a>
  <a href="https://github.com/zhayujie/chatgpt-on-wechat/blob/master/LICENSE"><img src="https://img.shields.io/github/license/zhayujie/chatgpt-on-wechat" alt="License: MIT"></a>
  <a href="https://github.com/zhayujie/chatgpt-on-wechat"><img src="https://img.shields.io/github/stars/zhayujie/chatgpt-on-wechat?style=flat-square" alt="Stars"></a> <br/>
</p>

**chatgpt-on-wechat**（简称CoW）项目是基于大模型的智能对话机器人，支持自由切换多种模型，可接入网页、微信公众号、企业微信应用、飞书、钉钉中使用，能处理文本、语音、图片、文件等多模态消息，支持通过插件访问操作系统和互联网等外部资源，以及基于自有知识库定制企业AI应用。

# 简介

> 该项目既是一个可以开箱即用的对话机器人，也是一个支持高度扩展的AI应用框架，可以通过为项目添加大模型接口、接入渠道、自定义插件来灵活实现各种定制需求。支持的功能如下：

-  ✅   **多端部署：** 有多种部署方式可选择且功能完备，目前已支持网页、微信公众号、企业微信应用、飞书、钉钉等部署方式
-  ✅   **基础对话：** 私聊及群聊的AI智能回复，支持多轮会话上下文记忆，基础模型支持OpenAI, Claude, Gemini, DeepSeek, 通义千问, Kimi, 文心一言, 讯飞星火, ChatGLM, MiniMax, GiteeAI, ModelScope, LinkAI
-  ✅   **语音能力：** 可识别语音消息，通过文字或语音回复，支持 openai(whisper/tts), azure, baidu, google 等多种语音模型
-  ✅   **图像能力：** 支持图片生成、图片识别、图生图，可选择 Dall-E-3, stable diffusion, replicate, midjourney, CogView-3, vision模型
-  ✅   **丰富插件：** 支持自定义插件扩展，已实现多角色切换、敏感词过滤、聊天记录总结、文档总结和对话、联网搜索、智能体等内置插件
-  ✅   **Agent能力：** 支持访问浏览器、终端、文件系统、搜索引擎等各类工具，并可通过多智能体协作完成复杂任务，基于 [AgentMesh](https://github.com/MinimalFuture/AgentMesh) 框架实现
-  ✅   **知识库：** 通过上传知识库文件自定义专属机器人，可作为数字分身、智能客服、企业助手使用，基于 [LinkAI](https://link-ai.tech) 实现

## 声明

1. 本项目遵循 [MIT开源协议](/LICENSE)，仅用于技术研究和学习，使用本项目时需遵守所在地法律法规、相关政策以及企业章程，禁止用于任何违法或侵犯他人权益的行为。任何个人、团队和企业，无论以何种方式使用该项目、对何对象提供服务，所产生的一切后果，本项目均不承担任何责任
2. 境内使用该项目时，建议使用国内厂商的大模型服务，并进行必要的内容安全审核及过滤
3. 本项目当前主要接入协同办公平台，推荐使用网页、公众号、企微自建应用、钉钉、飞书等接入通道，其他通道为历史产物暂不维护

## 演示

DEMO视频：https://cdn.link-ai.tech/doc/cow_demo.mp4

## 社区

添加小助手微信加入开源项目交流群：

<img width="140" src="https://img-1317903499.cos.ap-guangzhou.myqcloud.com/docs/open-community.png">

<br/>

# 企业服务

<a href="https://link-ai.tech" target="_blank"><img width="750" src="https://cdn.link-ai.tech/image/link-ai-intro.jpg"></a>

> [LinkAI](https://link-ai.tech/) 是面向企业和开发者的一站式AI智能体平台，聚合多模态大模型、知识库、Agent 插件、工作流等能力，支持一键接入主流平台并进行管理，支持SaaS、私有化部署等多种模式。
>
> LinkAI 目前已在智能客服、私域运营、企业效率助手等场景积累了丰富的AI解决方案，在消费、健康、文教、科技制造等各行业沉淀了大模型落地应用的最佳实践，致力于帮助更多企业和开发者拥抱 AI 生产力。

**产品咨询和企业服务** 可联系产品客服：

<img width="150" src="https://cdn.link-ai.tech/portal/linkai-customer-service.png">

<br/>

# 🏷 更新日志

>**2025.05.23：** [1.7.6版本](https://github.com/zhayujie/chatgpt-on-wechat/releases/tag/1.7.6) 优化web网页channel、新增 [AgentMesh多智能体插件](https://github.com/zhayujie/chatgpt-on-wechat/blob/master/plugins/agent/README.md)、百度语音合成优化、企微应用`access_token`获取优化、支持`claude-4-sonnet`和`claude-4-opus`模型

>**2025.04.11：** [1.7.5版本](https://github.com/zhayujie/chatgpt-on-wechat/releases/tag/1.7.5) 新增支持 [wechatferry](https://github.com/zhayujie/chatgpt-on-wechat/pull/2562) 协议、新增 deepseek 模型、新增支持腾讯云语音能力、新增支持 ModelScope 和 Gitee-AI API接口

>**2024.12.13：** [1.7.4版本](https://github.com/zhayujie/chatgpt-on-wechat/releases/tag/1.7.4) 新增 Gemini 2.0 模型、新增web channel、解决内存泄漏问题、解决 `#reloadp` 命令重载不生效问题

>**2024.10.31：** [1.7.3版本](https://github.com/zhayujie/chatgpt-on-wechat/releases/tag/1.7.3) 程序稳定性提升、数据库功能、Claude模型优化、linkai插件优化、离线通知

更多更新历史请查看: [更新日志](/docs/version/release-notes.md)

<br/>

# 🚀 快速开始



- 快速开始详细文档：[项目搭建文档](https://docs.link-ai.tech/cow/quick-start)

- 一键安装脚本说明：[一键安装脚本](https://github.com/zhayujie/chatgpt-on-wechat/wiki/%E4%B8%80%E9%94%AE%E5%AE%89%E8%A3%85%E5%90%AF%E5%8A%A8%E8%84%9A%E6%9C%AC)

```bash
bash <(curl -sS https://cdn.link-ai.tech/code/cow/install.sh)
```

- 项目管理脚本说明：[项目管理脚本](https://github.com/zhayujie/chatgpt-on-wechat/wiki/%E9%A1%B9%E7%9B%AE%E7%AE%A1%E7%90%86%E8%84%9A%E6%9C%AC)

## 一、准备

### 1. 账号注册

项目默认使用OpenAI接口，需前往 [OpenAI注册页面](https://beta.openai.com/signup) 创建账号，创建完账号则前往 [API管理页面](https://beta.openai.com/account/api-keys) 创建一个 API Key 并保存下来，后面需要在项目中配置这个key。接口需要海外网络访问及绑定信用卡支付。

> 默认对话模型是 openai 的 gpt-3.5-turbo，计费方式是约每 1000tokens (约750个英文单词 或 500汉字，包含请求和回复) 消耗 $0.002，图片生成是Dell E模型，每张消耗 $0.016。

项目同时也支持使用 LinkAI 接口，无需代理，可使用 Kimi、文心、讯飞、GPT-3.5、GPT-4o 等模型，支持 定制化知识库、联网搜索、MJ绘图、文档总结、工作流等能力。修改配置即可一键使用，参考 [接入文档](https://link-ai.tech/platform/link-app/wechat)。

### 2.运行环境

支持 Linux、MacOS、Windows 系统（可在Linux服务器上长期运行)，同时需安装 `Python`。
> 建议Python版本在 3.7.1~3.9.X 之间，推荐3.8版本，3.10及以上版本在 MacOS 可用，其他系统上不确定能否正常运行。

> 注意：Docker 或 Railway 部署无需安装python环境和下载源码，可直接快进到下一节。

**(1) 克隆项目代码：**

```bash
git clone https://github.com/zhayujie/chatgpt-on-wechat
cd chatgpt-on-wechat/
```

注: 如遇到网络问题可选择国内镜像 https://gitee.com/zhayujie/chatgpt-on-wechat

**(2) 安装核心依赖 (必选)：**
> 能够使用`itchat`创建机器人，并具有文字交流功能所需的最小依赖集合。
```bash
pip3 install -r requirements.txt
```

**(3) 拓展依赖 (可选，建议安装)：**

```bash
pip3 install -r requirements-optional.txt
```
> 如果某项依赖安装失败可注释掉对应的行再继续

## 二、配置

配置文件的模板在根目录的`config-template.json`中，需复制该模板创建最终生效的 `config.json` 文件：

```bash
  cp config-template.json config.json
```

然后在`config.json`中填入配置，以下是对默认配置的说明，可根据需要进行自定义修改（注意实际使用时请去掉注释，保证JSON格式的完整）：

```bash
# config.json文件内容示例
{
  "model": "gpt-4o-mini",                                     # 模型名称, 支持 gpt-4o-mini, gpt-4.1, gpt-4o, wenxin, xunfei, glm-4, claude-3-7-sonnet-latest, moonshot等
  "open_ai_api_key": "YOUR API KEY",                          # 如果使用openAI模型则填入上面创建的 OpenAI API KEY
  "open_ai_api_base": "https://api.openai.com/v1",            # OpenAI接口代理地址
  "proxy": "",                                                # 代理客户端的ip和端口，国内环境开启代理的需要填写该项，如 "127.0.0.1:7890"
  "single_chat_prefix": ["bot", "@bot"],                      # 私聊时文本需要包含该前缀才能触发机器人回复
  "single_chat_reply_prefix": "[bot] ",                       # 私聊时自动回复的前缀，用于区分真人
  "group_chat_prefix": ["@bot"],                              # 群聊时包含该前缀则会触发机器人回复
  "group_name_white_list": ["ChatGPT测试群", "ChatGPT测试群2"], # 开启自动回复的群名称列表
  "group_chat_in_one_session": ["ChatGPT测试群"],              # 支持会话上下文共享的群名称  
  "image_create_prefix": ["画", "看", "找"],                   # 开启图片回复的前缀
  "conversation_max_tokens": 1000,                            # 支持上下文记忆的最多字符数
  "speech_recognition": false,                                # 是否开启语音识别
  "group_speech_recognition": false,                          # 是否开启群组语音识别
  "voice_reply_voice": false,                                 # 是否使用语音回复语音
  "character_desc": "你是基于大语言模型的AI智能助手，旨在回答并解决人们的任何问题，并且可以使用多种语言与人交流。",  # 人格描述
  # 订阅消息，公众号和企业微信channel中请填写，当被订阅时会自动回复，可使用特殊占位符。目前支持的占位符有{trigger_prefix}，在程序中它会自动替换成bot的触发词。
  "subscribe_msg": "感谢您的关注！\n这里是ChatGPT，可以自由对话。\n支持语音对话。\n支持图片输出，画字开头的消息将按要求创作图片。\n支持角色扮演和文字冒险等丰富插件。\n输入{trigger_prefix}#help 查看详细指令。",
  "use_linkai": false,                                        # 是否使用LinkAI接口，默认关闭，开启后可国内访问，使用知识库和MJ
  "linkai_api_key": "",                                       # LinkAI Api Key
  "linkai_app_code": ""                                       # LinkAI 应用或工作流code
}
```
**配置说明：**

**1.个人聊天**

+ 个人聊天中，需要以 "bot"或"@bot" 为开头的内容触发机器人，对应配置项 `single_chat_prefix` (如果不需要以前缀触发可以填写  `"single_chat_prefix": [""]`)
+ 机器人回复的内容会以 "[bot] " 作为前缀， 以区分真人，对应的配置项为 `single_chat_reply_prefix` (如果不需要前缀可以填写 `"single_chat_reply_prefix": ""`)

**2.群组聊天**

+ 群组聊天中，群名称需配置在 `group_name_white_list ` 中才能开启群聊自动回复。如果想对所有群聊生效，可以直接填写 `"group_name_white_list": ["ALL_GROUP"]`
+ 默认只要被人 @ 就会触发机器人自动回复；另外群聊天中只要检测到以 "@bot" 开头的内容，同样会自动回复（方便自己触发），这对应配置项 `group_chat_prefix`
+ 可选配置: `group_name_keyword_white_list`配置项支持模糊匹配群名称，`group_chat_keyword`配置项则支持模糊匹配群消息内容，用法与上述两个配置项相同。（Contributed by [evolay](https://github.com/evolay))
+ `group_chat_in_one_session`：使群聊共享一个会话上下文，配置 `["ALL_GROUP"]` 则作用于所有群聊

**3.语音识别**

+ 添加 `"speech_recognition": true` 将开启语音识别，默认使用openai的whisper模型识别为文字，同时以文字回复，该参数仅支持私聊 (注意由于语音消息无法匹配前缀，一旦开启将对所有语音自动回复，支持语音触发画图)；
+ 添加 `"group_speech_recognition": true` 将开启群组语音识别，默认使用openai的whisper模型识别为文字，同时以文字回复，参数仅支持群聊 (会匹配group_chat_prefix和group_chat_keyword, 支持语音触发画图)；
+ 添加 `"voice_reply_voice": true` 将开启语音回复语音（同时作用于私聊和群聊）

**4.其他配置**

+ `model`: 模型名称，目前支持 `gpt-4o-mini`, `gpt-4.1`, `gpt-4o`, `gpt-3.5-turbo`, `wenxin` , `claude` , `gemini`, `glm-4`,  `xunfei`, `moonshot`等，全部模型名称参考[common/const.py](https://github.com/zhayujie/chatgpt-on-wechat/blob/master/common/const.py)文件
+ `temperature`,`frequency_penalty`,`presence_penalty`: Chat API接口参数，详情参考[OpenAI官方文档。](https://platform.openai.com/docs/api-reference/chat)
+ `proxy`：由于目前 `openai` 接口国内无法访问，需配置代理客户端的地址，详情参考  [#351](https://github.com/zhayujie/chatgpt-on-wechat/issues/351)
+ 对于图像生成，在满足个人或群组触发条件外，还需要额外的关键词前缀来触发，对应配置 `image_create_prefix `
+ 关于OpenAI对话及图片接口的参数配置（内容自由度、回复字数限制、图片大小等），可以参考 [对话接口](https://beta.openai.com/docs/api-reference/completions) 和 [图像接口](https://beta.openai.com/docs/api-reference/completions)  文档，在[`config.py`](https://github.com/zhayujie/chatgpt-on-wechat/blob/master/config.py)中检查哪些参数在本项目中是可配置的。
+ `conversation_max_tokens`：表示能够记忆的上下文最大字数（一问一答为一组对话，如果累积的对话字数超出限制，就会优先移除最早的一组对话）
+ `rate_limit_chatgpt`，`rate_limit_dalle`：每分钟最高问答速率、画图速率，超速后排队按序处理。
+ `clear_memory_commands`: 对话内指令，主动清空前文记忆，字符串数组可自定义指令别名。
+ `hot_reload`: 程序退出后，暂存等于状态，默认关闭。
+ `character_desc` 配置中保存着你对机器人说的一段话，他会记住这段话并作为他的设定，你可以为他定制任何人格      (关于会话上下文的更多内容参考该 [issue](https://github.com/zhayujie/chatgpt-on-wechat/issues/43))
+ `subscribe_msg`：订阅消息，公众号和企业微信channel中请填写，当被订阅时会自动回复， 可使用特殊占位符。目前支持的占位符有{trigger_prefix}，在程序中它会自动替换成bot的触发词。

**5.LinkAI配置 (可选)**

+ `use_linkai`: 是否使用LinkAI接口，开启后可国内访问，使用知识库和 `Midjourney` 绘画, 参考 [文档](https://link-ai.tech/platform/link-app/wechat)
+ `linkai_api_key`: LinkAI Api Key，可在 [控制台](https://link-ai.tech/console/interface) 创建
+ `linkai_app_code`: LinkAI 应用或工作流的code，选填

**本说明文档可能会未及时更新，当前所有可选的配置项均在该[`config.py`](https://github.com/zhayujie/chatgpt-on-wechat/blob/master/config.py)中列出。**

## 三、运行

### 1.本地运行

如果是开发机 **本地运行**，直接在项目根目录下执行：

```bash
python3 app.py                                    # windows环境下该命令通常为 python app.py
```

终端输出二维码后，进行扫码登录，当输出 "Start auto replying" 时表示自动回复程序已经成功运行了（注意：用于登录的账号需要在支付处已完成实名认证）。扫码登录后你的账号就成为机器人了，可以在手机端通过配置的关键词触发自动回复 (任意好友发送消息给你，或是自己发消息给好友)，参考[#142](https://github.com/zhayujie/chatgpt-on-wechat/issues/142)。

### 2.服务器部署

使用nohup命令在后台运行程序：

```bash
nohup python3 app.py & tail -f nohup.out          # 在后台运行程序并通过日志输出二维码
```
扫码登录后程序即可运行于服务器后台，此时可通过 `ctrl+c` 关闭日志，不会影响后台程序的运行。使用 `ps -ef | grep app.py | grep -v grep` 命令可查看运行于后台的进程，如果想要重新启动程序可以先 `kill` 掉对应的进程。日志关闭后如果想要再次打开只需输入 `tail -f nohup.out`。此外，`scripts` 目录下有一键运行、关闭程序的脚本供使用。

> **多账号支持：** 将项目复制多份，分别启动程序，用不同账号扫码登录即可实现同时运行。

> **特殊指令：** 用户向机器人发送 **#reset** 即可清空该用户的上下文记忆。


### 3.Docker部署

> 使用docker部署无需下载源码和安装依赖，只需要获取 docker-compose.yml 配置文件并启动容器即可。

> 前提是需要安装好 `docker` 及 `docker-compose`，安装成功的表现是执行 `docker -v` 和 `docker-compose version` (或 docker compose version) 可以查看到版本号，可前往 [docker官网](https://docs.docker.com/engine/install/) 进行下载。

**(1) 下载 docker-compose.yml 文件**

```bash
wget https://open-1317903499.cos.ap-guangzhou.myqcloud.com/docker-compose.yml
```

下载完成后打开 `docker-compose.yml` 修改所需配置，如 `OPEN_AI_API_KEY` 和 `GROUP_NAME_WHITE_LIST` 等。

**(2) 启动容器**

在 `docker-compose.yml` 所在目录下执行以下命令启动容器：

```bash
sudo docker compose up -d
```

运行 `sudo docker ps` 能查看到 NAMES 为 chatgpt-on-wechat 的容器即表示运行成功。

注意：

 - 如果 `docker-compose` 是 1.X 版本 则需要执行 `sudo  docker-compose up -d` 来启动容器
 - 该命令会自动去 [docker hub](https://hub.docker.com/r/zhayujie/chatgpt-on-wechat) 拉取 latest 版本的镜像，latest 镜像会在每次项目 release 新的版本时生成

最后运行以下命令可查看容器运行日志，扫描日志中的二维码即可完成登录：

```bash
sudo docker logs -f chatgpt-on-wechat
```

**(3) 插件使用**

如果需要在docker容器中修改插件配置，可通过挂载的方式完成，将 [插件配置文件](https://github.com/zhayujie/chatgpt-on-wechat/blob/master/plugins/config.json.template)
重命名为 `config.json`，放置于 `docker-compose.yml` 相同目录下，并在 `docker-compose.yml` 中的 `chatgpt-on-wechat` 部分下添加 `volumes` 映射:

```
volumes:
  - ./config.json:/app/plugins/config.json
```
**注**：采用docker方式部署的详细教程可以参考：[docker部署CoW项目](https://www.wangpc.cc/ai/docker-deploy-cow/)

<br>

# 🔎 常见问题

FAQs： <https://github.com/zhayujie/chatgpt-on-wechat/wiki/FAQs>

或直接在线咨询 [项目小助手](https://link-ai.tech/app/Kv2fXJcH)  (知识库持续完善中，回复供参考)

# 🛠️ 开发

欢迎接入更多应用渠道，参考 [Terminal代码](https://github.com/zhayujie/chatgpt-on-wechat/blob/master/channel/terminal/terminal_channel.py) 实现接收和发送消息逻辑即可接入。 同时欢迎增加新的插件，参考 [插件说明文档](https://github.com/zhayujie/chatgpt-on-wechat/tree/master/plugins)。

# ✉ 联系

欢迎提交PR、Issues，以及 🌟Star 支持一下。程序运行遇到问题可以查看 [常见问题列表](https://github.com/zhayujie/chatgpt-on-wechat/wiki/FAQs) ，其次前往 [Issues](https://github.com/zhayujie/chatgpt-on-wechat/issues) 中搜索。个人开发者可加入开源交流群参与更多讨论，企业用户可联系[产品客服](https://cdn.link-ai.tech/portal/linkai-customer-service.png)咨询。

# 🌟 贡献者

![cow contributors](https://contrib.rocks/image?repo=zhayujie/chatgpt-on-wechat&max=1000)
