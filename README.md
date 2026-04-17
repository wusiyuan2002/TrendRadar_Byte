<div align="center" id="trendradar">

<a href="https://github.com/sansan0/TrendRadar" title="TrendRadar">
  <img src="/_image/banner.webp" alt="TrendRadar Banner" width="80%">
</a>

最快<strong>30秒</strong>部署的竞品情报助手 —— 自动收集 AIGC 动态，AI 生成战略日报

<br><br>

[![GitHub Stars](https://img.shields.io/github/stars/sansan0/TrendRadar?style=flat-square&logo=github&color=yellow)](https://github.com/sansan0/TrendRadar)
[![License](https://img.shields.io/badge/license-GPL--3.0-blue.svg?style=flat-square)](LICENSE)
[![飞书通知](https://img.shields.io/badge/飞书-战略日报推送-00D4AA?style=flat-square)](https://www.feishu.cn/)
[![AI分析推送](https://img.shields.io/badge/AI-大模型战略分析-FF6B6B?style=flat-square&logo=openai&logoColor=white)](#)

</div>

<div align="center">

**中文** | **[English](README-EN.md)**

</div>

> 本项目基于 TrendRadar 轻量级架构定制，专注于 **AIGC 视频/3D/音乐生成** 与 **AI 社交玩法** 的情报收集，并利用大模型自动生成面向字节跳动的竞品战略日报。

<br>

## 📑 快速导航

| | | |
|:---:|:---:|:---:|
| [🎯 **核心功能**](#-核心功能) | [🚀 **飞书推送配置**](#-飞书机器人配置教程) | [🧠 **AI 战略分析配置**](#-开启-ai-战略分析日报) |
| [☁️ **云端存储配置**](#-数据存储云端配置教程) | [⚙️ **调度系统设置**](#-设置推送时间与频率) | |

<br>

## ✨ 核心功能（摘录）

### **全网竞品与 AIGC 热点聚合**
- 默认监控主流技术社区与媒体平台。
- **四大竞品专项追踪**：重点采集 **OpenAI (Sora)、Meta (Movie Gen)、Google (Veo/Gemini)、Grok/xAI** 的官方动态及行业爆料。
- **RSS 深度订阅**：支持订阅竞品官方技术博客，获取一手论文与 API 更新信息。

### **AI 驱动的战略分析日报**
- **大模型自动撰稿**：调用免费 AI API，将零散新闻转化为结构化战略洞察。
- **对抗性视角分析**：提示词针对字节业务定制，包含技术突破评估、竞品迭代意图推演、潜在威胁研判。
- **飞书定时播报**：每日固定时间将《AIGC 竞品战略日报》推送至飞书群，实现晨会前信息同步。

### **HTML 报告与数据回看**
- 每日自动生成包含趋势标记的网页版报告，支持暗色模式与关键词检索，方便周末复盘制作长图。

### **云端免服务器运行**
- **GitHub Actions 驱动**：无需自有服务器，利用 GitHub 定时任务自动抓取。
- **远程云存储**：数据保存在云端，不占用本地资源，支持历史数据回溯分析。

<br>

## 🚀 飞书机器人配置教程

本项目的核心输出渠道为**飞书群机器人**。配置完成后，AI 生成的战略日报将直接送达你的飞书客户端。

### 第一步：获取飞书 Webhook 地址

**方案一：使用飞书机器人助手（推荐，配置最快）**
1. 电脑浏览器打开 [飞书机器人助手](https://botbuilder.feishu.cn/home/my-command)。
2. 点击“新建机器人指令”。
3. 触发器选择“Webhook 触发”。
4. 复制生成的 **Webhook 地址** 暂存。
5. 在“参数”中填入以下 JSON 结构（确保消息能正确解析）：
   ```json
   {
     "message_type": "text",
     "content": {
       "text": "{{内容}}"
     }
   }
