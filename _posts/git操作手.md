---
layout: post
title: "Git 操作手册"
subtitle: ' The Git Guide'
author: "Action.c"
header-style: text
tags:
  - Vim
---

Update: 我最后还是放弃在 Vim 模式下输入中文了，mental model 的 cost 太重了（

---

# 测试github地址
https://github.com/szc3659/szc3659.github.io.git
## 1、从远程仓库下载新分支与数据：

git fetch
该命令执行完后需要执行git merge 远程分支到你所在的分支。

## 2、从远端仓库提取数据并尝试合并到当前分支：
git  merge
该命令就是在执行 git fetch 之后紧接着执行 git merge 远程分支到你所在的任意分支。

假设你配置好了一个远程仓库，并且你想要提取更新的数据，你可以首先执行 git fetch [alias] 告诉 Git 去获取它有你没有的数据，然后你可以执行 git merge [alias]/[branch] 以将服务器上的任何更新（假设有人这时候推送到服务器了）合并到你的当前分支。
