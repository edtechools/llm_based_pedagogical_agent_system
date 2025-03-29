<div align="center"><a name="readme-top"></a>

![][image-banner]

# LLM-based-Pedagogical-Agent-System

基于大语言模型的教学智能体系统

<p align="center">
    <a href="https://ppt.edtools.top" target="_blank">
        <img alt="Static Badge" src="https://img.shields.io/badge/系统演示-f6f8fa"></a>
     <a href="https://docs.edtools.top" target="_blank">
        <img alt="Static Badge" src="https://img.shields.io/badge/项目文档-009054"></a>
    <a href="https://docs.edtools.top" target="_blank">
        <img alt="Static Badge" src="https://img.shields.io/badge/dynamic/json?color=ff69b4&label=bilibili-video&query=data.stat.view&url=https%3A%2F%2Fapi.bilibili.com%2Fx%2Fweb-interface%2Fview%3Fbvid%3DBV1hryGYzEVN"></a>
</p>

![Vue.js Badge](https://img.shields.io/badge/Vue.js-4FC08D?logo=vuedotjs&logoColor=fff&style=for-the-badge)
![Python Badge](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=fff&style=for-the-badge)
![FastAPI Badge](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=fff&style=for-the-badge)
![Django Badge](https://img.shields.io/badge/Django-092E20?logo=django&logoColor=fff&style=for-the-badge)
![Mattermost Badge](https://img.shields.io/badge/Mattermost-0058CC?logo=mattermost&logoColor=fff&style=for-the-badge)
![NGINX Badge](https://img.shields.io/badge/NGINX-009639?logo=nginx&logoColor=fff&style=for-the-badge)
![PostgreSQL Badge](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=fff&style=for-the-badge)
![Redis Badge](https://img.shields.io/badge/Redis-FF4438?logo=redis&logoColor=fff&style=for-the-badge)
![Docker Badge](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=fff&style=for-the-badge)
![Ubuntu Badge](https://img.shields.io/badge/Ubuntu-E95420?logo=ubuntu&logoColor=fff&style=for-the-badge)

</div>

<details>
<summary><kbd>Table of contents</kbd></summary>

#### TOC

- [目的](#目的)
- [功能介绍](#功能介绍)
- [使用方法](#使用方法)
  - [`1` 下载项目文件](#1-下载项目文件)
  - [`2` 安装项目依赖](#2-安装项目依赖)
  - [`3` 实现幻灯片](#3-实现幻灯片)
  - [`4` 加入教学智能体](#4-加入教学智能体)
  - [`5` 运行项目](#5-运行项目)
  - [`6` 部署项目](#6-部署项目)
- [Star History](#star-history)

####

<br/>

</details>

## 目的
> 为教师提供以『教师需求为核心』的设计与实现融入教学过程的**基于大语言模型的教学智能体**的技术工具

<div align="right">

[![][back-to-top]](#readme-top)

</div>

## 功能介绍

1. 幻灯片演示功能
2. 全局弹幕功能
3. 学生注意状态追踪功能
4. 教学智能体对话功能
5. 社群求助功能
6. 其它教学辅助功能

[![][back-to-top]](#readme-top)

## 使用方法

### `1` 下载项目文件

- 方法一：使用 git

```bash
git clone https://github.com/EdTechools/LLM-based-Pedagogical-Agent-System.git
```

- 方法二：下载 Releases 中的压缩包解压使用

### `2` 安装项目依赖

```bash
cd LLM-based-Pedagogical-Agent-System
npm install
```
<div align="right">

[![][back-to-top]](#readme-top)

</div>

### `3` 实现幻灯片

参考 [Slidev 文档](https://cn.sli.dev/guide/)

<div align="right">

[![][back-to-top]](#readme-top)

</div>

### `4` 加入教学智能体

1. 在 Dify 中实现应用，参考 [构建应用](https://docs.dify.ai/zh-hans/guides/application-orchestrate)
2. 获取应用的密钥，参考 [基于 APIs 开发](https://docs.dify.ai/zh-hans/guides/application-publishing/developing-with-apis)
3. 按照配置格式加入到对应的幻灯片中
- 每一个智能体由一个唯一标识字段标识，其下有三个子字段，分别是 `title` `key` `show`
- `title` 字段用来说明该教学智能体的名称。
- `key` 字段填入从 Dify 平台获得的该智能体的密钥。
- `show` 字段用来控制该智能体在页面的那一部分子页面进行展示，值的类型为数字列表，列表元素代表子页面的序号，如果值为字符串『all』时，代表智能体始终在该页面显示。
- 为了使智能体正常显示，还需要在内容部分引入 `<Agent />` 这个组件，该组件是该研究的开发成果，封装了教学智能体的显示逻辑，
使用者只需要按照格式完成配置即可。
- 和 agent 字段同一级别的 `clicks` 字段用来配置当前页面有几个子页面。
<div align="right">

[![][back-to-top]](#readme-top)

</div>

### `5` 运行项目

```bash
npm run dev
```
<div align="right">

[![][back-to-top]](#readme-top)

</div>

### `6` 部署项目

```
npm run build
```

将 `dist`目录中的静态文件部署到服务器上

<div align="right">

[![][back-to-top]](#readme-top)

</div>

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=EdTechools/LLM-based-Pedagogical-Agent-System&type=Date)](https://www.star-history.com/#EdTechools/LLM-based-Pedagogical-Agent-System&Date)

[back-to-top]: https://img.shields.io/badge/-BACK_TO_TOP-151515?style=flat-square
[image-banner]: https://github.com/EdTechools/LLM-based-Pedagogical-Agent-System/blob/main/img-storage/banner.png?raw=true
