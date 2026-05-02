# 首页所示的引导安装程序运行过程中的命令行提示

在 [Get started -> Overview -> OpenClaw](./01%20Get%20started/01%20Overview/01%20OpenClaw/index.md) 的*引导并安装服务*部分，执行`openclaw onboard --install-daemon`后，出现以下内容

```text


🦞 OpenClaw 2026.4.29 (a448042) — Your AI assistant, now without the $3,499 headset.

Windows detected - OpenClaw runs great on WSL2!
Native Windows might be trickier.
Quick setup: wsl --install (one command, one reboot)
Guide: https://docs.openclaw.ai/windows
▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄
██░▄▄▄░██░▄▄░██░▄▄▄██░▀██░██░▄▄▀██░████░▄▄▀██░███░██
██░███░██░▀▀░██░▄▄▄██░█░█░██░█████░████░▀▀░██░█░█░██
██░▀▀▀░██░█████░▀▀▀██░██▄░██░▀▀▄██░▀▀░█░██░██▄▀▄▀▄██
▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀
                  🦞 OPENCLAW 🦞

T  OpenClaw setup
|
o  Security disclaimer ----------------------------------------------------------------------+
|                                                                                            |
|  OpenClaw is a hobby project and still in beta. Expect sharp edges.                        |
|  By default, OpenClaw is a personal agent: one trusted operator boundary.                  |
|  This bot can read files and run actions if tools are enabled.                             |
|  A bad prompt can trick it into doing unsafe things.                                       |
|                                                                                            |
|  OpenClaw is not a hostile multi-tenant boundary by default.                               |
|  If multiple users can message one tool-enabled agent, they share that delegated tool      |
|  authority.                                                                                |
|                                                                                            |
|  If you’re not comfortable with security hardening and access control, don’t run           |
|  OpenClaw.                                                                                 |
|  Ask someone experienced to help before enabling tools or exposing it to the internet.     |
|                                                                                            |
|  Recommended baseline                                                                      |
|  - Pairing/allowlists + mention gating.                                                    |
|  - Multi-user/shared inbox: split trust boundaries (separate gateway/credentials, ideally  |
|    separate OS users/hosts).                                                               |
|  - Sandbox + least-privilege tools.                                                        |
|  - Shared inboxes: isolate DM sessions (session.dmScope: per-channel-peer) and keep tool   |
|    access minimal.                                                                         |
|  - Keep secrets out of the agent’s reachable filesystem.                                   |
|  - Use the strongest available model for any bot with tools or untrusted inboxes.          |
|                                                                                            |
|  Run regularly                                                                             |
|  openclaw security audit --deep                                                            |
|  openclaw security audit --fix                                                             |
|                                                                                            |
|  Learn more                                                                                |
|  - https://docs.openclaw.ai/gateway/security                                               |
|                                                                                            |
+--------------------------------------------------------------------------------------------+
|
*  I understand this is personal-by-default and shared/multi-user use requires lock-down. Continue?
|    Yes / > No
```

翻译后：

````text
# OpenClaw 2026.4.29 安装与安全声明

## 1. 启动界面预览

以下是 OpenClaw 启动时的终端界面翻译，包含安装建议与安全须知：

```text
🦞 OpenClaw 2026.4.29 (a448042) — 您的 AI 助手，现已摆脱 $3,499 的头显限制。

检测到 Windows 系统 - OpenClaw 在 WSL2 上运行体验极佳！
在原生 Windows 环境下配置可能会比较棘手。
快速安装：wsl --install（只需一条命令，一次重启）
指南：[https://docs.openclaw.ai/windows](https://docs.openclaw.ai/windows)
▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄
██░▄▄▄░██░▄▄░██░▄▄▄██░▀██░██░▄▄▀██░████░▄▄▀██░███░██
██░███░██░▀▀░██░▄▄▄██░█░█░██░█████░████░▀▀░██░█░█░██
██░▀▀▀░██░█████░▀▀▀██░██▄░██░▀▀▄██░▀▀░█░██░██▄▀▄▀▄██
▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀
                   🦞 OPENCLAW 🦞

T  OpenClaw 设置
|
o  安全免责声明 ----------------------------------------------------------------------+
|                                                                                            |
|  OpenClaw 是一个业余项目，目前仍处于测试（Beta）阶段。可能会有一些不完善之处。             |
|  默认情况下，OpenClaw 是一个个人智能体：处于单一受信任操作者的边界内。                     |
|  如果启用了相关工具，此机器人可以读取文件并执行操作。                                      |
|  恶意的提示词可能会诱导它执行不安全的操作。                                                |
|                                                                                            |
|  默认情况下，OpenClaw 并非为应对带有敌意的多租户环境而设计。                               |
|  如果多个用户可以向同一个启用了工具的智能体发送消息，他们将共享该委托工具的权限。          |
|                                                                                            |
|  如果您对安全加固和访问控制不熟悉，请不要运行 OpenClaw。                                   |
|  在启用工具或将其暴露到互联网之前，请寻求有经验的人士的帮助。                              |
|                                                                                            |
|  推荐的安全基线                                                                            |
|  - 配对/白名单 + 提及（@）限制机制。                                                       |
|  - 多用户/共享收件箱：划分信任边界（分离网关/凭证，最好分离操作系统用户/主机）。           |
|  - 沙箱环境 + 最小权限工具。                                                               |
|  - 共享收件箱：隔离私信会话（session.dmScope: per-channel-peer）并保持极简的工具访问权限。 |
|  - 不要将机密信息放置在智能体可访问的文件系统中。                                          |
|  - 为任何带有工具或处理不受信任收件箱的机器人使用最强大的可用模型。                        |
|                                                                                            |
|  定期运行                                                                                  |
|  openclaw security audit --deep                                                            |
|  openclaw security audit --fix                                                             |
|                                                                                            |
|  了解更多                                                                                  |
|  - [https://docs.openclaw.ai/gateway/security](https://docs.openclaw.ai/gateway/security)                                               |
|                                                                                            |
+--------------------------------------------------------------------------------------------+
|
* 我理解此程序默认为个人使用，在共享/多用户环境下使用需要进行安全锁定。是否继续？
|  是 / > 否
````
