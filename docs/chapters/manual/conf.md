LabelFree提供一系列的可配置项，通过.env文件进行配置。

配置项如下：

| 环境变量                | 描述                                            | 默认值              | 可能值       |
| ----------------------- | ----------------------------------------------- | ------------------- | ------------ |
| **SERVER_PORT**         | 服务端口（用于浏览器访问）                      | 8080                | 数字         |
| **SERVER_RUNTIME**      | 智能标注算法运行环境,runc（CPU）或nvidia（GPU） | runc                | runc，nvidia |
| **MAIL_SERVER**         | SMPT 服务器地址（用于重置密码）                 | 空                  | 任意         |
| **MAIL_PORT**           | SMPT 服务器地址端口                             | 空                  | 任意         |
| **MAIL_USERNAME**       | 发送者邮箱                                      | 空                  | 任意         |
| **MAIL_PASSWORD**       | SMTP 密码                                       | 空                  | 任意         |
| **MYSQL_ROOT_PASSWORD** | 数据库密码                                      | root!2345           | 任意         |
| **REDIS_PASSWORD**      | redis密码                                       | root!2345           | 任意         |
| **MINIO_ROOT_PASSWORD** | MINIO对象存储密码                               | YOUR_MINIO_PASSWORD | 任意         |


