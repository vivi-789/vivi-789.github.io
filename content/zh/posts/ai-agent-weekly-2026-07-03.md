---
title: "AI Native 组织变革周报 - 2026年7月3日"
slug: "ai-agent-weekly-2026-07-03"
date: 2026-07-03T15:00:00+08:00
draft: false
tags: ["AI Agent", "组织变革", "周报", "AI Native", "企业落地"]
categories: ["ai-native"]
description: "AI Native 组织变革周报第1期，涵盖 Agent Harness、AI Factory、人才模型变革等9条精选内容。"
disableToc: true
hideMeta: true
fullWidth: true
---

{{< rawhtml >}}
<style>

  :root {
    --bg: #faf7f2;
    --card: #fffdf9;
    --card-hover: #fdf8f0;
    --accent: #8b6f47;
    --accent-light: #a68763;
    --text: #3d352e;
    --text-muted: #8a7e72;
    --border: #e8ddd0;
    --tag-bg: #f3ece2;
    --tag-text: #8b6f47;
    --green: #5a7a52;
    --orange: #c47a3a;
    --red: #b85450;
    --section-bg: #f7f1e8;
  }
  * { margin: 0; padding: 0; box-sizing: border-box; }
  .weekly-report {
    background: var(--bg);
    color: var(--text);
    font-family: -apple-system, "PingFang SC", "Microsoft YaHei", "Helvetica Neue", sans-serif;
    line-height: 1.75;
  }
  .report-header {
    text-align: center;
    padding: 36px 24px 28px;
    background: linear-gradient(135deg, #1a1d27 0%, #16181f 100%);
    border-radius: 16px;
    border: 1px solid var(--border);
    margin-bottom: 28px;
  }
  .report-header h1 {
    font-size: 24px;
    font-weight: 700;
    margin-bottom: 8px;
    background: linear-gradient(135deg, #8b6f47, #c47a3a);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }
  .report-header .meta {
    font-size: 13px;
    color: var(--text-muted);
    display: flex;
    justify-content: center;
    gap: 16px;
    flex-wrap: wrap;
  }
  .report-header .meta span { display: inline-flex; align-items: center; gap: 4px; }

  /* 统计栏 */
  .stats-bar {
    display: flex;
    gap: 12px;
    margin-bottom: 28px;
    flex-wrap: wrap;
  }
  .stat-card {
    flex: 1;
    min-width: 140px;
    background: var(--card);
    border: 1px solid var(--border);
    border-radius: 12px;
    padding: 16px 20px;
    text-align: center;
  }
  .stat-card .num { font-size: 28px; font-weight: 700; color: var(--accent-light); }
  .stat-card .label { font-size: 12px; color: var(--text-muted); margin-top: 4px; }

  /* 板块标题 */
  .section-title {
    font-size: 18px;
    font-weight: 700;
    margin: 32px 0 16px;
    padding-left: 14px;
    border-left: 4px solid var(--accent);
    display: flex;
    align-items: center;
    justify-content: space-between;
  }
  .section-title .badge {
    font-size: 12px;
    background: var(--tag-bg);
    color: var(--tag-text);
    padding: 2px 10px;
    border-radius: 20px;
    font-weight: 400;
  }

  /* 访谈卡片 */
  .video-card {
    background: var(--card);
    border: 1px solid var(--border);
    border-radius: 14px;
    padding: 24px;
    margin-bottom: 20px;
    transition: border-color 0.2s;
  }
  .video-card:hover { border-color: var(--accent); }
  .video-card .card-header {
    display: flex;
    gap: 14px;
    margin-bottom: 16px;
    flex-wrap: wrap;
  }
  .video-card .thumb {
    width: 120px;
    height: 68px;
    border-radius: 8px;
    background: var(--section-bg);
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 11px;
    color: var(--text-muted);
    border: 1px solid var(--border);
    flex-shrink: 0;
  }
  .video-card .card-meta { flex: 1; min-width: 200px; }
  .video-card h3 {
    font-size: 15px;
    font-weight: 600;
    margin-bottom: 6px;
    line-height: 1.5;
  }
  .video-card h3 a {
    color: var(--text);
    text-decoration: none;
  }
  .video-card h3 a:hover { color: var(--accent-light); }
  .video-card .info-line {
    font-size: 12px;
    color: var(--text-muted);
    display: flex;
    gap: 10px;
    flex-wrap: wrap;
  }
  .video-card .info-line .channel { color: var(--accent-light); }
  .video-card .info-line .views { color: var(--green); }

  .speaker-box {
    background: var(--section-bg);
    border-radius: 8px;
    padding: 10px 14px;
    margin-bottom: 14px;
    font-size: 13px;
  }
  .speaker-box .label {
    color: var(--accent);
    font-weight: 600;
    margin-right: 6px;
  }

  .tags {
    display: flex;
    gap: 6px;
    flex-wrap: wrap;
    margin-bottom: 14px;
  }
  .tag {
    font-size: 11px;
    background: var(--tag-bg);
    color: var(--tag-text);
    padding: 3px 10px;
    border-radius: 20px;
  }

  .insight-list { list-style: none; padding: 0; }
  .insight-list li {
    padding: 10px 0 10px 22px;
    position: relative;
    font-size: 14px;
    border-bottom: 1px solid var(--border);
  }
  .insight-list li:last-child { border-bottom: none; }
  .insight-list li::before {
    content: "▸";
    position: absolute;
    left: 4px;
    color: var(--accent);
    font-size: 13px;
  }
  .insight-list li strong { color: var(--accent-light); font-weight: 600; }
  .insight-list li .timestamp { color: var(--orange); font-size: 12px; margin-left: 4px; }

  .actions-box {
    background: var(--section-bg);
    border-radius: 8px;
    padding: 14px 16px;
    margin-top: 14px;
  }
  .actions-box .actions-title {
    font-size: 12px;
    color: var(--orange);
    font-weight: 600;
    margin-bottom: 8px;
  }
  .actions-box .actions-title::before { content: "⚡ "; }
  .actions-box ol { padding-left: 18px; }
  .actions-box ol li {
    font-size: 13px;
    margin-bottom: 6px;
    color: var(--text);
  }

  /* 趋势雷达 */
  .radar-section {
    background: var(--card);
    border: 1px solid var(--border);
    border-radius: 14px;
    padding: 24px;
    margin-bottom: 20px;
  }
  .radar-section h3 {
    font-size: 15px;
    margin-bottom: 12px;
    color: var(--accent-light);
  }
  .radar-item {
    display: flex;
    gap: 12px;
    padding: 10px 0;
    border-bottom: 1px solid var(--border);
  }
  .radar-item:last-child { border-bottom: none; }
  .radar-item .signal {
    font-size: 10px;
    padding: 2px 8px;
    border-radius: 20px;
    font-weight: 600;
    white-space: nowrap;
    height: fit-content;
    margin-top: 2px;
  }
  .signal-hot { background: rgba(248,113,113,0.15); color: var(--red); }
  .signal-rising { background: rgba(74,222,128,0.15); color: var(--green); }
  .signal-watch { background: rgba(251,146,60,0.15); color: var(--orange); }
  .radar-item .radar-text { font-size: 13px; }
  .radar-item .radar-text strong { color: var(--accent-light); }

  /* 时间线 */
  .timeline {
    position: relative;
    padding-left: 24px;
  }
  .timeline::before {
    content: "";
    position: absolute;
    left: 6px;
    top: 4px;
    bottom: 4px;
    width: 2px;
    background: var(--border);
  }
  .timeline-item {
    position: relative;
    padding-bottom: 20px;
  }
  .timeline-item::before {
    content: "";
    position: absolute;
    left: -22px;
    top: 6px;
    width: 10px;
    height: 10px;
    border-radius: 50%;
    background: var(--accent);
    border: 2px solid var(--bg);
  }
  .timeline-item .time {
    font-size: 11px;
    color: var(--text-muted);
  }
  .timeline-item .event {
    font-size: 13px;
    margin-top: 2px;
  }
  .timeline-item .event strong { color: var(--accent-light); }

  /* 金句卡片 */
  .quote-card {
    background: linear-gradient(135deg, #fffdf9 0%, #f7f1e8 100%);
    border: 1px solid var(--border);
    border-radius: 12px;
    padding: 20px 24px;
    margin-bottom: 16px;
    position: relative;
  }
  .quote-card::before {
    content: "❝";
    font-size: 32px;
    color: var(--accent);
    opacity: 0.3;
    position: absolute;
    top: 8px;
    left: 14px;
  }
  .quote-card .quote-text {
    font-size: 15px;
    font-style: italic;
    padding-left: 24px;
    margin-bottom: 8px;
    color: var(--text);
  }
  .quote-card .quote-author {
    font-size: 12px;
    color: var(--text-muted);
    padding-left: 24px;
  }

  /* 优先级 */
  .priority-list {
    display: flex;
    flex-direction: column;
    gap: 10px;
  }
  .priority-item {
    display: flex;
    align-items: center;
    gap: 12px;
    background: var(--card);
    border: 1px solid var(--border);
    border-radius: 10px;
    padding: 12px 16px;
  }
  .priority-item .rank {
    width: 28px;
    height: 28px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 14px;
    font-weight: 700;
    flex-shrink: 0;
  }
  .rank-1 { background: var(--accent); color: #fff; }
  .rank-2 { background: var(--tag-bg); color: var(--accent-light); border: 1px solid var(--accent); }
  .rank-3 { background: var(--tag-bg); color: var(--text-muted); border: 1px solid var(--border); }
  .priority-item .p-text { font-size: 13px; }
  .priority-item .p-text strong { color: var(--accent-light); }
  .footer {
    text-align: center;
    padding: 28px 0 8px;
    font-size: 12px;
    color: var(--text-muted);
  }
  .footer hr { border: none; border-top: 1px solid var(--border); margin-bottom: 16px; }

  @media (max-width: 600px) {
    .video-card .card-header { flex-direction: column; }
    .video-card .thumb { width: 100%; height: 80px; }
    .stats-bar { flex-direction: column; }
  }

</style>
<div class="weekly-report">
<div class="report-header">
  <h1>AI Native 组织变革周报</h1>
  <div class="meta">
    <span>📅 2026年7月3日（周三）</span>
    <span>📊 第1期</span>
    <span>🎬 9 条精选内容</span>
  </div>
</div>

<!-- 统计栏 -->
<div class="stats-bar">
  <div class="stat-card">
    <div class="num">9</div>
    <div class="label">精选视频/访谈</div>
  </div>
  <div class="stat-card">
    <div class="num">4</div>
    <div class="label">CEO/CXO 级分享</div>
  </div>
  <div class="stat-card">
    <div class="num">6</div>
    <div class="label">企业落地案例</div>
  </div>
  <div class="stat-card">
    <div class="num">14</div>
    <div class="label">可执行行动建议</div>
  </div>
</div>

<!-- 趋势雷达 -->
<div class="section-title">
  趋势雷达 <span class="badge">本周信号</span>
</div>
<div class="radar-section">
  <div class="radar-item">
    <span class="signal signal-hot">🔥 热门</span>
    <div class="radar-text"><strong>Agent Harness 成为共识关键词</strong> — Aaron Levie（Box）与 Harrison Chase（LangChain）共同提出企业需要的不是单个聊天机器人，而是整合权限、内容、审计、人工确认的"Agent 工作台"。</div>
  </div>
  <div class="radar-item">
    <span class="signal signal-hot">🔥 热门</span>
    <div class="radar-text"><strong>大厂从"卖工具"转向"帮转型"</strong> — Microsoft 动员 6000 人新部门帮企业客户落地 AI，Palantir CEO 批评 AI 销售方式"完全出了问题"，企业 AI 价值链正在重组。</div>
  </div>
  <div class="radar-item">
    <span class="signal signal-rising">📈 上升</span>
    <div class="radar-text"><strong>"Agent Crews / Agent 工厂"模式</strong> — Groupon 提出 AI Factory 概念，用统一底座+分散创新让全员成为 builder，不再是 IT 部门专利。</div>
  </div>
  <div class="radar-item">
    <span class="signal signal-rising">📈 上升</span>
    <div class="radar-text"><strong>人才模型从 T 型到圆型</strong> — Nebius CTO 提出工程师需具备多深度专长+系统级理解力，纯执行型硬技能正在贬值。</div>
  </div>
  <div class="radar-item">
    <span class="signal signal-watch">👀 观察</span>
    <div class="radar-text"><strong>90% Agent 卡在试点</strong> — 多位嘉宾共识：瓶颈不在技术而在变革管理、部门壁垒和"像管理员工一样管理 Agent"的治理能力。</div>
  </div>
  <div class="radar-item">
    <span class="signal signal-watch">👀 观察</span>
    <div class="radar-text"><strong>AI 成熟度三阶段模型</strong> — 日本论坛提出 AI 1.0（个人提效）→ AI 2.0（标准流程）→ AI 3.0（决策自我维护），大部分企业仍停留在 1.0。</div>
  </div>
</div>

<!-- 本周金句 -->
<div class="section-title">
  本周金句 <span class="badge">值得引用</span>
</div>
<div class="quote-card">
  <div class="quote-text">如果每个知识工作者都能调用无限"工程能力"，组织形态、岗位定义、管理方式会怎样改变？</div>
  <div class="quote-author">— Aaron Levie, CEO of Box（与 Harrison Chase 对谈，LangChain 频道）</div>
</div>
<div class="quote-card">
  <div class="quote-text">AI 转型最难的跟技术无关。是打破人的部门壁垒，以及学会像管理员工一样管理 Agent。</div>
  <div class="quote-author">— Akshit Kandi, CEO of SkySync（Executives Unplugged 频道）</div>
</div>
<div class="quote-card">
  <div class="quote-text">AI Agent 就像一个初级工程师——需要明确指令、需要审查输出、需要引导方向。把它当成资深工程师来用会导致灾难。</div>
  <div class="quote-author">— Danila Shtan, CTO of Nebius（Beyond Coding 频道）</div>
</div>
<div class="quote-card">
  <div class="quote-text">未来公司只剩两种人：builder 和 seller，中层全被砍。</div>
  <div class="quote-author">— Nick Hsu, 前小红书工程师（塞掐 Side Chat E412）</div>
</div>

<!-- Part 1: 深度访谈 -->
<div class="section-title">
  1. 本期大咖深度访谈/核心观点提炼 <span class="badge">4 条</span>
</div>

<!-- 访谈一 -->
<div class="video-card">
  <div class="card-header">
    <div class="thumb">🎬 31分钟</div>
    <div class="card-meta">
      <h3><a href="https://www.youtube.com/watch?v=agSRMrhNTf4" target="_blank">Why Enterprise AI Adoption Is Slower Than You Think</a></h3>
      <div class="info-line">
        <span class="channel">LangChain</span>
        <span class="views">4,081次观看</span>
        <span>7天前</span>
      </div>
    </div>
  </div>
  <div class="speaker-box">
    <span class="label">核心分享人:</span> Aaron Levie（Box CEO）× Harrison Chase（LangChain 联合创始人兼 CEO）
  </div>
  <div class="tags">
    <span class="tag">Agent Harness</span>
    <span class="tag">知识工作 Agent</span>
    <span class="tag">权限治理</span>
    <span class="tag">Jevons 悖论</span>
    <span class="tag">Token 成本</span>
  </div>
  <ul class="insight-list">
    <li><strong>编程 Agent 与知识工作 Agent 的根本差异</strong>：编程 Agent 成功是因为代码世界高度结构化（代码库、测试、CI/CD、Issue 追踪），知识工作 Agent 面对的是散落在文档/邮件/表格/SaaS 系统里的"非结构化组织记忆"。<span class="timestamp">3:28</span></li>
    <li><strong>"Agent Harness"概念</strong>：企业真正需要的不是聊天机器人，而是整合模型、企业内容检索、权限控制、工具调用、审计、人工确认的"Agent 工作台"。Box 正围绕企业文件系统构建自己的 Harness。<span class="timestamp">12:05</span></li>
    <li><strong>权限是知识工作 Agent 核心瓶颈</strong>：Agent 继承了人类员工的权限复杂度——谁能看哪些文件、能编辑哪些系统、能审批哪些流程，企业里高度定制化。不能精确管理权限就无法进入工作流。<span class="timestamp">7:40</span></li>
    <li><strong>"AI Forward-Deployed Engineers"新角色</strong>：未来企业内部出现既懂业务流程又能把 Agent 嵌入岗位工作流的新型人才，类似 Palantir forward-deployed 模式但面向内部。<span class="timestamp">10:44</span></li>
    <li><strong>Headless vs In-Product 的 Jevons 悖论</strong>：Agent 做成 headless（后台无界面运行）可能比产品内聊天框驱动更多使用量，因为可嵌入任何系统任何流程。<span class="timestamp">15:04</span></li>
    <li><strong>Deep Agents 应构建在编程 Harness 之上</strong>：Harrison 提出即使知识工作 Agent 底层也应有类似编程 Agent 的迭代、测试、验证机制。<span class="timestamp">20:31</span></li>
    <li><strong>Token 成本与企业 EPS 压力</strong>：企业需像管理云成本一样管理 AI 推理成本，单模型 vs 多模型 Harness 的 token 成本差异直接影响每股收益。<span class="timestamp">28:39</span></li>
  </ul>
  <div class="actions-box">
    <div class="actions-title">实践启发</div>
    <ol>
      <li>不要从"给每人聊天机器人"开始，应从高频知识流程切入（合同审阅、客户资料整理、研发文档沉淀），有明确验收标准和可衡量 ROI。</li>
      <li>HR/组织侧可提前设计"Agent 权限矩阵"：哪些岗位的 Agent 可读取哪些系统、执行哪些动作、哪些必须人工确认——本质是组织治理问题。</li>
    </ol>
  </div>
</div>

<!-- 访谈二 -->
<div class="video-card">
  <div class="card-header">
    <div class="thumb">🎬 7分钟</div>
    <div class="card-meta">
      <h3><a href="https://www.youtube.com/watch?v=EKhA9oRC6yg" target="_blank">Microsoft Shifts Strategy on Enterprise AI</a></h3>
      <div class="info-line">
        <span class="channel">Bloomberg Technology</span>
        <span class="views">2,219次观看</span>
        <span>7小时前</span>
      </div>
    </div>
  </div>
  <div class="speaker-box">
    <span class="label">核心分享人:</span> Judson Althoff（Microsoft 商业业务 CEO）× Ed Ludlow（Bloomberg Technology）
  </div>
  <div class="tags">
    <span class="tag">企业 AI 转型</span>
    <span class="tag">从卖工具到帮转型</span>
    <span class="tag">6000人新部门</span>
    <span class="tag">B2B 价值链重组</span>
  </div>
  <ul class="insight-list">
    <li><strong>6000 人新部门的信号</strong>：Microsoft 动员 6000 名员工组建新部门专门帮助企业客户"真正把 AI 用起来"。瓶颈已从"模型能力"和"工具采购"转向"落地执行和变革管理"。</li>
    <li><strong>从"产品售卖"到"转型伙伴"</strong>：企业客户需要的不只是 Copilot 许可证，而是有人帮他们识别用例、改造流程、培训员工、验证 ROI。这是咨询式、场景式、变革式导入。</li>
    <li><strong>企业 AI 价值链正在重组</strong>：从"工具+许可"变成"工具+流程改造+人才赋能+持续优化"。B2B 软件公司需要更多行业顾问、客户成功经理、AI 架构师，而非传统销售。</li>
    <li><strong>对传统制造/硬件企业的间接启示</strong>：如果 Microsoft 这样的巨头都在为"用不起来"发愁，传统制造/芯片企业的 AI 落地难度更大，需要更有针对性的组织变革策略。</li>
  </ul>
  <div class="actions-box">
    <div class="actions-title">实践启发</div>
    <ol>
      <li>内部推动 AI Native 不宜只做工具培训，应建立"业务场景共创机制"：业务负责人+IT+HR+AI Champion 共同定义试点，以业务结果而非使用人数为成功标准。</li>
      <li>参考 Microsoft 打法，把内部 AI 推广团队定位为"AI 转型办公室"（AI Transformation Office），对业务结果负责而非对系统稳定负责。</li>
    </ol>
  </div>
</div>

<!-- 访谈三 -->
<div class="video-card">
  <div class="card-header">
    <div class="thumb">🎬 CNBC</div>
    <div class="card-meta">
      <h3><a href="https://www.youtube.com/watch?v=0A3sGymV6kY" target="_blank">Palantir CEO Alex Karp: "something has gone completely wrong" with how AI is sold</a></h3>
      <div class="info-line">
        <span class="channel">CNBC Television</span>
        <span class="views">29万次观看</span>
        <span>1天前</span>
      </div>
    </div>
  </div>
  <div class="speaker-box">
    <span class="label">核心分享人:</span> Alex Karp（Palantir CEO）× CNBC Squawk Box
  </div>
  <div class="tags">
    <span class="tag">AI 销售方式</span>
    <span class="tag">Forward-Deployed</span>
    <span class="tag">NVIDIA 合作</span>
    <span class="tag">决策链路</span>
  </div>
  <ul class="insight-list">
    <li><strong>AI 不应被包装成泛化工具</strong>：Karp 核心论点——当前 AI 行业销售方式"完全出了问题"，太多公司把 AI 当概念性平台卖，而非围绕客户真实运营问题交付可衡量结果。</li>
    <li><strong>Palantir × NVIDIA 新合作</strong>：将前沿 AI 模型与 Palantir 企业数据操作系统结合，直接进入客户关键决策链路。</li>
    <li><strong>Forward-Deployed 模式的组织含义</strong>：未来 AI 组织形态更接近"业务作战系统"——人、数据、模型、流程和决策权限被重新组合，而非"IT 交付工具给业务用"。</li>
    <li><strong>AI 价值在"进入决策链路"而非"模型很强"</strong>：企业 AI 应进入供应链、生产、销售、风控、客户响应等核心决策环节，而非 PPT 上的模型跑分。</li>
  </ul>
  <div class="actions-box">
    <div class="actions-title">实践启发</div>
    <ol>
      <li>评估 AI Agent 项目时，不要只看使用人数和调用次数，要看是否改变了核心业务动作的速度、质量或成本。</li>
      <li>对管理层汇报时用"业务结果语言"替代"模型能力语言"：节省多少审批时间、减少多少返工、提升多少客户响应效率。</li>
    </ol>
  </div>
</div>

<!-- 访谈四 -->
<div class="video-card">
  <div class="card-header">
    <div class="thumb">🎬 1小时11分</div>
    <div class="card-meta">
      <h3><a href="https://www.youtube.com/watch?v=BJ92fomIRJM" target="_blank">Agent 該怎麼分工？同樣的 AI 只有不到 1% 的人做得出成果！</a></h3>
      <div class="info-line">
        <span class="channel">INSIDE 硬塞的網路趨勢觀察</span>
        <span class="views">1万次观看</span>
        <span>3天前</span>
      </div>
    </div>
  </div>
  <div class="speaker-box">
    <span class="label">核心分享人:</span> Nick Hsu（前小红书工程师，后转战加密货币交易所，现独立创业者）
  </div>
  <div class="tags">
    <span class="tag">30 个 Agent 并行</span>
    <span class="tag">驾驭工程</span>
    <span class="tag">Builder vs Seller</span>
    <span class="tag">AI 泡沫论</span>
    <span class="tag">招聘变革</span>
  </div>
  <ul class="insight-list">
    <li><strong>一次派出 30 个 Agent 同时开发</strong>：Nick 在交易所内部一次性派出 30 个 Agent 并行处理开发任务，半夜自动改好 code。Agent 使用已从"个人提效"进入"团队级编排"阶段。<span class="timestamp">20:59</span></li>
    <li><strong>"驾驭工程"取代"编码工程"</strong>：模型能力已超越资深员工，人核心价值不再是亲自编码而是"驾驭"——拆分任务、定义边界、给上下文、验收结果、管理多 Agent 协作。<span class="timestamp">11:50</span></li>
    <li><strong>"不到 1% 的人做得出成果"的落差</strong>：同样的 AI 工具，大部分人给的是模糊指令，少数人能把模糊问题变成清晰可执行任务链。关键在"问题定义能力"和"任务拆解能力"。</li>
    <li><strong>AI 泡沫论两个面向</strong>：区分"资本价格泡沫"（概念股估值过高）和"实际应用泡沫"（落地效果远低于宣传），两个泡沫可能同时存在但不一定同步破裂。<span class="timestamp">27:06</span></li>
    <li><strong>招聘条件正在被 AI 改变</strong>：Agent 可完成初级工程师工作，招聘标准从"能不能写代码"转向"能不能定义问题、驾驭 Agent、验收质量"。<span class="timestamp">34:49</span></li>
    <li><strong>未来公司只剩 builder 和 seller</strong>：中间管理层如果只做信息传递和进度跟踪，价值会被 Agent 压缩。<span class="timestamp">39:42</span></li>
    <li><strong>生产力翻 10 倍但营收没变？</strong>关键在工作场景还是传统样子——AI 生产力提升必须配合业务场景重塑才能转化为商业价值。<span class="timestamp">44:06</span></li>
    <li><strong>用 AI 重建冲浪学校</strong>：离开交易所后用 AI 从零重建冲浪学校，展示 Agent 不仅适用于科技公司也能赋能线下实体。<span class="timestamp">01:05:55</span></li>
  </ul>
  <div class="actions-box">
    <div class="actions-title">实践启发</div>
    <ol>
      <li>HR 可把"AI 驾驭能力"纳入人才盘点模型：是否会拆解任务、定义验收标准、编排多个 Agent、复盘输出质量——这不是技术能力而是管理能力。</li>
      <li>管理者培训应加入"Agent 分工设计"模块——把团队工作流改造成"人机协作流程"，明确哪些环节 Agent 执行、哪些人决策、哪些人机协同。</li>
    </ol>
  </div>
</div>

<!-- Part 2: 案例 -->
<div class="section-title">
  2. AI 能力建设与效能提升案例 <span class="badge">5 条</span>
</div>

<!-- 案例一 -->
<div class="video-card">
  <div class="card-header">
    <div class="thumb">🎬 50分钟</div>
    <div class="card-meta">
      <h3><a href="https://www.youtube.com/watch?v=pQj8qOyan-Q" target="_blank">Building the AI-Native Enterprise, Agent Crews and the AI Factory</a></h3>
      <div class="info-line">
        <span class="channel">Augmented U</span>
        <span class="views">513次观看</span>
        <span>5小时前</span>
      </div>
    </div>
  </div>
  <div class="speaker-box">
    <span class="label">核心分享人:</span> Masha Sharma（Groupon VP of Merchant Experience AI，25年技术全栈经验，曾担任工程师/创始人/CTO/产品负责人/高管）
  </div>
  <div class="tags">
    <span class="tag">AI Native 2027</span>
    <span class="tag">Agent Crews</span>
    <span class="tag">AI Factory</span>
    <span class="tag">全员 Builder</span>
    <span class="tag">Compliance Agent</span>
    <span class="tag">Truth-Layer RAG</span>
  </div>
  <ul class="insight-list">
    <li><strong>Groupon 的 AI Native 2027 目标</strong>：公司级战略目标——2027 年成为 AI 原生公司。AI Native 不是"用了一些 AI 工具"，而是让每个职能都具备持续构建 AI 工作流的能力。<span class="timestamp">6:19</span></li>
    <li><strong>集中治理 vs 团队赋能的平衡</strong>：选择"统一底座+分散创新"——统一安全规则、评估框架、数据架构，但允许业务团队快速孵化场景。<span class="timestamp">8:36</span></li>
    <li><strong>Build vs Buy 决策已改变</strong>：AI 能力变化太快，买成品可能 3 个月过时，但完全自建又跟不上模型迭代。Groupon 有系统化的决策框架。<span class="timestamp">10:40</span></li>
    <li><strong>AI 产物审查机制</strong>：当所有人都能用 AI 构建工作流，需建立 AI 产物审查流程确保产出质量符合业务标准。<span class="timestamp">18:09</span></li>
    <li><strong>商家体验 AI 改造</strong>：AI 驱动的交易生成、商家智能层、商家自助入驻和合规 Agent Crews。<span class="timestamp">19:53</span></li>
    <li><strong>Compliance Agent Crews</strong>：专门的合规 Agent 团队自动处理商户入驻合规审查、资质验证、风险筛查，从人工流程转为 Agent 驱动。<span class="timestamp">24:22</span></li>
    <li><strong>Truth-Layer RAG 系统</strong>：Agent 生成内容前先检索经验证的企业知识库，减少幻觉风险。</li>
    <li><strong>用例优先级排序方法</strong>：综合考虑业务影响、技术可行性、数据准备度和变革难度，而非"哪个最酷"。<span class="timestamp">25:38</span></li>
    <li><strong>Human-in-the-Loop vs 全自主</strong>：根据风险等级和可逆性决定哪些环节需要人工确认，哪些可全自主运行。<span class="timestamp">39:09</span></li>
    <li><strong>"Ship Small 胜过 Analysis Paralysis"</strong>：宁可快速发布小版本快速迭代，也不要在分析阶段停滞。AI 发展太快，等分析完美时机会已过。</li>
    <li><strong>"Become a Builder Today"</strong>：今天就开始用 AI 构建东西，哪怕很小的工作流。AI Native 不是规划出来的，是实践出来的。<span class="timestamp">49:07</span></li>
  </ul>
  <div class="actions-box">
    <div class="actions-title">实践启发</div>
    <ol>
      <li>建立"AI Factory"机制：统一底座（模型、安全、评估）+ 统一门户（所有人可申请构建 Agent），但允许业务团队快速孵化场景——类似内部创业孵化器。</li>
      <li>设计"人人成为 Builder"的能力地图：第一层基础提示词 → 第二层流程拆解和任务编排 → 第三层低代码/Agent 构建 → 第四层 AI 输出审核和治理。</li>
    </ol>
  </div>
</div>

<!-- 案例二 -->
<div class="video-card">
  <div class="card-header">
    <div class="thumb">🎬 17分钟</div>
    <div class="card-meta">
      <h3><a href="https://www.youtube.com/watch?v=RkfKNLKO-2k" target="_blank">AI writes the code. Who ships it? (Harness Autonomous Worker Agents)</a></h3>
      <div class="info-line">
        <span class="channel">The New Stack</span>
        <span class="views">107次观看</span>
        <span>2天前</span>
      </div>
    </div>
  </div>
  <div class="speaker-box">
    <span class="label">核心分享人:</span> Jyoti Bansal（Harness 创始人兼 CEO，此前创立 AppDynamics 并成功上市退出）
  </div>
  <div class="tags">
    <span class="tag">Autonomous Worker Agents</span>
    <span class="tag">软件交付流水线</span>
    <span class="tag">安全护栏</span>
    <span class="tag">Agent Marketplace</span>
  </div>
  <ul class="insight-list">
    <li><strong>Agent 在生产环境运行是"完全不同的野兽"</strong>：让 Agent 在开发环境写代码是一回事，在生产交付流水线自主运行是另一回事——前者出错可重来，后者出错可能生产事故。<span class="timestamp">3:58</span></li>
    <li><strong>Harness 四阶段演进</strong>：可靠部署 → 专家 Agent 和知识图谱 → Autonomous Worker Agents → 从 Jira Ticket 到生产全自主愿景。<span class="timestamp">0:00</span></li>
    <li><strong>把流水线每步从固定脚本变成"推理 Agent"</strong>：部署、测试、安全扫描、合规检查不再是 if-else，而是根据上下文推理决策。</li>
    <li><strong>安全护栏五要素</strong>：(1) 沙箱隔离 (2) 作用域身份/最小权限 (3) 策略强制 (4) 审计追踪 (5) 成本上限。<span class="timestamp">5:27</span></li>
    <li><strong>United Airlines Hackathon 案例</strong>：非科技公司也能在 Hackathon 中快速构建可用生产级 Agent。<span class="timestamp">14:38</span></li>
    <li><strong>Agent Marketplace 信任问题</strong>：社区 Agent 的信任是核心难题——怎么敢让第三方 Agent 操作生产系统？需要新信任验证机制。<span class="timestamp">15:02</span></li>
  </ul>
  <div class="actions-box">
    <div class="actions-title">实践启发</div>
    <ol>
      <li>研发效能提升不能只考核"AI 写了多少代码"，要考核从需求→开发→测试→上线→故障恢复的全链路周期时间。</li>
      <li>设置"AI 代码准入规则"：AI 生成内容必须经过自动化测试、代码审查、安全扫描和责任人确认后才能合并。</li>
    </ol>
  </div>
</div>

<!-- 案例三 -->
<div class="video-card">
  <div class="card-header">
    <div class="thumb">🎬 David Senra</div>
    <div class="card-meta">
      <h3><a href="https://www.youtube.com/watch?v=PYobZzjW_ic" target="_blank">The Future of Software & AI | Cognition's Scott Wu</a></h3>
      <div class="info-line">
        <span class="channel">David Senra</span>
        <span class="views">1.8万次观看</span>
        <span>4天前</span>
      </div>
    </div>
  </div>
  <div class="speaker-box">
    <span class="label">核心分享人:</span> Scott Wu（Cognition 联合创始人兼 CEO，Devin 背后团队。Cognition 2026年5月估值 260 亿美元，年化收入从 100 万→7300 万美元）
  </div>
  <div class="tags">
    <span class="tag">Devin AI 工程师</span>
    <span class="tag">企业部署</span>
    <span class="tag">ROI 衡量</span>
    <span class="tag">Model-Neutral</span>
    <span class="tag">长期自主 Agent</span>
  </div>
  <ul class="insight-list">
    <li><strong>Devin 的企业部署实况</strong>：不是简单卖工具，而是深入客户现场理解开发流程、代码库结构、协作方式，定制 Agent 工作模式。与 Palantir forward-deployed 模式异曲同工。<span class="timestamp">42:41</span></li>
    <li><strong>"衡量 ROI 而不是 Token 消耗"</strong>：关键指标不是 token 花了多少，而是节省了多少工程师时间、加速了多少交付周期、减少了多少外包成本。<span class="timestamp">48:34</span></li>
    <li><strong>Model-Neutral 策略</strong>：不绑定单一模型供应商，根据任务类型选最优模型。Agent 平台层核心竞争力是编排、评估和治理能力，而非模型能力。<span class="timestamp">50:01</span></li>
    <li><strong>"当 Agent 可以连续工作数月"</strong>：Agent 自主工作时间从分钟级扩展到天级甚至月级时，组织管理方式需根本性变革——不能像管理人的任务一样管理数字员工。<span class="timestamp">22:57</span></li>
    <li><strong>从"AI 辅助编码"到"AI 承担完整工程任务"</strong>：Devin 不是 Copilot 式代码补全，而是独立承接完整工程任务——理解需求、设计方案、编写代码、运行测试、修复 Bug、提交 PR。</li>
    <li><strong>专注让创业公司击败巨头</strong>：巨头同时做一百件事，创业公司只做一件事做到极致。<span class="timestamp">52:18</span></li>
  </ul>
  <div class="actions-box">
    <div class="actions-title">实践启发</div>
    <ol>
      <li>企业试点研发 Agent 时，选择边界清晰、验收明确的任务：修复低中复杂度 Bug、补测试用例、迁移脚本、文档更新。不要一开始就负责核心架构设计。</li>
      <li>重新定义工程师能力模型四层：(1) 能使用 AI 编码 (2) 能审查 AI 输出 (3) 能设计 AI 工作流 (4) 能治理 AI 系统——四层能力应区别培养。</li>
    </ol>
  </div>
</div>

<!-- 案例四 -->
<div class="video-card">
  <div class="card-header">
    <div class="thumb">🎬 58分钟</div>
    <div class="card-meta">
      <h3><a href="https://www.youtube.com/watch?v=zTenuG5b4Eo" target="_blank">Only Hundreds of Engineers Have This Skill (Nebius CTO)</a></h3>
      <div class="info-line">
        <span class="channel">Beyond Coding</span>
        <span class="views">1万次观看</span>
        <span>1天前</span>
      </div>
    </div>
  </div>
  <div class="speaker-box">
    <span class="label">核心分享人:</span> Danila Shtan（Nebius CTO，Nebius 是全球最大 AI 云之一，提供 AI 训练和推理基础设施）
  </div>
  <div class="tags">
    <span class="tag">稀缺工程技能</span>
    <span class="tag">T型→圆型工程师</span>
    <span class="tag">面试禁用 AI</span>
    <span class="tag">禁止 Claude Code</span>
    <span class="tag">AI 代码合并规则</span>
  </div>
  <ul class="insight-list">
    <li><strong>"AI Agent 能做一切"是谎言</strong>：Agent 在特定场景强大，但"Agent 能替代所有工程工作"不成立。<span class="timestamp">0:00</span></li>
    <li><strong>最稀缺的技能不是你在卷的</strong>：全球只有几百人真正掌握的不是编程语言或框架，而是对复杂系统的深度理解——分布式系统、网络协议、编译器、操作系统层面的架构判断。<span class="timestamp">4:31</span></li>
    <li><strong>面试中禁止使用 AI</strong>：要评估候选人的真实理解深度而非 AI 辅助下的表现。关键人才选拔中"裸能力"仍重要。<span class="timestamp">10:51</span></li>
    <li><strong>禁止使用"Headcount"这个词</strong>：应用"能力"和"产出"衡量团队而非人数——AI 让一个人产出等于过去十个人。<span class="timestamp">16:31</span></li>
    <li><strong>Agent = 初级工程师</strong>：需要明确指令、需审查输出、需引导方向。当资深工程师来用会导致灾难。<span class="timestamp">35:32</span></li>
    <li><strong>禁止团队用 Claude Code + AI 代码合并规则</strong>：AI 生成代码必须经人审查、理解每行代码含义后才能合并。不是排斥 AI 而是确保质量和安全。<span class="timestamp">36:57</span></li>
    <li><strong>从 T 型到圆型工程师</strong>：从"一个深度专长+广泛基础"演变为"多个深度专长+系统级理解力+跨领域沟通力"。<span class="timestamp">42:32</span></li>
    <li><strong>将会被淘汰的工程师</strong>：只会按指令执行、不理解系统全局、不主动思考问题的工程师会被淘汰。能存活的是把 AI 当工具放大判断力的人。<span class="timestamp">47:11</span></li>
  </ul>
  <div class="actions-box">
    <div class="actions-title">实践启发</div>
    <ol>
      <li>人才发展不应把 AI 培训做成工具课，应做成"问题定义+系统思考+技术判断+AI 协作"的综合能力训练。</li>
      <li>建立新的人才分层：(1) 能使用 AI 完成明确任务 (2) 能审查和修正 AI 输出 (3) 能设计 AI 工作流和评估框架 (4) 能治理 AI 系统和安全——四类能力区别培养、定级。</li>
    </ol>
  </div>
</div>

<!-- 案例五 -->
<div class="video-card">
  <div class="card-header">
    <div class="thumb">🎬 18分钟</div>
    <div class="card-meta">
      <h3><a href="https://www.youtube.com/watch?v=AdxhVilgxhU" target="_blank">Why 90% of AI Agents Are Stuck in a Pilot</a></h3>
      <div class="info-line">
        <span class="channel">Executives Unplugged</span>
        <span class="views">18次观看</span>
        <span>2天前</span>
      </div>
    </div>
  </div>
  <div class="speaker-box">
    <span class="label">核心分享人:</span> Akshit Kandi（SkySync CEO，曾指导超 100 家创业公司，此前在 Salesforce Agentforce 平台构建 Agent）
  </div>
  <div class="tags">
    <span class="tag">90% 卡在试点</span>
    <span class="tag">变革管理</span>
    <span class="tag">Agent 岗位说明书</span>
    <span class="tag">进攻 vs 防御心态</span>
    <span class="tag">ROI 仪表盘</span>
  </div>
  <ul class="insight-list">
    <li><strong>AI 转型最难的跟技术无关</strong>：最大瓶颈不是技术，而是打破人的部门壁垒和学会像管理员工一样管理 Agent。</li>
    <li><strong>"像管理员工一样管理 Agent"</strong>：Agent 需要明确岗位描述、绩效指标、工作边界、汇报关系——和人一样。不知道怎么评估 Agent"绩效"就还没准备好部署。<span class="timestamp">2:22</span></li>
    <li><strong>300% 增长案例</strong>：一个客户仅用一个营销 Agent 就实现新业务 300% 增长。关键不是 Agent 多聪明，而是被正确嵌入销售流程瓶颈环节。<span class="timestamp">3:45</span></li>
    <li><strong>变革管理才是真正瓶颈</strong>：技术部署可能只需 2 周，但让团队接受、适应、善用新工作流可能需 2-6 个月。大多数项目失败在这一阶段。<span class="timestamp">6:55</span></li>
    <li><strong>进攻 vs 防御心态</strong>：成功企业用"进攻心态"（如何用 AI 创造新价值），失败企业用"防御心态"（如何用 AI 防止被淘汰）。前者驱动创新，后者只驱动恐惧。<span class="timestamp">9:30</span></li>
    <li><strong>先从内部 Agent 开始</strong>：先部署面向员工的内部 Agent，再部署面向客户的外部 Agent。内部出错影响可控，可快速学习迭代。<span class="timestamp">23:50</span></li>
    <li><strong>从会议记录和现有系统挖掘 Agent 场景</strong>：分析会议记录、邮件线程、工单系统，找出重复出现、流程化程度高、耗时长但价值低的任务。<span class="timestamp">26:52</span></li>
    <li><strong>ROI 仪表盘：衡量 Token 使用而非最大化</strong>：不要追求"用最多 Token"，要衡量"每个 Token 创造多少价值"。追踪业务指标而非技术指标。<span class="timestamp">29:42</span></li>
  </ul>
  <div class="actions-box">
    <div class="actions-title">实践启发</div>
    <ol>
      <li>部署 Agent 前先写"Agent 岗位说明书"——明确解决什么问题、汇报给谁、绩效指标是什么、出错时谁负责。和招聘新员工流程一样。</li>
      <li>用"进攻心态"驱动 AI 转型——不要从"怎么省人"开始，从"怎么创造以前不可能的能力"开始。前者让团队恐惧，后者让团队兴奋。</li>
    </ol>
  </div>
</div>

<!-- 案例六 -->
<div class="video-card">
  <div class="card-header">
    <div class="thumb">🎬 21分钟</div>
    <div class="card-meta">
      <h3><a href="https://www.youtube.com/watch?v=lex4jtFyRlA" target="_blank">客服 AI Agent 理論與應用的轉型之路 | TO Talk EP132</a></h3>
      <div class="info-line">
        <span class="channel">TechOrange 科技報橘</span>
        <span class="views">64次观看</span>
        <span>16小时前</span>
      </div>
    </div>
  </div>
  <div class="speaker-box">
    <span class="label">核心分享人:</span> Satoshi Okuda（早稻田大学副教授）× Hiroshi Nishikawa（MoBagel 日本区总经理）× 苏盈诚（勤业众信管理顾问协理）
  </div>
  <div class="tags">
    <span class="tag">日本企业 AI</span>
    <span class="tag">AI 1.0/2.0/3.0</span>
    <span class="tag">工程师缺工</span>
    <span class="tag">地端 AI 部署</span>
    <span class="tag">信用评分 AI</span>
  </div>
  <ul class="insight-list">
    <li><strong>三菱日联信用评分 AI</strong>：日本最大金融集团已在信用评分环节部署 AI Agent，不只是自动化审批而是让 AI 参与风险评估决策。<span class="timestamp">1:05</span></li>
    <li><strong>地端 AI 风险管理</strong>：出于数据安全和合规要求，日本银行选择地端部署而非云端。对保守文化企业有直接参考价值。<span class="timestamp">3:16</span></li>
    <li><strong>AI 缓解日本 IT 工程师缺工</strong>：不是替代现有工程师，而是把稀缺专家经验产品化、流程化、可复制化，让非专家也能完成部分工程工作。<span class="timestamp">10:03</span></li>
    <li><strong>AI 成熟度三阶段模型</strong>：AI 1.0（个人提示词提效）→ AI 2.0（嵌入标准流程和组织系统）→ AI 3.0（决策与营运自我维护的自主 Agent）。大部分企业还停留在 1.0。<span class="timestamp">14:49</span></li>
    <li><strong>AI 3.0 的终极形态</strong>：Agent 自主监控运营指标、发现异常、提出决策建议甚至自主执行优化——要求极高数据质量、流程标准化和治理成熟度。<span class="timestamp">19:10</span></li>
  </ul>
  <div class="actions-box">
    <div class="actions-title">实践启发</div>
    <ol>
      <li>客服、HRSSC、IT Helpdesk 等共享服务场景适合作为 AI Agent 先行区——流程高频、知识可沉淀、反馈闭环快、出错影响可控。</li>
      <li>推进时先做"标准流程 AI 2.0"：把 FAQ、SOP、工单规则、升级机制结构化，再谈更高阶自主决策。跳过 2.0 直接做 3.0 会因数据质量和流程不成熟而失败。</li>
    </ol>
  </div>
</div>

<!-- 本周优先观看 -->
<div class="section-title">
  本周优先观看建议 <span class="badge">Top 3</span>
</div>
<div class="priority-list">
  <div class="priority-item">
    <div class="rank rank-1">1</div>
    <div class="p-text"><strong>Masha Sharma（Groupon）</strong>— 最完整的 AI Native 组织建设实战案例，涵盖治理、场景、技术架构、人才赋能全链路。<a href="https://www.youtube.com/watch?v=pQj8qOyan-Q" target="_blank" style="color:var(--accent);font-size:12px;">→ 观看</a></div>
  </div>
  <div class="priority-item">
    <div class="rank rank-2">2</div>
    <div class="p-text"><strong>Aaron Levie + Harrison Chase</strong>— 最适合理解企业 AI Agent 落地的结构性瓶颈和"Agent Harness"核心概念。<a href="https://www.youtube.com/watch?v=agSRMrhNTf4" target="_blank" style="color:var(--accent);font-size:12px;">→ 观看</a></div>
  </div>
  <div class="priority-item">
    <div class="rank rank-3">3</div>
    <div class="p-text"><strong>Danila Shtan（Nebius CTO）</strong>— 对人才能力模型变革最有启发的硬核视角，适合驱动内部人才盘点和能力重塑讨论。<a href="https://www.youtube.com/watch?v=zTenuG5b4Eo" target="_blank" style="color:var(--accent);font-size:12px;">→观看</a></div>
  </div>
</div>

<div class="footer">
  <hr>
  <p>AI Native 组织变革周报 · 由 Hermes Agent 自动生成</p>
  <p>数据来源：YouTube 公开视频 · 仅供学习参考</p>
</div>
</div>
{{< /rawhtml >}}
