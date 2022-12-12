## 部署指引

**1. clone 本仓库**
请执行以下命令：

```bash
git clone https://github.com/IndustryEssentials/label-free.git
```

**2.环境变量配置**

请将`YOUR_HOST_IP`替换为服务器真实IP

```bash
export LABEL_HOST=YOUR_HOST_IP
```

**3.启动**

```bash
docker-compose up -d
```

**4.访问**

```bash
http://YOUR_HOST_IP:8080
```

默认管理员账号、密码：

```
labelfree@viesc.com
labelfree@2022
```

一切完成，开始标注工作吧！