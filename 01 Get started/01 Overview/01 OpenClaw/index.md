### 概览 (Overview)

**OpenClaw**

> [Logo 图 略]  
> “蜕壳！蜕壳！”——大概是一只太空龙虾说的  
> P.S. 译者注：EXFOLIATE 是一个科幻双关语。这句话的语气和句式，完美复刻了英国国民级科幻剧《神秘博士》中经典反派戴立克的标志性战吼：“EXTERMINATE! EXTERMINATE!”（抹杀！消灭！）。

**适用于任何操作系统的 AI 智能体网关，支持 Discord、Google Chat、iMessage、Matrix、Microsoft Teams、Signal、Slack、Telegram、WhatsApp、Zalo 等平台。**  
P.S. 译者注：在计算机网络和软件架构中，网关的主要作用是连接两个**协议不同、标准不同、甚至语言不同**的系统，并让他们能够顺畅地交流。

发送消息，即可从自己衣服口袋里获得智能体的回复。

仅需运行一个网关，即可横跨内置渠道、随附渠道插件、网页端聊天以及移动节点协同工作。

P.S. 译者注：  
<注开始>

- 内置渠道 (Built-in channels)：指软件在安装后，**原生自带、无需额外配置**就能直接使用的通信平台。你装好程序，填个 Token 就能用。
- 随附渠道插件 (Bundled channel plugins)：
  - 含义
    1. 插件 (plugins) ： 意味着这些功能是模块化的，不属于核心代码。如果某个平台（比如 Zalo 或特定的企业内网工具）API 变了，开发者只需要更新这个插件包，而不用重新发布整个网关程序。
    2. 随附 (Bundled（捆绑）) ： 虽然是插件形式，但开发者在发布安装包时，已经帮你把这些常用的扩展包**预先**打包在一起了。
       - 简单来说：插件是“零件”，扩展包（或插件包）是“零件盒”。
  - 就像买手机（网关）时附赠的一袋适配器（插件），虽然它们不是焊在手机里的，但你拿到手时就已经有了。
- 网页端聊天 (WebChat)：指基于浏览器的聊天界面。它可能是一个可以嵌入到任何网页上的 小组件，就像很多官网右下角的客服弹窗。也可能是一个独立的 Web 控制台，让你直接在浏览器里跟 AI 智能体对话，而不需要打开任何第三方聊天软件（如 WhatsApp）。
- 移动节点：通常的 App 只是一个“客户端”，它只负责显示画面。但“移动节点”暗示你的手机（移动端）本身就在运行网关的一部分功能。这意味着网关不仅仅死板地运行在服务器上，它也可以在你的 iOS 或 Android 设备上作为独立节点存在，直接处理消息、维护连接。

<注结束>

- [**开始使用 (Get Started)**](https://docs.openclaw.ai/start/getting-started)
  安装 OpenClaw 并在几分钟内启动网关。
- [**运行引导程序 (Run Onboarding)**](https://docs.openclaw.ai/start/wizard)
  使用 `openclaw onboard` 和配对流程进行引导式设置。
  - P.S. 译者注
    - 引导流程 (Onboarding)：原意是“登船”，现在指“新手引导”或“入职培训”。指用户第一次启动软件时，程序带你熟悉环境的过程。它是一个宏观的概念，包含了从你打开软件到你能够正常使用它之间的所有步骤（比如创建账号、接受协议、了解功能亮点等）。
    - 配对流程 (Pairing Process)：字面意思是 两个东西连在一起。例如：你在电脑上运行 openclaw，它显示一个二维码或验证码，你用手机扫一下或输入这个码。这个“握手”并建立信任的过程就是配对。
    - 引导式设置 (Guided Setup)：字面意思是 手把手教你如何配置。程序问：“你想连接哪个平台？”你选 “Telegram”。程序问：“你的 API Key 是多少？”你输入。这种“第一步...第二步...完成！”的向导模式就是引导式设置。
- [**打开控制台 UI (Open the Control UI)**](https://docs.openclaw.ai/web/control-ui)
  启动浏览器仪表盘，用于聊天、配置和会话管理。

---

### 什么是 OpenClaw？(What is OpenClaw?)

OpenClaw 是一个**自托管网关**，可将你最喜欢的聊天应用和渠道界面（内置渠道以及捆绑或外部渠道插件，如 Discord、Google Chat、iMessage、Matrix、Microsoft Teams、Signal、Slack、Telegram、WhatsApp、Zalo 等）连接到像 Pi 这样的 AI 编码智能体。你在自己的机器（或服务器）上运行单个网关进程，它就会成为你的消息传递应用与随时待命的 AI 助手之间的桥梁。  
P.S. 译者注：  
<注开始>

- 自托管 (Self-hosted)：
  - 云服务（非自托管）： 就像住酒店。你不需要打扫卫生、修水管（不用管维护），但你的一举一动酒店都知道，而且得交房费。
  - 自托管： 就像自己盖房子住。你需要自己配置服务器（比如家里的一台旧电脑、NAS 或者树莓派），自己安装和运行程序。
- 聊天应用 (Chat Apps) 和 渠道界面 (Channel Interfaces)
  - 聊天应用：外部平台。指 Discord、WhatsApp、微信等这些具体的软件产品。
  - 渠道界面：内部接口。这是网关内部的“翻译插件”。比如网关通过“Discord 渠道接口”去和“Discord 软件”打交道。
- Pi：这里的 Pi 指的应该是 Inflection AI 公司开发的一款名为 Pi 的人工智能（就像 ChatGPT 里的 GPT 一样）。它主打“个人助理（Personal Intelligence）”，说话风格非常像真人，且具有极高的情商。

<注结束>

**适用人群是谁？** 希望拥有一个可以随时随地发送消息的个人 AI 助手，同时又不想放弃数据控制权或依赖托管服务的开发人员和高级用户。  
P.S. 译者注：  
<注开始>  
目前的 AI 助手市场存在一个“鱼与熊掌不可兼得”的局面：

- 托管服务，比如 ChatGPT、Claude 的官方 App。
  - 优点： 随时随地，打开即用（Anytime, Anywhere）。
  - 代价： 你的对话数据存在人家的服务器上，你并不真正拥有数据控制权，且随时可能因为服务商调价或封号而受到影响。
- 本地运行 (Local AI)： 比如在自己电脑上跑 Ollama。
  - 优点： 隐私极高，完全免费。
  - 代价： 出了家门（离开了那台高性能电脑）就用不了，很难在手机上随时发消息沟通。

这段话的意思是：
“如果你既想要像用微信一样方便地调戏 AI，又有一颗‘被害妄想症’（极其重视隐私）且爱折腾的心，那么 OpenClaw 就是为你准备的。”  
我的理解是，它可以让你用微信（或类似的聊天工具），跟家里的插了 100 张显卡的电脑上跑着的本地 AI 说话，并得到其回复。  
<注结束>

**它有什么特别之处？**

- **自托管 (Self-hosted)：** 运行在你自己的硬件上，规则由你定。
- **多渠道 (Multi-channel)：** 单一网关可同时服务于内置渠道以及捆绑的或外部的渠道插件。
- **智能体原生 (Agent-native)：** 专为具备“工具使用”、“会话”、“记忆”和“多智能体路由”功能的编码智能体而构建。
  - 工具使用 (Tool use)：AI 不仅仅会“说”，还会“做”。例子： 你对 AI 说“查一下上海明天的天气并写个总结”。如果只是没有联网的本地聊天机器人，它可能会瞎编；但在“工具使用”支持下，网关能让 AI 真的去调用天气 API 接口，拿到真实数据再回复你。
  - 会话： 保证对话的连贯性，它知道你这句“它多少钱？”里的“它”是指上一句提到的“树莓派”。
  - 记忆： 这更进一步。它可能包含短期记忆（当前对话）和长期记忆（你三年前告诉它你喜欢 Python 编程）。网关会负责帮 AI 存储和检索这些“陈年往事”。
  - 多智能体路由：你的后台可能跑着好几个 AI。当你问“这段 Python 代码怎么优化？”——网关把消息路由给专攻编程的智能体。当你问“帮我画个猫”——网关自动切换到负责生成图片的智能体。
    - **路由**就是根据你的需求，把任务分发给最合适的那个 AI 处理。
  - 编码智能体 (Coding Agent)：
    - 聊天机器人 (Chatbot)： 像是一个理论专家。你问他“怎么写一个扫雷游戏？”，他会给你列出代码片段和步骤，然后对你说：“祝你好运，你自己去跑跑看吧。”
    - 编码智能体 (Coding Agent)： 像是一个实习生/助理。你告诉他“给我写个扫雷游戏”，他会：
      1. 自己打开编辑器，创建文件。
      2. 写下代码。
      3. 运行代码看看有没有 Bug。
      4. 如果报错了，他会自己看报错信息并修复，直到程序跑通。
      5. 最后把成品交给你。
- **开源 (Open source)：** 采用 MIT 许可证，由社区驱动。

---

### 你需要准备什么？(What do you need?)

Node 24（推荐），或者出于兼容性考虑使用 Node 22 LTS (22.14+)；一个来自你所选提供商的 API 密钥；以及 5 分钟的时间。为了获得最佳质量和安全性，请使用可获取的最强大的最新一代模型。

### 工作原理 (How it works)

该网关是会话、路由和渠道连接的唯一真实数据源（Single source of truth）。

### 核心能力 (Key capabilities)

- **多渠道网关 (Multi-channel gateway)：** 通过单一网关进程支持 Discord、iMessage、Signal、Slack、Telegram、WhatsApp、WebChat 等。
- **插件渠道 (Plugin channels)：** 在当前的常规版本中，捆绑的插件添加了对 Matrix、Nostr、Twitch、Zalo 等的支持。
- **多智能体路由 (Multi-agent routing)：** 为每个智能体、工作区或发送者提供隔离的会话。
- **媒体支持 (Media support)：** 发送和接收图像、音频和文档。
- **Web 控制台 UI (Web Control UI)：** 用于聊天、配置、会话和节点管理的浏览器仪表盘。
- **移动节点 (Mobile nodes)：** 配对 iOS 和 Android 节点，以实现画布（Canvas）、摄像头和语音驱动的工作流。

---

### 快速入门 (Quick start)

**1. 安装 OpenClaw**

```bash
npm install -g openclaw@latest
```

**2. 引导并安装服务**

```bash
openclaw onboard --install-daemon
```

**3. 聊天**
在浏览器中打开控制台 UI 并发送消息：

```bash
openclaw dashboard
```

或者连接一个渠道（Telegram 最快）并通过你的手机聊天。

需要完整的安装和开发设置指南？请参阅**开始使用 (Getting Started)**。

---

### 仪表盘 (Dashboard)

网关启动后，打开浏览器控制台 UI。

- 本地默认地址：**[http://127.0.0.1:18789/](http://127.0.0.1:18789/)**
- 远程访问：**Web 界面** 和 **Tailscale**

_(注：此处为聊天界面截图示例，一般在文档中不需要翻译截图内容)_

---

### 配置（可选）(Configuration (optional))

配置文件位于 `~/.openclaw/openclaw.json`。

- 如果你**不做任何配置**，OpenClaw 将在 RPC 模式下使用捆绑的 Pi 二进制文件，并采用按发送者隔离的会话。
- 如果你想限制访问权限，可以从设置 `channels.whatsapp.allowFrom` 以及（针对群组的）提及（@）规则开始。

示例：

```json
{
	"channels": {
		"whatsapp": {
			"allowFrom": ["+15555550123"],
			"groups": { "*": { "requireMention": true } }
		}
	},
	"messages": { "groupChat": { "mentionPatterns": ["@openclaw"] } }
}
```

---

### 从这里开始 (Start here)

- **文档中心 (Docs hubs)：** 所有的文档和指南，按用例组织。
- **配置 (Configuration)：** 核心网关设置、令牌 (tokens) 和提供商配置。
- **远程访问 (Remote access)：** SSH 和 tailnet 访问模式。
- **渠道 (Channels)：** 针对飞书 (Feishu)、Microsoft Teams、WhatsApp、Telegram、Discord 等的特定渠道设置。
- **节点 (Nodes)：** 支持配对、画布 (Canvas)、摄像头和设备操作的 iOS 及 Android 节点。
- **帮助 (Help)：** 常见修复方法和故障排除的入口点。

---

### 了解更多 (Learn more)

- **完整功能列表 (Full feature list)：** 完整的渠道、路由和媒体功能。
- **多智能体路由 (Multi-agent routing)：** 工作区隔离和按智能体划分的会话。
- **安全性 (Security)：** 令牌 (Tokens)、白名单和安全控制。
- **故障排除 (Troubleshooting)：** 网关诊断和常见错误。
- **关于与致谢 (About and credits)：** 项目起源、贡献者和许可证。
