<div align="center" id="trendradar">

<a href="https://github.com/sansan0/TrendRadar" title="TrendRadar">
  <img src="/_image/banner.webp" alt="TrendRadar Banner" width="80%">
</a>

<p>最快<strong>30秒</strong>部署的竞品情报助手 —— 自动收集 AIGC 动态，AI 生成战略日报</p>

<a href="https://trendshift.io/repositories/14726" target="_blank">
  <img src="https://trendshift.io/api/badge/repositories/14726" alt="sansan0%2FTrendRadar | Trendshift" style="width: 250px; height: 55px;" width="250" height="55">
</a>

<br><br>

<a href="https://github.com/sansan0/TrendRadar/stargazers">
  <img src="https://img.shields.io/github/stars/sansan0/TrendRadar?style=flat-square&logo=github&color=yellow" alt="GitHub Stars">
</a>
<a href="https://github.com/sansan0/TrendRadar/network/members">
  <img src="https://img.shields.io/github/forks/sansan0/TrendRadar?style=flat-square&logo=github&color=blue" alt="GitHub Forks">
</a>
<a href="LICENSE">
  <img src="https://img.shields.io/badge/license-GPL--3.0-blue.svg?style=flat-square" alt="License">
</a>
<a href="https://github.com/sansan0/TrendRadar">
  <img src="https://img.shields.io/badge/version-v6.6.1-blue.svg" alt="Version">
</a>
<a href="https://www.feishu.cn/">
  <img src="https://img.shields.io/badge/飞书-战略日报推送-00D4AA?style=flat-square" alt="飞书通知">
</a>
<a href="#">
  <img src="https://img.shields.io/badge/AI-大模型分析-FF6B6B?style=flat-square&logo=openai&logoColor=white" alt="AI分析推送">
</a>
<a href="https://github.com/sansan0/TrendRadar">
  <img src="https://img.shields.io/badge/GitHub_Actions-自动化-2088FF?style=flat-square&logo=github-actions&logoColor=white" alt="GitHub Actions">
</a>
<a href="https://hub.docker.com/r/wantcat/trendradar">
  <img src="https://img.shields.io/badge/Docker-部署-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker">
</a>

</div>

<div align="center">

<strong>中文</strong> | <a href="README-EN.md"><strong>English</strong></a>

</div>

<blockquote>
<p>本项目基于 TrendRadar 轻量级架构定制，专注于 <strong>AIGC 视频/3D/音乐生成</strong> 与 <strong>AI 社交玩法</strong> 的情报收集，并利用大模型自动生成面向字节跳动的竞品战略日报。</p>
</blockquote>

<br>

<h2>📑 快速导航</h2>

<div align="center">

<table>
  <tr>
    <td align="center"><a href="#-核心功能"><strong>🎯 核心功能</strong></a></td>
    <td align="center"><a href="#-飞书机器人配置"><strong>🚀 飞书配置</strong></a></td>
    <td align="center"><a href="#-ai-战略分析配置"><strong>🧠 AI 战略分析</strong></a></td>
  </tr>
  <tr>
    <td align="center"><a href="#-远程云存储配置"><strong>☁️ 云端存储</strong></a></td>
    <td align="center"><a href="#-调度系统配置"><strong>⚙️ 调度设置</strong></a></td>
    <td align="center"><a href="#-更新日志"><strong>📝 更新日志</strong></a></td>
  </tr>
</table>

</div>

<br>

<h2>✨ 核心功能</h2>

<h3>📊 全网竞品与 AIGC 热点聚合</h3>
<ul>
  <li>默认监控主流技术社区与科技媒体平台。</li>
  <li><strong>四大竞品专项追踪</strong>：重点采集 <strong>OpenAI (Sora)、Meta (Movie Gen)、Google (Veo/Gemini)、Grok/xAI</strong> 的官方动态及行业爆料。</li>
  <li><strong>RSS 深度订阅</strong>：支持订阅竞品官方技术博客，获取一手论文与 API 更新信息。</li>
</ul>

<h3>🧠 AI 驱动的战略分析日报</h3>
<ul>
  <li><strong>大模型自动撰稿</strong>：调用免费 AI API，将零散新闻转化为结构化战略洞察。</li>
  <li><strong>对抗性视角分析</strong>：提示词针对字节业务定制，包含技术突破评估、竞品迭代意图推演、潜在威胁研判。</li>
  <li><strong>飞书定时播报</strong>：每日固定时间将《AIGC 竞品战略日报》推送至飞书群，实现晨会前信息同步。</li>
</ul>

<h3>📄 HTML 报告与数据回看</h3>
<ul>
  <li>每日自动生成包含趋势标记的网页版报告，支持暗色模式与关键词检索，方便周末复盘制作长图。</li>
</ul>

<h3>☁️ 云端免服务器运行</h3>
<ul>
  <li><strong>GitHub Actions 驱动</strong>：无需自有服务器，利用 GitHub 定时任务自动抓取。</li>
  <li><strong>远程云存储</strong>：数据保存在云端，不占用本地资源，支持历史数据回溯分析。</li>
</ul>

<br>

<h2>🚀 飞书机器人配置</h2>

<p>本项目的核心输出渠道为<strong>飞书群机器人</strong>。配置完成后，AI 生成的战略日报将直接送达你的飞书客户端。</p>

<details>
<summary><strong>👉 点击展开：飞书 Webhook 配置教程</strong></summary>
<br>

<p><strong>GitHub Secret 配置（⚠️ Name 名称必须严格一致）：</strong></p>
<ul>
  <li><strong>Name（名称）</strong>：<code>FEISHU_WEBHOOK_URL</code></li>
  <li><strong>Secret（值）</strong>：你的飞书机器人 Webhook 地址</li>
</ul>

<br>

<p><strong>方案一：飞书机器人助手（推荐，配置简单）</strong></p>

<ol>
  <li>电脑浏览器打开 <a href="https://botbuilder.feishu.cn/home/my-command" target="_blank">https://botbuilder.feishu.cn/home/my-command</a></li>
  <li>点击"新建机器人指令"</li>
  <li>点击"选择触发器"，往下滑动，点击"Webhook 触发"</li>
  <li>此时你会看到"Webhook 地址"，复制暂存</li>
  <li>"参数"里放入以下内容，点击"完成"：</li>
</ol>

<pre><code>{
  "message_type": "text",
  "content": {
    "text": "{{内容}}"
  }
}
</code></pre>

<ol start="6">
  <li>点击"选择操作" &gt; "通过官方机器人发消息"</li>
  <li>消息标题填写"AIGC 战略日报"</li>
  <li>关键步骤：点击 + 按钮，选择"Webhook 触发"，按下图摆放：</li>
</ol>

<img src="_image/feishu.png" alt="飞书机器人配置示例" width="400">

<ol start="9">
  <li>将第4步复制的 Webhook 地址配置到 GitHub Secrets 中的 <code>FEISHU_WEBHOOK_URL</code></li>
</ol>

<br>

<p><strong>多群推送</strong>：用分号 <code>;</code> 分隔多个 Webhook URL 即可同时推送到多个飞书群。</p>

</details>

<br>

<h2>🧠 AI 战略分析配置</h2>

<p>目标：让 AI 读懂 AIGC 新闻，以字节跳动产品/战略视角输出日报。</p>

<details>
<summary><strong>👉 点击展开：AI 分析配置详解</strong></summary>
<br>

<h3>必需配置项（环境变量）</h3>

<table>
  <tr>
    <th>变量名</th>
    <th>填写内容</th>
    <th>说明</th>
  </tr>
  <tr>
    <td><code>AI_ANALYSIS_ENABLED</code></td>
    <td><code>true</code></td>
    <td>开启 AI 分析总开关</td>
  </tr>
  <tr>
    <td><code>AI_API_KEY</code></td>
    <td><code>sk-xxxxxx</code></td>
    <td>你的大模型 API Key</td>
  </tr>
  <tr>
    <td><code>AI_MODEL</code></td>
    <td><code>deepseek/deepseek-chat</code></td>
    <td>推荐 DeepSeek（上下文长、成本低）</td>
  </tr>
</table>

<h3>可选配置项</h3>

<table>
  <tr>
    <th>变量名</th>
    <th>默认值</th>
    <th>说明</th>
  </tr>
  <tr>
    <td><code>AI_API_BASE</code></td>
    <td>(自动)</td>
    <td>自定义 API 地址</td>
  </tr>
  <tr>
    <td><code>AI_TEMPERATURE</code></td>
    <td><code>1.0</code></td>
    <td>采样温度（0-2）</td>
  </tr>
  <tr>
    <td><code>AI_MAX_TOKENS</code></td>
    <td><code>5000</code></td>
    <td>最大生成 token 数</td>
  </tr>
</table>

<h3>自定义分析提示词</h3>

<p>修改 <code>config/ai_analysis_prompt.txt</code> 文件，植入以下分析逻辑：</p>

<ul>
  <li><strong>角色设定</strong>：你是一名服务于字节跳动 AIGC 团队的资深战略分析师。</li>
  <li><strong>关注焦点</strong>：
    <ol>
      <li>视频生成/3D/音频生成的技术突破（关注 Sora、Veo、即梦相关进展）。</li>
      <li>AI 社交类产品（Character.ai、Meta AI 角色）的新玩法。</li>
      <li>四大竞品（OpenAI、Meta、Google、xAI）的动态。</li>
    </ol>
  </li>
  <li><strong>输出要求</strong>：
    <ol>
      <li>核心摘要（200字以内）。</li>
      <li>对字节跳动相关业务的潜在影响评估。</li>
      <li>明早产研晨会建议关注的高优事项。</li>
    </ol>
  </li>
</ul>

</details>

<br>

<h2>☁️ 远程云存储配置</h2>

<p>为了在 GitHub Actions 环境下保存历史新闻数据以支持 AI 进行趋势对比，<strong>必须配置远程云存储</strong>。</p>

<details>
<summary><strong>👉 点击展开：Cloudflare R2 配置教程</strong></summary>
<br>

<p><strong>GitHub Secret 配置（需添加 4 项）：</strong></p>

<table>
  <tr>
    <th>Name（名称）</th>
    <th>Secret（值）说明</th>
  </tr>
  <tr>
    <td><code>S3_BUCKET_NAME</code></td>
    <td>存储桶名称（如 <code>trendradar-data</code>）</td>
  </tr>
  <tr>
    <td><code>S3_ACCESS_KEY_ID</code></td>
    <td>访问密钥 ID</td>
  </tr>
  <tr>
    <td><code>S3_SECRET_ACCESS_KEY</code></td>
    <td>访问密钥</td>
  </tr>
  <tr>
    <td><code>S3_ENDPOINT_URL</code></td>
    <td>S3 API 端点（格式：<code>https://&lt;account-id&gt;.r2.cloudflarestorage.com</code>）</td>
  </tr>
</table>

<br>

<p><strong>详细操作步骤：</strong></p>

<ol>
  <li>登录 <a href="https://dash.cloudflare.com/" target="_blank">Cloudflare Dashboard</a></li>
  <li>左侧侧边栏找到 <code>R2对象存储</code></li>
  <li>点击<code>概述</code> &gt; <code>创建存储桶</code>，输入名称（如 <code>trendradar-data</code>）</li>
  <li>回到<strong>概述</strong>页面，点击右下角 <code>Account Details</code> 中的 <code>Manage R2 API Tokens</code></li>
  <li>点击 <code>创建 Account API 令牌</code></li>
  <li><strong>关键设置</strong>：
    <ul>
      <li>权限：选择 <code>管理员读和写</code></li>
      <li>指定存储桶：选择 <code>仅适用于指定存储桶</code> 并选中你的桶</li>
    </ul>
  </li>
  <li>创建后<strong>立即复制</strong> Access Key ID 和 Secret Access Key（只显示一次）</li>
</ol>

</details>

<br>

<h2>⚙️ 调度系统配置</h2>

<details>
<summary><strong>👉 点击展开：推送时间与执行频率设置</strong></summary>
<br>

<h3>1. 调度预设（何时生成日报）</h3>

<p>在 <code>config/config.yaml</code> 中配置：</p>

<pre><code>schedule:
  enabled: true
  preset: "morning_evening"   # 早晚各汇总一次
</code></pre>

<p><strong>可选预设模板：</strong></p>

<table>
  <tr>
    <th>模板名</th>
    <th>说明</th>
  </tr>
  <tr>
    <td><code>morning_evening</code></td>
    <td>全天增量 + 晚间汇总（推荐）</td>
  </tr>
  <tr>
    <td><code>always_on</code></td>
    <td>全天候监控，有新增就推</td>
  </tr>
  <tr>
    <td><code>office_hours</code></td>
    <td>工作日办公时间推送</td>
  </tr>
</table>

<h3>2. 执行频率（多久抓取一次）</h3>

<p>修改 <code>.github/workflows/crawler.yml</code>：</p>

<pre><code>on:
  schedule:
    # 每30分钟抓取一次（UTC时间，对应北京时间需+8小时）
    - cron: "*/30 * * * *"
</code></pre>

<p><strong>常用 Cron 表达式参考：</strong></p>

<table>
  <tr>
    <th>需求</th>
    <th>Cron 表达式</th>
  </tr>
  <tr>
    <td>每30分钟</td>
    <td><code>*/30 * * * *</code></td>
  </tr>
  <tr>
    <td>每小时</td>
    <td><code>0 * * * *</code></td>
  </tr>
  <tr>
    <td>每天早8点（北京时间）</td>
    <td><code>0 0 * * *</code></td>
  </tr>
</table>

<blockquote>
<p>⚠️ <strong>注意</strong>：GitHub Actions 使用 UTC 时间，北京时间 = UTC + 8 小时。</p>
</blockquote>

</details>

<br>

<h2>📝 更新日志</h2>

<h3>2026/03/28 - v6.6.0</h3>
<ul>
  <li><strong>HTML 报告浏览器增强</strong>：支持宽屏布局、Tab 快速切换、暗色模式、实时搜索</li>
  <li><strong>一键复制新闻</strong>：鼠标悬停即可复制标题和链接</li>
  <li><strong>快捷键系统</strong>：支持 <code>W</code> 宽屏切换、<code>D</code> 暗色模式、<code>/</code> 搜索</li>
</ul>

<h3>2026/02/09 - mcp-v4.0.0</h3>
<ul>
  <li><strong>AI 消息直推飞书</strong>：AI 生成内容一键推送到飞书，Markdown 自动适配</li>
  <li><strong>智能分批发送</strong>：超长消息自动按飞书 30KB 限制拆分</li>
</ul>

<h3>2026/01/23 - v5.4.0</h3>
<ul>
  <li>增加 AI 分析模式的独立控制功能</li>
  <li>新增 AI 分析时间窗口控制</li>
</ul>

<h3>2026/01/17 - v5.2.0</h3>
<ul>
  <li><strong>AI 翻译功能</strong>：支持将推送内容翻译为任意语言</li>
  <li><strong>配置架构优化</strong>：分析和翻译共享模型配置</li>
</ul>

<h3>2026/01/10 - v5.0.0</h3>
<ul>
  <li><strong>AI 智能分析推送</strong>：使用大模型对推送内容进行深度分析</li>
  <li><strong>飞书等渠道推送重构</strong>：五大板块清晰展示</li>
  <li><strong>独立展示区</strong>：指定平台完整热榜不受关键词过滤</li>
</ul>

<br>

<h2>📄 许可证</h2>

<p>GPL-3.0 License</p>

<hr>

<div align="center">

<a href="#trendradar">🔝 回到顶部</a>

</div>
