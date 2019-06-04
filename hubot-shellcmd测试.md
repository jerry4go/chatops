1. 进入机器人的根目录
```
cd my-awesome-hubot/
```
2. 执行模块安装命令
```
npm install hubot-script-shellcmd

cp -R node_modules/hubot-script-shellcmd/bash ./

```

脚本会从 bash/handlers  读取，自己的编写的脚本要加执行权限，否则无法执行
```
chmod +x bash/handlers/*
```
3. 编辑external-scripts.json

添加一行
```
"hubot-script-shellcmd"
```
4. 常用命令

查看当前有哪些脚本
```
shellcmd
```

执行某个脚本，比如执行查看硬盘的脚本 disk
```
shellcmd disk
```

如果不想用shellcmd开头来执行，可以用别名来替换

比如用 run 替换 shellcmd

只需要在启动robot的时候加载这个变量
```
HUBOT_SHELLCMD_KEYWORD=run
```

5. 后台启动脚本
```
cd mybot

npm install --save forever

vim bin/hubot

把原先的启动脚本注释掉

#exec node_modules/.bin/hubot --name "my-awesome-hubot" "$@"

修改为

forever start -c coffee node_modules/.bin/hubot --name "my-awesome-hubot" "$@"


```












