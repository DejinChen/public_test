# public_test

使用VSCode想要在电脑上换一个git账户pull/push，有那种保存多账号方法，但是也可以直接重置，
git config --global --unset credential.helper
git config --global --unset user.name  
git config --global --unset user.email 

然后重设账户：
git config --global user.name "用户名"
git config --global user.email "用户邮箱"

同时还可以设置让VSCode记住git账号和密码：
git config --global credential.helper store

# git(vscode)修改用户名与密码
清除掉缓存在git中的账号和密码
git credential-manager remove | uninstall

运行一下命令，缓存输入的账号和密码：
git config --global credential.helper wincred