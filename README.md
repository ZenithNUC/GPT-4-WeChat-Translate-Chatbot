# GPT-4 WeChat Translate Chatbot

一个基于OpenAI GPT-4的微信翻译机器人，为用户提供文本翻译功能。

## 功能

私聊中自动翻译用户内容至目标语言
群聊中通过设定唤醒关键词激活机器人回复
支持重置聊天上下文
支持通过配置文件自定义参数

## 环境要求

Node.js >= 14

TypeScript

## 安装与运行
克隆本项目至本地：

下载代码
```bash
git clone https://github.com/yourusername/your-repo.git
```
进入项目目录：

```bash
cd your-repo
```
安装依赖：

```bash
npm install
```

在src/config.json中修改其中的配置参数，例如API密钥和目标语言等。

编译TypeScript代码：

```bash
npm run build
```

运行项目：

```bash
npm start
```

这将启动微信机器人，扫描二维码登录后即可开始使用。

## 配置文件说明

在config.json文件中，您可以设置以下参数：

OPENAI_API_KEY: 您的OpenAI API密钥

reverseProxyUrl: 反向代理地址，如果需要使用，请填写您的代理服务器地址

groupKey: 群聊中唤醒机器人的关键词

privateKey: 私聊中唤醒机器人的关键词（可留空）

resetKey: 重置聊天上下文的关键词

groupReplyMode: 是否在群聊中带上提问的问题（布尔值，true或false）

privateReplyMode: 是否在私聊中带上提问的问题（布尔值，true或false）

transLanguage: 要翻译的目标语言（如法语）

## 注意事项

使用时请遵守相关法律法规，尊重用户隐私，合理使用API。
本项目仅供学习和研究使用，不得用于任何商业用途。

## 开源许可

本项目采用MIT许可协议，项目基于[ChatGPT-wechat-bot](!https://github.com/AutumnWhj/ChatGPT-wechat-bot)进行修改
