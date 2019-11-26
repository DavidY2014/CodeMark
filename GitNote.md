# CodeMark

# 如何把本地仓库和远程仓库关联
1,在github上新建一个仓库，勾选 Initialize this repository with a README 这一步的目的是为了获取仓库的地址，比如我的地址是
```
https://github.com/an942014/TechUHowToConnectLocalToRemoteStepbyStep.git
```

2,进入本地目录，创建一个空的仓库
```
git init
```

3，此时本地仓库没有远程仓库链接，所以需要关联远程仓库,记住远程连接是自己的，不要让我的仓库做测试
```
git remote add origin https://github.com/an942014/TechUHowToConnectLocalToRemoteStepbyStep.git
```

4,测试关联性,如果你本地获取到ReadMe的文件，说明就关联上了
```
git pull origin master
```

5,编辑gitignore，这个不是必须的

6,测试新增一个文件并提交到本地仓库
```
touch newfile
git add newfile
git commit -m'add new file'
```

6，推送本地的修改到远程仓库
```
git push -u origin master
```
