#VIM
##安装
```
在ubuntu中安装
sudo apt-get install vim
```

##打开要编辑的文件
```
vi file
```
##编辑
```
i 进入插入模式
```
##复制、粘贴
```
yy 复制当前行
nyy 复制n行
p 粘贴
```
##删除
```
x 删除光标所在的字符
dd 删除当前行
```
##跳转
```
gg 跳转到文件首行
NG 跳到第N行
G 跳转到文件尾行
0 跳转到行首
$ 跳转到行尾
```
##搜索
```
/pattern 搜索pattern
```
##取消、恢复
```
u 取消
ctrl+r 恢复
```
##其他
```
Esc 退出编辑模式
:q 退出vim
:q! 强制退出vim
:wq 保存并退出vim
```