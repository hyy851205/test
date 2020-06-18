#test0002
https://blog.csdn.net/weixin_40816738/article/details/90383728?utm_medium=distribute.pc_relevant.none-task-blog-baidujs-2

https://www.cnblogs.com/chen8023miss/p/12082093.html
1硬件电路

1登录github，新建一个项目new repository
2把当前目录变成git可以管理的仓库
确认当前目录是自己的项目工程目录，在终端输入
git init
此时终端会显示“初始化空的Git仓库于/......git”
3查看当前提交状态
4提交文件
git commit -m ""
5在github里添加origin
git remote add origin https://github.com/***.git
如果之前配置过一次，再次配置则会提示以下错误：
ERROR：远程 origin 已经存在。
此时只需要将远程配置删除，重新添加即可；
git remote rm origin
git remote add origin https://github.com/***.git
再次提交文件即可正常使用

6上传文件
git push -u origin master
执行此命令后，git会提示输入github账户的用户名和密码，验证通过后，进行文件上传！




    ERROR：向github仓库推送时(Git push originmaster)，出现当前分支 master 没有对应的上游分支的错误。
    解决：推送当前分支并建立与远程上游的跟踪
    git push --set-upstream origin master

    ERROR：更新被拒绝，因为远程版本库包含您本地尚不存在的提交。这通常是因为另外一个版本库已向该引用进行了推送。再次推送前，您可能需要先整合远程变更（如 'git pull...'）。详见 'git push -- help' 中的 'Note about fast-forwards'小节。
    解决：git push -u origin +master
    强制推送，但这样会删除github仓库中之前有的文件！

    ERROR：如果git没有commit就执行push操作会出现以下错误，"unable to access https://github.com/**.git/: Empty reply from server"
    解决：只需要先commit 在 push即可



git config --global user.name "hyy851205"
 git config --global user.email "82611092@qq.com"
 git remote add origin https://github.com/hyy851205/test.gi
 git push -u origin +master
git push origin master

git remote rm origin

