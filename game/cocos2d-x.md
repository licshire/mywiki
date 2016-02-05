###新项目
```
cocos new newgame -p com.you.newgame -l cpp -d newgame
```
new 项目名 -p 包名 -l 语言 -d 目录

###发布Android版本
在项目目录执行如下命令  
debug版本  
```
cocos run -p android –android-studio
```

release版本  
```
cocos run -p android -m release –android-studio
```

###Android NDK版本选择
r10c  (cocos2d-x 3.7)
###Android SDK版本选择
sdk 19  (cocos2d-x 3.7)