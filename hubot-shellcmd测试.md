1. 进入机器人的根目录
```
cd my-awesome-hubot/
```
2. 执行模块安装命令
```
npm install hubot-script-shellcmd
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
