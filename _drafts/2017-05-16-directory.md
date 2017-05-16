---
layout: post
title: Linux常用命令之目录操作
categories: Linux
description: some word here
keywords: Linux, command, directory
---

和 Windows 系统类似，Linux 系统下的文件系统也是一个树形结构。不过Linux中的文件系统只有一棵树，且树的顶端是一个目录（directory），名为`/`。

# 相关概念

## 分区

在 Windows 系统中，硬盘将分为多个分区（ C盘，D盘…），每个盘的最顶级都是多个文件夹（ folder ），每个文件夹下面有文件和子文件夹，子亦有孙，孙亦有子，形成一个树形结构。 每个分区会有自己的一个树。每一根儿树的最顶端是像 C: 或 D: 这样的盘符。

Linux 系统下的情况类似，硬盘也会被分为多个分区（ partition ），但是名字不叫 C 盘 D 盘，而是叫 sda1，sda2… 文件的组织也是一个树形结构。区别是，Linux 下把文件夹（ folder ）叫做目录（ directory ），而且整个系统不管有多少个分区，文件系统却只会有一棵树。树的顶端是一个目录（名字叫`/`）。

### 挂载点

为了将多个分区对应到一棵文件系统树上，



# 相关命令

## man

查看关键词的manpage(manual page) 。

```shell
$ man ls
```



## --help

bash命令，查看关键词的快捷帮助而不是manpage。

```shell
$ ls --help
```

“--help”选项并不是一个“独立”的工具，而是作为一种命令的选项，提供一种快捷、高效的帮助。

## info

与man相比，info工具可显示更完整的最新的GNU工具信息。

```shell
$ info ls
```

通常情况下，man工具显示的非GNU工具的信息是唯一的，而info工具显示的非GNU工具的信息是man页内容的副本补充。



