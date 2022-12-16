## 部署步骤

### 1.服务器要求

- 操作系统要求：任何支持 Docker 的  x86 
- CPU内存要求：最低要求 2C4G
- 部署目录空间要求： 50G（取决于标注数据集的大小）

### 2.网络端口要求：

labelfree正常运行需要网络环境提供如下的网络端口配置要求，管理员可根据实际环境中组件部署的方案，在网络侧和主机侧开放相关端口：

| 组件  | 默认端口 | 说明                            |
| ----- | -------- | ------------------------------- |
| nginx | 8080     | 浏览器访问端口                  |
| mysql | 3306     | 默认安装的数据库对外提供的端口  |
| minio | 9000     | 默认安装的 minio对外提供的端口  |
| redis | 6379     | 默认安装的 Redis 对外提供的端口 |

### 3.安装步骤

**clone 本仓库** 请执行以下命令

```
git clone https://github.com/IndustryEssentials/label-free.git
```

**启动**

```
docker-compose up -d
```

**访问**

```
http://YOUR_HOST_IP:8080
```

默认管理员账号、密码

```
labelfree@viesc.com 
labelfree@2022
```

![](https://files.catbox.moe/5yaj3f.png)
