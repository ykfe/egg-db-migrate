# egg-db-migrate

- https://github.com/arcanis/clipanion
- https://github.com/SBoudrias/Inquirer.js

## Install

```
$ npm i -g egg-db-migrate
```

## Usages

```
$ db migrate
$ db migrate
$ db migrate --dev
$ db migrate --prod
$ db migrate --file init.sql
```

Options

- env 无参数，默认值dev
- file 指定sql文件名称，支持1个或多个。逗号分隔。如无指定，默认为db/*.sql

## 步骤

- 提示当前基础信息（开发环境，数据库用户等），输入密码。
- 先解析参数
- 读取egg配置文件，读取mysql配置。
- 执行sql