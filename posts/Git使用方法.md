---
layout: page
title: Git使用方法
permalink: /GitUsage/
categories: Usage
parent: 开发者文档
---

# Git日常基本操作

- Git地址

  - 项目：[ByteLuv (github.com)](https://github.com/ByteLuv)
  - web前端仓库：[ByteLuv/ByteLuv-Web: ByteLuv web page (github.com)](https://github.com/ByteLuv/ByteLuv-Web)
  - 后端仓库：[ByteLuv/ByteLuv-Backend: ByteLuv backend repo (github.com)](https://github.com/ByteLuv/ByteLuv-Backend)
  - 文档：[ByteLuv Documentation](https://byteluv.github.io/)

- Git

  - Git是一种版本管理工具，将代码保存在远程仓库中，便于大家共同修改代码

- Git机制

  - 分为三部分：远程仓库（GitHub），本地仓库（.git)，本地文件
  - 远程仓库：如Github这样的网站，注册账号后可以自由创建目录

  ![image-20210912002016526](/assets/images/image-20210912002016526.png)

  - 本地仓库：本地克隆*或创建git仓库后的.git目录![image-20210912002027814](/assets/images/image-20210912002027814.png)

  - 本地文件：本地除了.git外的其他文件![image-20210912002146556](/assets/images/image-20210912002146556.png)

  - 日常流程如下：

    - 下载远程的仓库到本地（clone）
    - 从远程仓库把别人的修改同步到本地（pull）
    - 在本地修改一些代码
    - 标记修改的文件（add）
    - 将修改提交到本地仓库（commit）
    - 将本地仓库与远程仓库同步（push）

  - 常见问题：

    - 冲突（conflict）：在本地修改了文件A，有别人也修改了A并在你同步（Pull）之后提交到了远程仓库，从而造成某段代码同时被两个人修改的问题，导致无法提交（Push）
    - 解决方法：1. 在修改代码之前养成pull的习惯    2.出现冲突后，手动将代码整合正确，再次Commit，Push

    

- Git Desktop操作：

  - 下载[GitHub Desktop](https://desktop.github.com/)

  - 在Git Desktop中选择File -> Clone Repository

  - 加入ByteLuv组织后，会出现ByteLuv的仓库

    ![image-20210912002944168](/assets/images/image-20210912002944168.png)

  - **Clone：**选择本地目录后选择克隆

  ![image-20210912003047670](/assets/images/image-20210912003047670.png)

  - 此时本地仓库和本地文件都被同步到了指定的文件夹中

  ![image-20210912003249432](/assets/images/image-20210912003249432.png)

  - **Pull: **同步远程仓库的修改

  ![image-20210912004416499](/assets/images/image-20210912004416499.png)

  - 修改一些文件

  ![image-20210912003606304](/assets/images/image-20210912003606304.png)

  - 在Git Desktop中看到修改

  ![image-20210912003638431](/assets/images/image-20210912003638431.png)

  - **Add:** 标记希望提交的修改

  ![image-20210912003710181](/assets/images/image-20210912003710181.png)

  - **Commit:** 提交到本地仓库（需要加注释表明这次提交了什么修改）

  ![image-20210912003904314](/assets/images/image-20210912003904314.png)

  - History中核验自己的修改

  ![image-20210912003943308](/assets/images/image-20210912003943308.png)

  - **Push:** 同步到远程仓库

  ![image-20210912004004818](/assets/images/image-20210912004004818.png)

- **Git命令行操作**

  - Clone : ``` git clone https://github.com/ByteLuv/ByteLuv-Web.git```
  - Pull : ```git pull ```
  - Add 
    - 标记所有修改: ``` git add . ```
    - 逐个标记修改: ```git add README.md```
  - Commit : ```git commit -m "这是一段注释"```
  - Push : ```git push```


[jekyll-organization]: https://github.com/jekyll

