# Git安装和使用

1. 安装git

2. `git init`  初始化git仓库

- 这个仓库会存放，git对我们项目代码进行备份的文件

3. 配置个人信息
- 全局配置信息

- user 是git内自己的对象

  `git config --global user.name "小明"`

  `git config --global user.email "admin@xx.com"`

4. 把代码存储在仓库中
  4.1 把文件放在仓库的门口（暂存区）
  `git add .`
  4.2 把大门口的东西放在房间里（版本库）
  `git commit -m` "这是说明"

5. 查看当前的状态
  - `git status`

6. 可以一次性把代码存储在仓库中
    `git commit --all -m "这是一次性添加文件"`
7. 查看日志
    `git log` 查看历史提交的日志
    `git log --oneline` 查看简洁的日志
    

8. 回退到制定的版本  相当于备份
  8.1 通过索引进行回退  
    - `git reset --hard Head~0`  回退一次  0是索引 索引是从上一个文件开始 然后增加
  8.2 通过版本号进行回退
    - `git reset --hard 76bf939` 回退到当前的版本号
9 存储版本切换的记录
  `git reflog` 存储版本切换的记录 可以看到每一次版本的记录


10.创建分支 
  - 为了避免 功能未写完，如果提交到主分支，那么别人拿到代码是不能执行 然后采用了分支的思想
  `git branch dev` 创建dev分支
  `git branch` 查看分支
  `git checkout dev` 切换到dev分支
  `git checkout master` 切换到主分支 master中
  `git merge dev` 将dev 合并到master
  `git branch -d dev` 删除dev分支