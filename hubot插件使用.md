### 说明

hubot是一个开源的聊天机器人框架，支持很多的插件。

hubot的插件安装都是通过npm install来执行，安装完之后，

通常需要在external-scripts.json里面追加新安装的插件名（有的插件不需要加，比如hubot-bearychat）。

根据不同插件的需求，还需要设置相应的环境变量。

### 插件

1.hubot-slack

将hubot集成到slack中

安装（记得需要进入创建的机器人的主目录执行，否则报错）

npm install hubot-slack

环境变量

HUBOT_SLACK_TOKEN

2.hubot-jenkins

将hubot集成到jenkins中

安装（记得需要进入创建的机器人的主目录执行，否则报错）

``npm install hubot-jenkins``

环境变量

HUBOT_JENKINS_URL

HUBOT_JENKINS_AUTH（Auth的格式为user:password）

3.hubot-script-shellcmd

提供hubot执行linux shell脚本的能力

安装（记得需要进入创建的机器人的主目录执行，否则报错）

npm install hubot-script-shellcmd

4.hubot-grafana

将hubot接入到grafana获取到图表

安装

npm install hubot-grafana

环境变量

HUBOT_GRAFANA_HOST

HUBOT_GRAFANA_API_KEY



















