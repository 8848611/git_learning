git 命令总结:
1.git reset --hard 版本号    ==>回退到当前版本号
2.git mv 旧文件名 新文件名  ==>更改文件名 |mv是move的缩写|
3.git branch -v 查看本地有多少分支
4.git checkout -b 分支名称 版本号  ==>创建基于某个版本号的分支
5.git checkout 分支名称 ==>切换分支
6.gitk  ==>看版本历史界面工具
7.git cat-file -p 版本号  ==>显示版本库对象的内容

示例:
$ git cat-file -p 6b734da47b176bd5e8e518df1b17587fa8bf0824
tree 76d4b3d1e2bd50c8cf706fb4ffe3ac30ace8d644
parent 1087f96456c3b2dcb82b03e588cc0d200034b2e4
author zhiqingchun <18519395776@163.com> 1560263371 +0800
committer zhiqingchun <18519395776@163.com> 1560263371 +0800
-----------------------------------------------------------------------------
$ git cat-file -p 76d4b3d1e2bd50c8cf706fb4ffe3ac30ace8d644
100644 blob e91519abba8ad0259772b61c2096dd6bf87e1c36    demo.html
100644 blob ef171b9786a544bf286e135e138353b8b35a8824    vue.js
8.git diff 版本号 之前的版本号   ==> 版本号之间做比较(修改了哪些内容)
  或者是git diff HEAD HEAD~1(HEAD~2)  HEAD是当前版本号 HEAD~1是上一个版本号(HEAD~2是上一个的上一个版本号)
  或者是git diff HEAD HEAD^   原理同上
9.git branch -D 分支名  ==>删除分支
10.git commit --amend   ==>修改最近一次commit描述内容(amend:修正;修订)
	改完之后,ctrl+c :wq 保存并退出
11.git diff --cached  ==>暂存区和HEAD所含文件的差异
12.git diff  ==>工作区和暂存区的差异(所有文件)
13.git diff -- 文件名  ==>工作区和暂存区指定文件的差异
14.git diff 分支名 分支名 -- 文件名  ==>比较两个分支的某个文件的差异
15.git reset HEAD  ==>(当已经使用add命令放到暂存区了,但想让暂存区的所有文件恢复到HEAD,可用此命令)
16.git reset HEAD -- 文件名  ==>恢复暂存区部分文件的更改
17.git checkout -- 文件名  ==>将工作区恢复成暂存区的内容
18.git rm 文件名  ==>将文件名删除,然后直接commit即可
19.git stash  ==>将工作区修改的内容暂时先存起来
20.git stash list ==>查看stash列表
21.git stash apply  ==>恢复之前工作区暂存起来的内容,stash列表没有清空
22.git stash pop  ==>恢复之前工作区暂存起来的内容,stash列表清空
