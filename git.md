# Git安装和使用

1. 安装git

2. git init  初始化git仓库

- 这个仓库会存放，git对我们项目代码进行备份的文件

3. 配置个人信息
- 全局配置信息

- user 是git内自己的对象

  git config --global user.name "小明"

  git config --global user.email "admin@xx.com"

4. 把代码存储在仓库中
  4.1 把文件放在仓库的门口
  git add .
  4.2 把大门口的东西放在房间里
  git commit -m "这是说明"