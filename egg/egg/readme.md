-   npm i squelize-cli -D（devDependencies)
    -   -D是开发阶段的依赖 mysql的处理 上线的时候是用不到的
    -   创建表
    -   执行sql
    -   squelize-cli command-line 命令行

-   sequelize 命令行
    -   1.sequelize init 初始化数据库mysql的工作目录 config.json 可以配置端口 账户名
    -   sequelize db:create 可以创建一个应经在config.json配置好的数据库
    -   创建一个表sequelize migration:create --name create create-users-table     sequelize db:migrate
    -   删除一个表 return queryInterface.dropTable('shops');   sequelize db:migrate:undo