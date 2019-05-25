slack 集成 hubot 聊天机器人 安装流程

### 依赖
```
yum install -y epel-release

yum install -y nodejs
```
### 安装 创建第一个机器人
```
npm install -g yo generator-hubot

mkdir my-awesome-hubot && cd my-awesome-hubot

yo hubot --adapter=slack
```
### 从slack 获取token

有两种方式，一种是通过创建app，一种是创建integration

Create a Slack App with a Bot User (recommended)  用于新版本的slack

Create a configuration of the Hubot Integration   用于老版本的slack


### 允许hubot
```
cd my-awesome-hubot

rm -rf hubot-scripts.json

HUBOT_SLACK_TOKEN=xoxb-YOUR-TOKEN-HERE ./bin/hubot --adapter slack
```
### hubot 机器人说明

安装后预编写好的脚本功能 external-scripts.json

预编写后的回复，通过正则来匹配，然后响应  scripts/example.coffee

https://hubot.github.com/docs/scripting/

### 参考网址

https://api.slack.com/

https://slack.dev/hubot-slack/

https://hubot.github.com/docs

https://github.com/slackapi/hubot-slack

