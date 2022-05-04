---
title: 常用命令
comments: true
date: 2022-05-04 19:44:11
tags:
- 命令
categories:
- bash
---

## Git 命令总结

``` bash
# 撤销改动
$ git checkout -- file #撤销对工作区文件改动
$ git reset file #撤销 git add添加内容

$ git reset file && git checkout -- file #提交后工作区又进行修改

$ git reset HEAD -- file #撤销暂存区文件修改, 保留工作区修改
$ git reset -- hard HEAD -- file #撤销暂存区文件修改, 不保留工作区修改

# 创建新分支及提交
$ git checkout -b branch_name && git push origin branch_name -u
# 切换分支
$ git checkout branch_name
# 特定分支内容
$ git clone -b branch_name repository_add
```
