---
title: 'Anaconda环境配置+常用指令'
description: 'Anaconda'
pubDate: '2026-08-30'
category: 'learning'
---

## **前言**

笔者在本科期间由于没有做过一点工程，导致Git等工具用的非常差劲。感谢Gemini让我在配环境的时候没有那么痛苦。（但是Gemini有时候真的很笨

感觉自己记忆有点不好所以需要把一些常用的指令记下来方便查阅。

灵异事件：我自己记得我一直在用my_env，并且确实缺了一些库且进行了安装，但是在environment.yml里面居然一直是base，一直没有export，所以我在新电脑上面直接导入环境的时候有报错。

## **常用指令**

> 启动工作

```
// 启动 Anaconda Prompt
cd /d D:\Workspace\my_first_python
conda activate my_env
git pull // 保证代码最新
jupyter notebook
```

> 上传到仓库

```
// Ctrl + C 退出Jupyter
git status
git add .
git commit -m "备注"
git push
```

> 安装库

```
conda install scikit-learn
conda env export > environment.yml
git add environment.yml
git commit -m "chore: 添加了新库scikit-learn"
git push
```
