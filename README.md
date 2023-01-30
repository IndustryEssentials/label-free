<a name="readme-top"></a>

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/IndustryEssentials/label-free">
    <img src="docs/assets/logo.jpg" alt="Logo" width="665" height="234">
  </a>

  <h3 align="center">欢迎使用LabelFree👋👋👋</h3>

  <p align="center">
    Labelfree 是一个开放的、可私有化部署的标注系统。旨在提供一个操作简单、数据可靠、高性能的数据标注系统，为算法服务提供可靠的底层数据支撑。
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


## 1 特性

- **简单**。简化概念，快速上手，只为数据标注。
- **高性能**。支持**超大数据集标注**、流畅**多人在线标注**体验。
- **智能**。内置算法模型，支持**交互式辅助分割标注**，提高10×标注效率🚀🚀🚀。
- **通用**。支持VOC、COCO等主流数据集格式导出。
- **开放**。支持**免费私有化部署**，数据安全可靠。
- **一键标注**。提供专业、一站式的数据标注服务。

<div align="center">
<table>
    <tr>
        <td><img src="./docs/assets/images/7aczgb.gif"></td>
        <td><img src="./docs/assets/images/3dzyj2.gif"></td>
        <td><img src="./docs/assets/images/yne8u4.gif"></td>
    <tr>
    <tr>
        <td align="center">目标检测</td>
        <td align="center">图像分割</td>
        <td align="center">图像分类</td>
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

1. 进入到【**项目**】界面，点击【**新建项目**】按钮，跳转至【**基础信息**】界面![](../assets/images/%E9%A1%B9%E7%9B%AE%E5%88%9B%E5%BB%BA.jpg)

2. 点击【**下一步**】，跳转至【**标签管理**】界面

3. 点击【**下一步**】，跳转至【**其它信息**】界面

4. 点击【**下一步**】进入【**上传数据集**】界面
     - 包含预标注，需要上传相应格式的数据集
     - 不包含预标注，可以上传任意格式的`zip`压缩包，LabelFree会自动解压缩并解析所有图片文件

5. 完成数据集上传，点击【**保存**】，即可完成项目的快速创建。

![](../assets/images/ith1md.png)


## 2.标注

创建项目之后点击标注按钮进入标注环节

![img](./docs/assets/images/ohnrrq.gif)

## 常用快捷键

| 按键   | 功能         | 按键        | 功能     |
| ------ | ------------ | ----------- | -------- |
| Q      | 连续画框     | 滚轮；+ / - | 缩放图片 |
| W      | 单个画框     | M           | 移动图片 |
| R      | 四点画框     | F           | 隐藏类别 |
| S      | 提交         | G           | 隐藏属性 |
| A      | 切换上一张图 | H           | 隐藏选中 |
| D      | 切换下一张图 | X           | 独显选中 |
| Z      | 撤销         | K           | 显示全部 |
| V      | 恢复         | C           | 清空全部 |
| Delete | 删除         |             |          |


更多信息见文档中心：[文档中心](https://labelfree.gitee.io/label-free/)
