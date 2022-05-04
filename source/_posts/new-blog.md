---
title: 基础及出发
date: 2022-04-30 19:27:29
mathjax: true
tags:
---

> “生活需要**力量**，力量来自于**知识**。知识源自**积累**，积累出于兴趣与**渴望**”。

## 基础搭建
结合[Hexo图片公式问题](https://zhuanlan.zhihu.com/p/265077468)

### 多设备同步

1. 克隆需要同步的博客部分并修改:
``` bash
$ git clone git@github.com:jjjszszsjjj/jjjszszsjjj.github.io.git
```
2. 仅保留.git文件夹
3. 拷贝博客源文件除.deploy_git文件夹
4. 注意`.gitignore`文件
5. 上传至hexo(默认分支)
``` bash
$ git add .
$ git commit -m "upload to hexo branch"
$ git push
```
6. 移动/固定端使用
``` bash
$ git clone git@github.com:jjjszszsjjj/jjjszszsjjj.github.io.git # 默认hexo分支
$ git pull # 更新其他设备内容
$ npm install hexo --no-optional # 解决版本问题
```

### 图片相关修改
安装插件[hexo-renderer-marked](https://link.zhihu.com/?target=https%3A//github.com/hexojs/hexo-renderer-marked) 并修改`config.yaml`文档部分
``` bash
post_asset_folder: true
marked:
  prependRoot: true
  postAsset: true
```

### 工作机测试
插入图片并上传更新内容至hexo分支!["dsf"](/images/new-blog/temp.png)

### laptop测试
笔记本端修改并上传![移动端](/images/new-blog/temp2.png)

## 出发点

记录以及随时备份的必要性愈发关键,与此同时应当形成知识体系。

## 公式及其他

结合官方文档:[math equations](https://theme-next.js.org/docs/third-party-services/math-equations.html?highlight=math)

``` bash
$ npm un hexo-renderer-marked
$ npm i hexo-renderer-pandoc
```

$$ e=mc^2 $$  

$$
\begin{eqnarray}
\nabla\cdot\vec{E} &=& \frac{\rho}{\epsilon_0} \\
\nabla\cdot\vec{B} &=& 0 \\
\nabla\times\vec{E} &=& -\frac{\partial B}{\partial t} \\
\nabla\times\vec{B} &=& \mu_0\left(\vec{J}+\epsilon_0\frac{\partial E}{\partial t} \right)
\end{eqnarray}
$$

