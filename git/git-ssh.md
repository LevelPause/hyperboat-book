# 获取公钥
``` 
$ ssh-keygen -t rsa -C "youremail@xxx.com"
```
如果不需要密码的话, 一路三次回车即可得到公钥文件

# 将公钥添加至github
```
$ cd ~/.ssh
$ ls
```
将id_rsa.pub文件中的内容添加至github的ssh-key中

# 验证ssh

```console
$ ssh -T git@github.com
```
选择yes后如果出现以下内容则表示成功了, 否则请重新获取
```
 Hi humingx! You've successfully authenticated, but GitHub does not provide shell access.
```