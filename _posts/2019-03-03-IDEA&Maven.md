---
layout:     post
title:      IDEA
subtitle:   IDEA
date:       2019-03-03
author:     z9961
header-img: https://bing.ioliu.cn/v1/rand?w=1280&h=320
catalog: true
tags: IDEA
---





### 插件

##### .ignore 忽略文件或文件夹,免得把.idea提交上去

##### Lombok Plugin 使用@data来代替插入set、get、tostring等方法

##### Rainbow Brackets 多种颜色高亮

---

### 快捷键

soutv 快速打印变量

shift+alt+insert进入列选择模式，可选择一列或者多列

shift+alt+insert退出列选择模式


###  Intellij IDEA运行报Command line is too long

报错内容:

Error running 'ServiceStarter': Command line is too long. Shorten command line for ServiceStarter or also for Application default configuration.

修改项目下 .idea\workspace.xml，找到标签 <component name="PropertiesComponent"> ， 在标签里加一行  <property name="dynamic.classpath" value="true" />


### 无法记住github密码的问题

```
git config --global credential.helper store
```

设置之后再填一遍账号密码



## Maven

阿里云的maven镜像

```
<mirror>
<id>nexus-aliyun</id>
<mirrorOf>*</mirrorOf>
<name>Nexus aliyun</name>
<url>http://maven.aliyun.com/nexus/content/groups/public</url>
</mirror>

```

注意有的包不全,需要切换回来

例如com.github.ikidou中的TypeBuilder没有，不会在pom中报错，但是无法import



### update 2020.2.4