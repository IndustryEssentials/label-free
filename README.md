<a name="readme-top"></a>
简体中文 | [English](./README.en.md)

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/IndustryEssentials/label-free">
    <img src="docs/assets/logo.jpg" alt="Logo" width="665" height="234">
  </a>

  <h3 align="center">欢迎使用LabelFree👋👋👋</h3>

  <p align="center">
    Labelfree 是一个开放的、可私有化部署的标注系统。旨在提供一个操作简单、数据可靠、高性能的数据标注系统，为算法服务提供可靠的底层数据支撑。<br /> 
    <br />
    全新支持  <b>Segment Anything</b>  模型进行分割辅助标注 🚀🚀🚀
    <br />
    <a href="https://labelfree.gitee.io/label-free/"><strong>文档 »</strong></a>
    <br />
    <br />
    ·
    <a href="https://github.com/IndustryEssentials/label-free/issues">反馈</a>
    ·
    <a href="https://github.com/IndustryEssentials/label-free/issues">讨论</a>
  </p>
</div>

</div>

<div align="center">
<table>
    <tr>
        <td><img src="https://files.catbox.moe/7aczgb.gif"></td>
        <td><img src="https://files.catbox.moe/3dzyj2.gif"></td>
    <tr>
    <tr>
        <td align="center">目标检测</td>
        <td align="center">图像分割</td>
    <tr>

</table>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>目录</summary>
  <ol>
    <li>
      <a href="#特性">特性</a>
    </li>
    <li>
      <a href="#一键部署">一键部署</a>
    </li>
    <li>
      <a href="#使用指南">使用指南</a>
    </li>
  </ol>
</details>

## 特性
- 一切为了提升标注生产效率。提供强大的标注交互界面、丰富的快捷键、流畅的多人协作等功能，让标注更加高效。
- 支持基于 **Segment Anything** 模型辅助标注。对比传统的分割标注，LabelFree 提供了交互式的分割标注，可以大大提升标注效率。
- 易于部署，基于 Docker ，简单几条命令即可部署。
- 数据安全性高。可私有化内网部署，不存在数据泄漏风险。
- 高性能。原生支持对象存储，不限制标注数据大小，支持海量数据标注。
- 一键标注。提供专业、一站式的数据标注服务。
<p align="right">(<a href="#readme-top">返回顶部</a>)</p>

<!-- GETTING STARTED -->
## 一键部署

1 clone 本仓库
请执行以下命令：
```bash
git clone https://github.com/IndustryEssentials/label-free.git

cd label-free
```

2 启动
```bash
docker-compose up -d
```

如果使用的是的docker-compose-plugin请尝试使用：

```bash
docker compose up -d
```

*ps: 系统初始化需要60s左右，请耐心等待。*

3 访问

```bash
http://localhost:8080
```

默认管理员账号、密码：


```
labelfree@viesc.com
labelfree@2022
```
*如发现无法新建项目，请确认使用的是默认管理员账号登陆。*

一切完成，开始标注工作吧！🍻🍻🍻
<p align="right">(<a href="#readme-top">返回顶部</a>)</p>

## 使用指南

## 1.创建项目

**1.1 新建项目**
点击“创建项目”按钮，进入创建项目页面

![image.png](https://labelfree.oss-cn-shenzhen.aliyuncs.com/public/label/image.png)

**1.2 设置标签属性**
在右侧的输入栏里输入标签名称，标签名称根据实际需求设置

![image.png](https://labelfree.oss-cn-shenzhen.aliyuncs.com/public/label/image%20%281%29.png)

1.3 **输入项目描述信息**
项目名称为自动生成的一个随机值，可根据实际需求更改
![image.png](https://labelfree.oss-cn-shenzhen.aliyuncs.com/public/label/image%20%282%29.png)

1.4 **上传数据集**
数据集只支持zip格式的压缩包，默认不包括标注信息，如果要上传包含标注信息的数据集，图片需放入 images 文件夹内，标注文件需放入 annotations 文件夹中。

![image.png](https://labelfree.oss-cn-shenzhen.aliyuncs.com/public/label/image%20%283%29.png)

## 2.标注

创建项目之后点击标注按钮进入标注环节

![img](https://files.catbox.moe/7aczgb.gif)

### 常用快捷键

| 按键        | 功能         |
| ----------- | ------------ |
| Q           | 连续画框     |
| W           | 单个画框     |
| R           | 四点画框     |
| S           | 提交         |
| A           | 切换上一张图 |
| D           | 切换下一张图 |
| Z           | 撤销         |
| V           | 恢复         |
| Delete      | 删除         |
| 滚轮；+ / -  | 缩放图片     |
| M           | 移动图片     |
| F           | 隐藏类别     |
| G           | 隐藏属性     |
| H           | 隐藏选中     |
| X           | 独显选中     |
| K           | 显示全部     |
| C           | 清空全部     |

更多信息见文档中心：[https://industryessentials.github.io/label-free/](https://industryessentials.github.io/label-free/)
