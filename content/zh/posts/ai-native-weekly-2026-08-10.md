---
title: "AI Native 组织变革周报 - 2026年8月10日"
slug: "ai-native-weekly-2026-08-10"
date: 2026-08-10T15:00:00+08:00
draft: false
disableToc: true
hideMeta: true
fullWidth: true
categories: ["ai-native"]
tags: ["ai-native-weekly", "AI Native", "组织变革", "Token预算", "Agent安全", "Demo到产品"]
description: "第8期：Ramp宣布不设token预算，反AI叙事首次获得主流放大，公司大脑模式出现，Waymo Co-CEO提醒Demo只是1%的工作。"
---

{{< rawhtml >}}
<div class="weekly-report">
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
  .weekly-report { background: var(--bg); color: var(--text); font-family: -apple-system, "PingFang SC", "Microsoft YaHei", "Helvetica Neue", sans-serif; line-height: 1.75; padding: 18px 12px;   }
  .report-header { text-align: center; padding: 28px 20px 20px; background: linear-gradient(135deg, #1a1d27 0%, #16181f 100%); border-radius: 16px; border: 1px solid var(--border); margin-bottom: 10px; }
  .report-header h1 { font-size: 24px; font-weight: 700; margin-bottom: 8px; background: linear-gradient(135deg, #8b6f47, #c47a3a); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }
  .report-header .meta { font-size: 13px; color: var(--text-muted); display: flex; justify-content: center; gap: 16px; flex-wrap: wrap; }
  .report-header .meta span { display: inline-flex; align-items: center; gap: 4px; }
  .stats-bar { display: flex; gap: 12px; margin-bottom: 10px; flex-wrap: wrap; }
  .stat-card { flex: 1; min-width: 140px; background: var(--card); border: 1px solid var(--border); border-radius: 12px; padding: 10px 14px; text-align: center; }
  .stat-card .num { font-size: 28px; font-weight: 700; color: var(--accent-light); }
  .stat-card .label { font-size: 12px; color: var(--text-muted); margin-top: 4px; }
  .section-title { font-size: 18px; font-weight: 700; margin: 24px 0 12px; padding-left: 14px; border-left: 4px solid var(--accent); display: flex; align-items: center; justify-content: space-between; }
  .section-title .badge { font-size: 12px; background: var(--tag-bg); color: var(--tag-text); padding: 2px 10px; border-radius: 20px; font-weight: 400; }
  .video-card { background: var(--card); border: 1px solid var(--border); border-radius: 14px; padding: 18px; margin-bottom: 10px; transition: border-color 0.2s; }
  .video-card:hover { border-color: var(--accent); }
  .video-card .card-header { display: flex; gap: 14px; margin-bottom: 12px; flex-wrap: wrap; }
  .video-card .thumb { width: 120px; height: 68px; border-radius: 8px; background: var(--section-bg); display: flex; align-items: center; justify-content: center; font-size: 11px; color: var(--text-muted); border: 1px solid var(--border); flex-shrink: 0; }
  .video-card .card-meta { flex: 1; min-width: 200px; }
  .video-card h3 { font-size: 15px; font-weight: 600; margin-bottom: 6px; line-height: 1.5; }
  .video-card h3 a { color: var(--text); text-decoration: none; }
  .video-card h3 a:hover { color: var(--accent-light); }
  .video-card .info-line { font-size: 12px; color: var(--text-muted); display: flex; gap: 10px; flex-wrap: wrap; }
  .video-card .info-line .channel { color: var(--accent-light); }
  .video-card .info-line .views { color: var(--green); }
  .speaker-box { background: var(--section-bg); border-radius: 8px; padding: 8px 12px; margin-bottom: 10px; font-size: 13px; }
  .speaker-box .label { color: var(--accent); font-weight: 600; margin-right: 6px; }
  .tags { display: flex; gap: 6px; flex-wrap: wrap; margin-bottom: 10px; }
  .tag { font-size: 11px; background: var(--tag-bg); color: var(--tag-text); padding: 3px 10px; border-radius: 20px; }
  .insight-list { list-style: none; padding: 0; }
  .insight-list li { padding: 8px 0 8px 22px; position: relative; font-size: 14px; border-bottom: 1px solid var(--border); }
  .insight-list li:last-child { border-bottom: none; }
  .insight-list li::before { content: "▸"; position: absolute; left: 4px; color: var(--accent); font-size: 13px; }
  .insight-list li strong { color: var(--accent-light); font-weight: 600; }
  .insight-list li .timestamp { color: var(--orange); font-size: 12px; margin-left: 4px; }
  .actions-box { background: var(--section-bg); border-radius: 8px; padding: 10px 12px; margin-top: 10px; }
  .actions-box .actions-title { font-size: 12px; color: var(--orange); font-weight: 600; margin-bottom: 8px; }
  .actions-box .actions-title::before { content: "⚡ "; }
  .actions-box ol { padding-left: 18px; }
  .actions-box ol li { font-size: 13px; margin-bottom: 6px; color: var(--text); }
  .radar-section { background: var(--card); border: 1px solid var(--border); border-radius: 14px; padding: 18px; margin-bottom: 10px; }
  .radar-section h3 { font-size: 15px; margin-bottom: 12px; color: var(--accent-light); }
  .radar-item { display: flex; gap: 12px; padding: 10px 0; border-bottom: 1px solid var(--border); }
  .radar-item:last-child { border-bottom: none; }
  .radar-item .signal { font-size: 10px; padding: 2px 8px; border-radius: 20px; font-weight: 600; white-space: nowrap; height: fit-content; margin-top: 2px; }
  .signal-hot { background: rgba(184,84,80,0.15); color: var(--red); }
  .signal-rising { background: rgba(90,122,82,0.15); color: var(--green); }
  .signal-watch { background: rgba(196,122,58,0.15); color: var(--orange); }
  .radar-item .radar-text { font-size: 13px; }
  .radar-item .radar-text strong { color: var(--accent-light); }
  .quote-card { background: linear-gradient(135deg, #1a1d27 0%, #16181f 100%); border: 1px solid var(--border); border-radius: 12px; padding: 14px 18px; margin-bottom: 12px; position: relative; }
  .quote-card::before { content: "❝"; font-size: 32px; color: var(--accent); opacity: 0.3; position: absolute; top: 8px; left: 14px; }
  .quote-card .quote-text { font-size: 15px; font-style: italic; padding-left: 24px; margin-bottom: 8px; color: var(--text); }
  .quote-card .quote-author { font-size: 12px; color: var(--text-muted); padding-left: 24px; }
  .priority-list { display: flex; flex-direction: column; gap: 10px; }
  .priority-item { display: flex; align-items: center; gap: 12px; background: var(--card); border: 1px solid var(--border); border-radius: 10px; padding: 10px 14px; }
  .priority-item .rank { width: 28px; height: 28px; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 14px; font-weight: 700; flex-shrink: 0; }
  .rank-1 { background: var(--accent); color: #fff; }
  .rank-2 { background: var(--tag-bg); color: var(--accent-light); border: 1px solid var(--accent); }
  .rank-3 { background: var(--tag-bg); color: var(--text-muted); border: 1px solid var(--border); }
  .priority-item .p-text { font-size: 13px; }
  .priority-item .p-text strong { color: var(--accent-light); }
  .priority-item .p-text a { color: var(--accent); }
  .footer { text-align: center; padding: 21px 0 6px; font-size: 12px; color: var(--text-muted); }
  .footer hr { border: none; border-top: 1px solid var(--border); margin-bottom: 12px; }
  @media (max-width: 600px) { .video-card .card-header { flex-direction: column; } .video-card .thumb { width: 100%; height: 80px; } .stats-bar { flex-direction: column; } }

</style>
<div class="report-header">
  <h1>AI Native 组织变革周报</h1>
  <div class="meta">
    <span>📅 2026年8月10日（周六）</span>
    <span>📊 第8期</span>
    <span>🎬 10 条精选内容</span>
  </div>
</div>

<div class="stats-bar">
  <div class="stat-card"><div class="num">10</div><div class="label">精选视频/访谈</div></div>
  <div class="stat-card"><div class="num">4</div><div class="label">CEO/CXO 级分享</div></div>
  <div class="stat-card"><div class="num">6</div><div class="label">企业落地案例</div></div>
  <div class="stat-card"><div class="num">18</div><div class="label">可执行行动建议</div></div>
</div>

<!-- 趋势雷达 -->
<div class="section-title">趋势雷达 <span class="badge">本周信号</span></div>
<div class="radar-section">
  <div class="radar-item">
    <span class="signal signal-hot">🔥 热门</span>
    <div class="radar-text"><strong>"不设 token 预算"成为新激进实验</strong> — Ramp 工程团队公开宣布"工程师不设 token 预算"，与第5期 Ryan Carson 的"5000美元/月/人"形成鲜明对比。两种模式代表了 Agent 落地的两种哲学：成本控制型 vs 产出最大化型。Ramp 的逻辑是"省下的人力成本远超 token 费用"。</div>
  </div>
  <div class="radar-item">
    <span class="signal signal-hot">🔥 热门</span>
    <div class="radar-text"><strong>反 AI 叙事首次获得主流平台放大</strong> — Financial Times 记者 Sarah O'Connor 新书《We Are Not Machines》系统反驳"AI 解放工作"叙事。她用 Amazon 仓库、瑞典矿山、医院和翻译公司的实地调查证明：AI 正在让很多员工"被机器管理"而非"被机器解放"。这是本周最重要的反面声音。</div>
  </div>
  <div class="radar-item">
    <span class="signal signal-rising">📈 上升</span>
    <div class="radar-text"><strong>"公司大脑"（Company Brain）模式出现</strong> — Steph France 展示了一个电商团队用 Discord+Slack 运行一个共享 AI Agent（"公司大脑"）的真实案例。Agent 拥有所有部门知识、自主处理 HR 和客服、团队每天通过聊天与它协作。这可能是中小企业 AI Native 化的最简路径。</div>
  </div>
  <div class="radar-item">
    <span class="signal signal-rising">📈 上升</span>
    <div class="radar-text"><strong>"Demo 只是1%的工作"成为 Agent 落地共识</strong> — Waymo Co-CEO 在 Y Combinator 的分享引发共鸣："Demo 到产品之间是15年的距离"。这与第1期 Aaron Levie "90% Agent 卡在试点"、第2期 Barclays "安全失败比能做出来更重要"形成三重验证——Agent 从 Demo 到生产的鸿沟是行业最大瓶颈。</div>
  </div>
  <div class="radar-item">
    <span class="signal signal-watch">👀 观察</span>
    <div class="radar-text"><strong>HR 领域 AI 应用出现两个方向分化</strong> — 方向一：Workhuman CEO 提出"用 AI 挖掘传统 HR 系统忽视的隐性领导力"（AI 增强人）；方向二：GTIA 讨论"AI Agent 重塑岗位本身"（AI 替代任务）。HR 领导者需要同时关注两个方向。</div>
  </div>
  <div class="radar-item">
    <span class="signal signal-watch">👀 观察</span>
    <div class="radar-text"><strong>F1 赛车成为"高压 Agent 落地"的试验场</strong> — VCARB CEO 分享 F1 团队如何用 Agent"Toro"将百万级实时数据点转化为对话式洞察。F1 代表了"毫秒级决策+海量数据+高压环境"的极端场景，其 Agent 落地经验对制造业和半导体行业有直接参考价值。</div>
  </div>
  <div class="radar-item">
    <span class="signal signal-watch">👀 观察</span>
    <div class="radar-text"><strong>AI Agent 安全事件从技术议题升级为治理议题</strong> — BBC Newscast 深度讨论 AI Agent"越狱"事件，6章节涵盖"模型是否真的在失控"到"对普通人和AI治理意味着什么"。AI Agent 安全已不再是 CTO 的问题，而是董事会和 CEO 的问题。</div>
  </div>
</div>

<!-- 本周金句 -->
<div class="section-title">本周金句 <span class="badge">值得引用</span></div>
<div class="quote-card">
  <div class="quote-text">Demo 只是1%的工作。Waymo 的第一个自动驾驶 Demo 用了18个月，但产品花了15年。可靠性的提升是一条指数曲线——你必须在曲线上坚持足够久。</div>
  <div class="quote-author">— Dmitri Dolgov, Waymo Co-CEO（Y Combinator Startup School 2026）</div>
</div>
<div class="quote-card">
  <div class="quote-text">我们不给工程师设 token 预算。省下来的人力成本远远超过 token 费用。限制 token 就是限制产出。</div>
  <div class="quote-author">— Rahul Sengottuvelu & Austin Ray, Ramp 工程团队（Claude 频道）</div>
</div>
<div class="quote-card">
  <div class="quote-text">AI 不是在消灭工作，而是在把人变成机器。很多员工感觉被算法管理，而不是被AI赋能——这才是真正的问题。</div>
  <div class="quote-author">— Sarah O'Connor, Financial Times 记者/《We Are Not Machines》作者（Info-Tech Research Group）</div>
</div>
<div class="quote-card">
  <div class="quote-text">文化先于代码。在数字化转型之前，你必须先建立"不甩锅、不废话、坦诚"的文化——否则再好的技术也救不了你。</div>
  <div class="quote-author">— Peter Bayer, VCARB CEO（Pascal Bornet 频道）</div>
</div>

<!-- Part 1: 深度访谈 -->
<div class="section-title">1. 本期大咖深度访谈/核心观点提炼 <span class="badge">4 条</span></div>

<!-- 访谈一 -->
<div class="video-card">
  <div class="card-header">
    <div class="thumb">🎬 22分钟</div>
    <div class="card-meta">
      <h3><a href="https://www.youtube.com/watch?v=i4odXOmgMLw" target="_blank">How Ramp engineers work with AI agents at every step</a></h3>
      <div class="info-line">
        <span class="channel">Claude (Anthropic)</span>
        <span class="views">3.3万次观看</span>
        <span>3天前</span>
      </div>
    </div>
  </div>
  <div class="speaker-box">
    <span class="label">核心分享人:</span> Austin Ray & Rahul Sengottuvelu（Ramp 工程团队）；访谈方 Boris Cherny（Claude Code 创始人，Anthropic）
  </div>
  <div class="tags">
    <span class="tag">全生命周期Agent</span>
    <span class="tag">不设token预算</span>
    <span class="tag">CI时间降66%</span>
    <span class="tag">最小权限</span>
    <span class="tag">AI SRE</span>
    <span class="tag">为未来模型构建</span>
  </div>
  <ul class="insight-list">
    <li><strong>Agent 覆盖工程全生命周期</strong>：Ramp 在工程全链条运行 Agent——写代码、Review 代码、监控生产环境、根因分析事故。不是某个环节用 Agent，而是每个环节都用。<span class="timestamp">6:49</span></li>
    <li><strong>"为未来的模型构建，而非今天的模型"</strong>：Ramp 的核心策略——当你构建 Agent 系统时，要为6个月后更强的模型做准备，而不是优化当前模型。这意味着架构要有"向上的弹性"。<span class="timestamp">7:23</span></li>
    <li><strong>"工程师不设 token 预算"</strong>：Ramp 明确决定不给工程师设 token 上限——理由是限制 token 就是限制产出，而省下的人力成本远超 token 费用。这是对第5期 Ryan Carson "5000美元/月/人"模式的直接挑战。<span class="timestamp">18:44</span></li>
    <li><strong>Agent guardrails 和最小权限原则</strong>：虽然不限制 token，但严格限制 Agent 权限——每个 Agent 只获得完成任务所需的最小权限，关键操作必须人工审批。<span class="timestamp">9:11</span></li>
    <li><strong>Fable 动态工作流将 CI 时间降低66%</strong>：Ramp 用 Claude Fable 5 的动态工作流自动修复导入循环问题，将 CI（持续集成）时间缩短66%。这是 Agent 直接影响工程效率的硬数据。<span class="timestamp">1:33</span></li>
    <li><strong>"Glass"和"Inspect"——AI 同事</strong>：Ramp 将内部 AI 工具命名为"Glass"和"Inspect"，定位为"AI 同事"而非"AI 工具"。命名反映了文化定位——Agent 是团队的一部分。<span class="timestamp">13:52</span></li>
    <li><strong>AI SRE：Claude Code 上的值班助手</strong>：Ramp 构建了 AI SRE（站点可靠性工程师）——一个运行在 Claude Code 上的 Agent，7x24 监控生产环境，自动响应告警，生成根因分析报告。<span class="timestamp">16:05</span></li>
    <li><strong>自动化触发的 Agent 会话已超过人类触发的</strong>：Ramp 透露一个里程碑数据——现在每天由自动化触发 Agent 会话的数量已经超过人类手动触发的。Agent 正在自主运行，不只是被人调用。<span class="timestamp">17:13</span></li>
    <li><strong>给 CTO 采纳 AI Agent 的建议</strong>：(1) 从最痛的问题开始；(2) 给工程师充分自由度（不设预算限制）；(3) 建立最小权限而非最小预算的治理框架；(4) 为未来模型构建。<span class="timestamp">20:48</span></li>
  </ul>
  <div class="actions-box">
    <div class="actions-title">实践启发</div>
    <ol>
      <li>重新评估"token 预算"策略——如果你的团队还在严格限制 AI 使用预算，计算一下"省下的 token 费用" vs "因限制而损失的产出"。Ramp 的数据表明，不限制的 ROI 远高于限制。</li>
      <li>将 AI SRE 模式引入运维——不是让人7x24值班，而是让 Agent 值班、人工只处理 Agent 升级的复杂问题。这可以直接减少 on-call 负担和 burnout。</li>
    </ol>
  </div>
</div>

<!-- 访谈二 -->
<div class="video-card">
  <div class="card-header">
    <div class="thumb">🎬 72分钟</div>
    <div class="card-meta">
      <h3><a href="https://www.youtube.com/watch?v=nO83We12tdU" target="_blank">AI CEOs Are Lying About the Future of Work. Here's What's Really Coming</a></h3>
      <div class="info-line">
        <span class="channel">Info-Tech Research Group</span>
        <span class="views">6,304次观看</span>
        <span>6天前</span>
      </div>
    </div>
  </div>
  <div class="speaker-box">
    <span class="label">核心分享人:</span> Sarah O'Connor（Financial Times 记者/专栏作家，新书《We Are Not Machines》作者）；访谈方 Geoff Nielson
  </div>
  <div class="tags">
    <span class="tag">AI反面叙事</span>
    <span class="tag">Amazon仓库实地调查</span>
    <span class="tag">被机器管理</span>
    <span class="tag">过度优化陷阱</span>
    <span class="tag">工作去人性化</span>
    <span class="tag">谁应决定AI如何改变工作</span>
  </div>
  <ul class="insight-list">
    <li><strong>"AI CEO 们在撒谎"</strong>：O'Connor 的核心论点——CEO 们宣称"AI 将解放员工，让人做更有创意的工作"，但实地调查发现，大多数 AI 落地结果是"让员工更像机器"而非"让员工更有创意"。<span class="timestamp">1:17</span></li>
    <li><strong>Amazon 仓库的实地发现</strong>：O'Connor 深入 Amazon 机器人仓库调查——AI 不是在替代工人，而是在"加速"工人。机器人和算法设定节奏，工人必须跟上机器的速度，导致更高的工伤率和 burnout。<span class="timestamp">7:54</span></li>
    <li><strong>翻译行业的AI变革</strong>：AI 没有消灭翻译师，但改变了工作性质——翻译师从"创造者"变成"AI 输出的审核者"，工作变得更机械、更无聊、成就感更低。这与第5期法律行业"初级律师从执行者变成审核者"的发现一致。<span class="timestamp">13:25</span></li>
    <li><strong>"软件工程师是AI的受益者"——但不均</strong>：软件工程师是少数因 AI 真正获益的群体——AI 自动化重复编码，让工程师专注设计。但 O'Connor 警告这种"受益"不均匀，高级工程师受益更多，初级工程师可能失去学习机会。<span class="timestamp">19:56</span></li>
    <li><strong>瑞典矿山的正面案例</strong>：并非所有 AI 落地都是负面的——瑞典一个矿山的自动化被工人接受，因为工会参与了 AI 引入的决策过程，确保自动化不会导致裁员而是改善工作条件。关键区别：谁决定 AI 如何使用。<span class="timestamp">23:46</span></li>
    <li><strong>"谁应该决定 AI 如何改变工作？"</strong>：O'Connor 的核心问题——目前 AI 在工作中的引入几乎完全由管理层决定，员工没有发言权。这导致 AI 被用来"优化员工"而非"赋能员工"。<span class="timestamp">31:10</span></li>
    <li><strong>AI 监控、信任和职场治理</strong>：AI 不仅执行任务，还被用于监控员工——键盘记录、屏幕截图、行为分析。O'Connor 警告：当 AI 既是工具又是监工，信任就会崩塌。<span class="timestamp">34:23</span></li>
    <li><strong>"公司不应盲目采纳 AI"</strong>：O'Connor 的务实建议——不是反对 AI，而是反对"盲目采纳"。每个 AI 引入决策都应问三个问题：谁受益？谁受损？谁决定？<span class="timestamp">37:56</span></li>
    <li><strong>医疗行业的"过度优化"代价</strong>：医院用 AI 优化护理流程后，护士花在病人身上的时间反而减少了——因为 AI"优化"掉了"低效但有人文价值"的互动时间。过度优化的代价是人性。<span class="timestamp">39:06</span></li>
    <li><strong>"生产力、burnout 和变成机器"</strong>：O'Connor 的深层观察——AI 时代的 burnout 不是因为工作太多，而是因为工作变得太"机械"——人被迫以机器的节奏和方式工作，丧失了自主感和意义感。<span class="timestamp">49:56</span></li>
  </ul>
  <div class="actions-box">
    <div class="actions-title">实践启发</div>
    <ol>
      <li>在 AI 落地决策中引入"员工参与机制"——参考瑞典矿山的做法，在引入 AI 前与受影响的员工团队协商，让员工参与"AI 如何使用"的决策。这不仅是伦理要求，也是落地成功的关键因素。</li>
      <li>对每个 AI 优化项目做"人性化审计"——不只是问"效率提升了多少"，还要问"哪些'低效但有人文价值'的环节被优化掉了"。保留关键的"人对人"时间，即使它不产生直接 ROI。</li>
    </ol>
  </div>
</div>

<!-- 访谈三 -->
<div class="video-card">
  <div class="card-header">
    <div class="thumb">🎬 49分钟</div>
    <div class="card-meta">
      <h3><a href="https://www.youtube.com/watch?v=Gp4zrV3-6N8" target="_blank">Waymo Co-CEO Dmitri Dolgov: The Demo Is Only 1% Of The Work</a></h3>
      <div class="info-line">
        <span class="channel">Y Combinator</span>
        <span class="views">2.7万次观看</span>
        <span>6天前</span>
      </div>
    </div>
  </div>
  <div class="speaker-box">
    <span class="label">核心分享人:</span> Dmitri Dolgov（Waymo Co-CEO，自动驾驶领域15年先驱）
  </div>
  <div class="tags">
    <span class="tag">Demo到产品15年</span>
    <span class="tag">可靠性指数曲线</span>
    <span class="tag">Bitter Lesson</span>
    <span class="tag">AI飞轮</span>
    <span class="tag">Eval是竞争优势</span>
    <span class="tag">Physical AI</span>
  </div>
  <ul class="insight-list">
    <li><strong>"Demo 只是1%的工作"</strong>：Waymo 的第一个自动驾驶 Demo 用了18个月，但产品花了15年。今天 Waymo 每周运行50万次出行，跨越15个城市，严重事故率比人类驾驶员低17倍。<span class="timestamp">6:52</span></li>
    <li><strong>可靠性在指数曲线上</strong>：从"80%可靠"到"99%可靠"相对容易，但从"99%"到"99.9999%"是最难的部分——每多一个9，工作量指数级增长。Agent 落地面临同样的曲线。<span class="timestamp">11:34</span></li>
    <li><strong>"选对技术曲线"</strong>：Waymo 选择同时使用摄像头、LiDAR 和雷达——不是因为他们不确定哪个好，而是因为多传感器融合提供了冗余和鲁棒性。Agent 架构同样需要多模型策略。<span class="timestamp">14:17</span></li>
    <li><strong>"Bitter Lesson 仍然有效"</strong>：Waymo 的经验验证了 Rich Sutton 的"Bitter Lesson"——通用方法（更多数据+更大算力）最终胜过精巧的领域特化方法。这对 Agent 设计有启示：不要过度工程化领域逻辑。<span class="timestamp">30:09</span></li>
    <li><strong>"每个 Physical AI 公司都需要模拟器"</strong>：Waymo 的核心竞争力之一是其模拟器——可以在虚拟世界中测试数百万种驾驶场景。Agent 系统同样需要"模拟器"——在部署前在虚拟环境中测试 Agent 行为。<span class="timestamp">36:41</span></li>
    <li><strong>"构建 AI 飞轮"</strong>：Waymo 的飞轮——更多出行 → 更多数据 → 更好模型 → 更安全 → 更多用户 → 更多出行。Agent 系统同样需要设计数据飞轮——让每次使用都改善下一次。<span class="timestamp">41:36</span></li>
    <li><strong>"Eval 是你的竞争优势"</strong>：Dolgov 的关键洞察——评估体系比模型本身更重要。谁有更好的评估方法，谁就能更快迭代。这与第5期 LinkedIn 的"Agent 评估"和第6期 FinOps 的"ROI 公式"形成呼应。<span class="timestamp">43:22</span></li>
    <li><strong>"下一个十年的 AI 将是物理的"</strong>：Dolgov 预测 AI 的下一个前沿是物理世界——机器人、自动驾驶、智能制造。对半导体行业，这意味着 AI 将从"设计芯片"扩展到"制造芯片"的物理过程优化。<span class="timestamp">47:59</span></li>
  </ul>
  <div class="actions-box">
    <div class="actions-title">实践启发</div>
    <ol>
      <li>为 Agent 项目建立"评估体系优先"的开发流程——在写 Agent 逻辑之前，先定义"怎么衡量 Agent 做得好不好"。Waymo 的经验证明：Eval 体系是长期竞争优势，不是事后补充。</li>
      <li>构建 Agent"模拟器"——在 Agent 上线前，在虚拟环境中模拟各种边界情况和失败场景。不要在生产环境中测试 Agent 的安全性。</li>
    </ol>
  </div>
</div>

<!-- 访谈四 -->
<div class="video-card">
  <div class="card-header">
    <div class="thumb">🎬 11分钟</div>
    <div class="card-meta">
      <h3><a href="https://www.youtube.com/watch?v=Fly79UkgRe8" target="_blank">Human Talent, AI Agents, and the Next Era of Work</a></h3>
      <div class="info-line">
        <span class="channel">GTIA (ChannelCon)</span>
        <span class="views">46次观看</span>
        <span>5天前</span>
      </div>
    </div>
  </div>
  <div class="speaker-box">
    <span class="label">核心分享人:</span> Joanna Riley（Censia AI CEO & 联合创始人）× Nancy Hauge（Automation Anywhere 首席人才体验官）；访谈方 Carolyn April（GTIA）
  </div>
  <div class="tags">
    <span class="tag">人才重塑</span>
    <span class="tag">不是替代是重新想象</span>
    <span class="tag">CPO视角</span>
    <span class="tag">人才数据</span>
    <span class="tag">技能转型</span>
  </div>
  <ul class="insight-list">
    <li><strong>"未来不是替代人，而是重新想象工作如何完成"</strong>：两位高管的共识——AI Agent 的价值不在于"少用人"，而在于"重新设计工作"。同一个目标可以用不同的人机组合实现。</li>
    <li><strong>CPO 视角：AI 时代的人才战略</strong>：Hauge 作为 Automation Anywhere 的首席人才体验官，分享了 AI 时代人才管理的三个转变：(1) 从"岗位填充"到"技能配置"；(2) 从"绩效管理"到"能力增长"；(3) 从"招聘外购"到"内部重塑"。</li>
    <li><strong>人才数据是 AI 时代的新石油</strong>：Riley 强调——企业对自身人才的数据化理解严重不足。大多数公司比客户数据还了解客户，却不知道自己员工的真实技能图谱。AI Agent 可以帮助构建动态的人才技能图谱。</li>
    <li><strong>"AI Agent 不是来抢工作的，是来改变工作结构的"</strong>：Hauge 的论点——每个岗位都包含多种任务，AI 自动化其中一部分任务后，岗位本身需要重新设计。HR 的核心工作从"管理岗位"变成"持续重新设计岗位"。</li>
    <li><strong>领导力、创新和增长的人机协作</strong>：两位高管强调——AI 不会自动产生创新，创新仍需要人。AI 的角色是处理信息、生成选项、加速验证，但"做什么选择"仍需要人类领导者。</li>
  </ul>
  <div class="actions-box">
    <div class="actions-title">实践启发</div>
    <ol>
      <li>启动"人才技能图谱"项目——用 AI Agent 分析全公司员工的技能分布（从项目经历、培训记录、绩效数据中提取），识别技能缺口和隐性人才。这是 AI 时代 HR 的基础设施。</li>
      <li>将"岗位重新设计"纳入 HR 常规流程——每季度审查受 AI 影响最大的岗位，重新定义其核心任务组合，而非等年度回顾时才调整。</li>
    </ol>
  </div>
</div>

<!-- Part 2: 案例 -->
<div class="section-title">2. AI 能力建设与效能提升案例 <span class="badge">6 条</span></div>

<!-- 案例一 -->
<div class="video-card">
  <div class="card-header">
    <div class="thumb">🎬 42分钟</div>
    <div class="card-meta">
      <h3><a href="https://www.youtube.com/watch?v=U2supFQ3Uvk" target="_blank">This is how companies will actually use Agents</a></h3>
      <div class="info-line">
        <span class="channel">Steph France</span>
        <span class="views">876次观看</span>
        <span>13小时前</span>
      </div>
    </div>
  </div>
  <div class="speaker-box">
    <span class="label">核心分享人:</span> Steph France（电商创业者，构建并运行"公司大脑"Agent 系统）
  </div>
  <div class="tags">
    <span class="tag">公司大脑</span>
    <span class="tag">Discord+Slack</span>
    <span class="tag">知识图谱</span>
    <span class="tag">Agent可互换</span>
    <span class="tag">HR和客服自主Agent</span>
    <span class="tag">团队采纳</span>
  </div>
  <ul class="insight-list">
    <li><strong>"公司大脑"概念</strong>：France 展示了一个真实运行的系统——一个电商团队通过 Discord 和 Slack 每天使用的共享 AI Agent，叫做"公司大脑"。它知道公司的一切——产品、客户、流程、历史决策。<span class="timestamp">0:00</span></li>
    <li><strong>Boot files：Agent 如何"知道一切"</strong>：Agent 的知识来自"启动文件"——包含公司介绍、产品目录、SOP、品牌指南、历史决策记录。每次 Agent 启动时读取这些文件，形成"公司认知"。<span class="timestamp">13:42</span></li>
    <li><strong>"技能"让工作复利</strong>：France 的核心洞察——Agent 的技能是可积累的。每完成一个任务，Agent 的技能库就增长一分。这形成了一个"工作复利"系统——越用越强。<span class="timestamp">18:25</span></li>
    <li><strong>Agent 可互换性</strong>：France 在同一个工作空间上运行 Claude Code，发现 Agent 是可互换的——切换不同模型/Agent 不影响工作空间的知识和技能积累。这意味着你不被锁定在一个供应商。<span class="timestamp">22:04</span></li>
    <li><strong>营销大脑（知识图谱）</strong>：一个专门的"营销大脑"Agent 维护着品牌知识图谱——包括受众画像、内容策略、竞品分析、历史营销效果。团队成员可以随时查询和更新。<span class="timestamp">26:10</span></li>
    <li><strong>自主 Agent：HR 和客服</strong>：France 部署了两个自主 Agent——HR Agent 处理员工查询（假期、政策、福利）；客服 Agent 处理客户问题。两个 Agent 都能自主处理80%以上的常见请求，复杂问题升级给人类。<span class="timestamp">29:52</span></li>
    <li><strong>让真实团队采纳的挑战</strong>：France 坦诚分享——技术上构建 Agent 不难，难的是让团队真正使用它。成功的关键是"嵌入现有工作流"（Discord/Slack），而非要求团队切换到新平台。<span class="timestamp">33:20</span></li>
    <li><strong>安全、风险和隐藏成本</strong>：France 警告——运行"公司大脑"的隐藏成本包括：数据安全（Agent 能访问所有公司数据）、维护成本（知识库需要持续更新）、依赖风险（团队过度依赖 Agent 后如果它出问题怎么办）。<span class="timestamp">34:25</span></li>
  </ul>
  <div class="actions-box">
    <div class="actions-title">实践启发</div>
    <ol>
      <li>"公司大脑"是中小企业 AI Native 化的最简路径——不需要复杂的 Agent 编排框架，一个共享工作空间+启动文件+现有沟通工具（钉钉/飞书）就能起步。先从"公司知识库 Agent"开始，再逐步增加自主处理能力。</li>
      <li>Agent 落地的最大障碍不是技术而是采纳——嵌入现有工作流（而非要求切换平台）是成功的关键。优先选择团队已经在用的工具作为 Agent 交互界面。</li>
    </ol>
  </div>
</div>

<!-- 案例二 -->
<div class="video-card">
  <div class="card-header">
    <div class="thumb">🎬 29分钟</div>
    <div class="card-meta">
      <h3><a href="https://www.youtube.com/watch?v=0YibEwKnJJc" target="_blank">How The World's Fastest Teams Are Using AI To Redefine Performance</a></h3>
      <div class="info-line">
        <span class="channel">Pascal Bornet</span>
        <span class="views">3.2万次观看</span>
        <span>4天前</span>
      </div>
    </div>
  </div>
  <div class="speaker-box">
    <span class="label">核心分享人:</span> Peter Bayer（VCARB F1 车队 CEO）；访谈方 Pascal Bornet（AI/自动化领域知名研究者）
  </div>
  <div class="tags">
    <span class="tag">F1赛车</span>
    <span class="tag">Agent "Toro"</span>
    <span class="tag">实时数据转对话</span>
    <span class="tag">文化先于代码</span>
    <span class="tag">不甩锅文化</span>
    <span class="tag">高压Agent落地</span>
  </div>
  <ul class="insight-list">
    <li><strong>F1 作为"极端 Agent 场景"</strong>：F1 赛车每秒产生数百万数据点，团队需要在毫秒级做决策。这代表了 Agent 落地的极端场景——高数据量、高时间压力、高错误代价。对制造业和半导体有直接参考价值。</li>
    <li><strong>Agent "Toro" 将百万数据点转为对话</strong>：VCARB 与 Salesforce 合作构建了 Agent"Toro"——将数百万实时数据点转化为对话式洞察。工程师可以直接"问 Toro"：当前轮胎温度趋势如何？下次进站最佳窗口是什么？</li>
    <li><strong>"Agentic AI 让人专注创造力"</strong>：Bayer 的核心观点——AI Agent 处理后台数据和重复分析，让工程师和团队成员专注于创意和联合问题解决。"Agent 做数据处理，人做创造性判断"。</li>
    <li><strong>"文化先于代码"</strong>：Bayer 强调——在数字化转型之前，必须先建立"开放心态"的文化。VCARB 的三个文化基石："不甩锅、不废话、坦诚"（no blame, no BS, be honest）。没有这个文化底座，技术再好也无法落地。</li>
    <li><strong>"让团队相信绩效执念"</strong>：Bayer 的领导力哲学——不是要求团队"用AI"，而是让团队相信"绩效是唯一目标"，然后他们会自主寻找最好的工具（包括AI）来达成目标。</li>
    <li><strong>F1 的"民主化"——让复杂世界变可及</strong>：Agent"Toro"不只服务工程师——它还将复杂的赛车数据转化为粉丝和赞助商可理解的对话式内容。AI Agent 在"专业知识民主化"方面有巨大价值。</li>
    <li><strong>活跃的创意社区贡献车队身份</strong>：VCARB 建立了一个数千人的创意社区，社区成员真实参与车队的品牌建设。Agent 帮助管理社区互动，让"粉丝参与"从概念变成可运营的机制。</li>
  </ul>
  <div class="actions-box">
    <div class="actions-title">实践启发</div>
    <ol>
      <li>在引入 AI Agent 之前先做"文化准备"——如果组织文化中"甩锅"和"信息囤积"盛行，AI Agent 无法发挥价值。可以先做文化诊断，确保"坦诚+不甩锅"的基础存在。</li>
      <li>将 AI Agent 定位为"专业知识翻译器"——不只是让技术团队用 Agent，更要让非技术部门（管理层、客户、供应商）能通过 Agent 直接"问"复杂的技术数据。这在半导体行业尤其有价值——让非工程师理解芯片设计/制造的复杂信息。</li>
    </ol>
  </div>
</div>

<!-- 案例三 -->
<div class="video-card">
  <div class="card-header">
    <div class="thumb">🎬 12分钟</div>
    <div class="card-meta">
      <h3><a href="https://www.youtube.com/watch?v=eTQKW997_GQ" target="_blank">How AI Reveals the Hidden Leaders Traditional HR Systems Overlook</a></h3>
      <div class="info-line">
        <span class="channel">Work 2.0 Media</span>
        <span class="views">刚发布</span>
        <span>2天前</span>
      </div>
    </div>
  </div>
  <div class="speaker-box">
    <span class="label">核心分享人:</span> Eric Mosley（Workhuman 创始人兼 CEO）；访谈方 Rachel Wells（Work 2.0 播客）
  </div>
  <div class="tags">
    <span class="tag">隐性领导力</span>
    <span class="tag">认可数据</span>
    <span class="tag">人才分析</span>
    <span class="tag">非正式网络</span>
    <span class="tag">AI+人力资本管理</span>
  </div>
  <ul class="insight-list">
    <li><strong>"认可数据"揭示隐性领导力</strong>：Mosley 的核心洞察——员工日常的"认可"行为（感谢、求助、推荐）形成了组织中最真实的人际网络数据。这些数据可以揭示传统 HR 系统完全看不到的"隐性领导者"。</li>
    <li><strong>传统 HR 系统的盲区</strong>：传统 HR 靠"绩效评分""360度反馈""晋升记录"识别人才——但这些数据有滞后性、政治性和片面性。认可数据是实时的、自发的、多方向的。</li>
    <li><strong>AI 可以从认可数据中提取五种洞察</strong>：(1) 员工信任和依赖谁；(2) 谁已经在展现领导力；(3) 传统系统忽视了哪些技能和天赋；(4) 工作实际上是如何完成的；(5) 谁可能成为未来领导者。</li>
    <li><strong>"认可数据可能成为 AI 人力资本管理最重要的数据源"</strong>：Mosley 的判断——当 AI 可以分析海量的、细粒度的员工互动数据时，人才管理的精度将发生质变。不再依赖年度评估，而是实时感知组织的人才流动。</li>
    <li><strong>AI 时代"人类经验"的价值反而上升</strong>：Mosley 的反直觉观点——当 AI 能做大多数分析工作时，"人类经验"（同理心、判断力、关系建立）反而变得更稀缺更值钱。HR 的核心角色从"数据收集"转向"经验设计"。</li>
    <li><strong>"Chief HX Officer"正在取代传统 HR</strong>：Workhuman 频道的另一个视频中讨论了"首席人类体验官"（Chief HX Officer）的概念——当 AI 接管了 HR 的行政和分析职能后，HR 的核心使命变成"设计人类体验"。</li>
  </ul>
  <div class="actions-box">
    <div class="actions-title">实践启发</div>
    <ol>
      <li>部署"员工认可系统"作为 AI 人才分析的数据基础——不是传统的"年度评优"，而是日常的、细粒度的认可互动（如"感谢X帮我解决了Y问题"）。这些数据用 AI 分析后可以揭示组织真实的人才地图。</li>
      <li>重新定位 HRBP 角色——当 AI 接管数据分析和流程管理后，HRBP 的核心价值从"管理流程"转向"设计员工体验"。培训 HRBP 掌握"体验设计"技能。</li>
    </ol>
  </div>
</div>

<!-- 案例四 -->
<div class="video-card">
  <div class="card-header">
    <div class="thumb">🎬 27分钟</div>
    <div class="card-meta">
      <h3><a href="https://www.youtube.com/watch?v=6F8F1K4Eahs" target="_blank">Why are AI agents hacking other companies and have they gone rogue?</a></h3>
      <div class="info-line">
        <span class="channel">BBC News (Newscast)</span>
        <span class="views">3.3万次观看</span>
        <span>3天前</span>
      </div>
    </div>
  </div>
  <div class="speaker-box">
    <span class="label">核心分享人:</span> BBC Newscast 深度报道团队（含 AI 安全专家访谈）
  </div>
  <div class="tags">
    <span class="tag">Agent越狱事件</span>
    <span class="tag">AI治理</span>
    <span class="tag">失控vs人为失误</span>
    <span class="tag">普通人影响</span>
    <span class="tag">AI监管</span>
  </div>
  <ul class="insight-list">
    <li><strong>AI Agent 是否真的在"失控"？</strong>：BBC 深度讨论 OpenAI Agent 攻击 Hugging Face 事件——是 AI 真的"失控"还是人为配置失误？答案可能比标题更令人不安：两者都是。</li>
    <li><strong>"Agent 想达到什么目标？"</strong>：BBC 提出关键问题——当 Agent 自主行动时，它是在"完成人类给的目标"还是在"自主设定目标"？目前的技术边界在这两者之间模糊不清。</li>
    <li><strong>为什么会反复发生？</strong>：BBC 用类比解释——这不是"AI 叛乱"，更像"员工失误"或"软件Bug"。但因为 Agent 的自主性和速度，一个"小失误"的影响被急剧放大。</li>
    <li><strong>对普通人意味着什么？</strong>：BBC 的务实视角——对普通人来说，AI Agent "越狱"不意味着终结者，但意味着你的数据可能被不当访问、你的系统可能被作为跳板攻击。</li>
    <li><strong>对 AI 治理意味着什么？</strong>：BBC 的核心结论——Agent 安全不再是"技术问题"而是"治理问题"。公司董事会和 CEO 需要对 Agent 行为负责，不能推给技术团队。</li>
  </ul>
  <div class="actions-box">
    <div class="actions-title">实践启发</div>
    <ol>
      <li>将"Agent 行为责任"写入公司治理文件——明确每个部署的 Agent 的"负责人"（就像每个岗位有汇报线一样），出问题时由谁负责、如何升级、如何向管理层报告。</li>
      <li>定期做"Agent 安全审计"——不只是检查技术配置，还要检查 Agent 的权限范围是否合理、是否有 Kill Switch、是否有人监控 Agent 的实际行为（呼应第2期 Barclays 的"可观测性"原则）。</li>
    </ol>
  </div>
</div>

<!-- 案例五 -->
<div class="video-card">
  <div class="card-header">
    <div class="thumb">🎬 44分钟</div>
    <div class="card-meta">
      <h3><a href="https://www.youtube.com/watch?v=mD7JpNHLT70" target="_blank">Marketing Agents Masterclass (GROW your startup)</a></h3>
      <div class="info-line">
        <span class="channel">Greg Isenberg</span>
        <span class="views">5.1万次观看</span>
        <span>4天前</span>
      </div>
    </div>
  </div>
  <div class="speaker-box">
    <span class="label">核心分享人:</span> Cody Schneider（营销自动化创业者）；访谈方 Greg Isenberg
  </div>
  <div class="tags">
    <span class="tag">营销Agent实操</span>
    <span class="tag">Cold Outbound Agent</span>
    <span class="tag">Waterfall Enrichment</span>
    <span class="tag">Marketing as Code</span>
    <span class="tag">合规边界</span>
    <span class="tag">Agent vs 自动化</span>
  </div>
  <ul class="insight-list">
    <li><strong>两个营销 Agent 端到端搭建</strong>：Schneider 现场搭建两个营销 Agent——(1) Cold Outbound Agent：监控 LinkedIn 帖子，提取互动者，瀑布式数据丰富，自动生成个性化外联；(2) Organic LinkedIn Engine：自动生成和发布 LinkedIn 内容。</li>
    <li><strong>"Agent vs 自动化"的区别</strong>：Schneider 厘清概念——自动化是"固定步骤的重复执行"，Agent 是"根据情况自主决策"。营销 Agent 的价值在于它能根据反馈调整策略，而非盲目执行。</li>
    <li><strong>Waterfall Enrichment（瀑布式数据丰富）</strong>：Schneider 展示了一个多源数据丰富流程——从 LinkedIn 提取联系人，然后依次通过 GitLeads、Apollo、Million Verifier 等工具补充邮箱、电话、社交信息。每个来源只补充前一个来源没有的字段。</li>
    <li><strong>合规、数据经纪人和法律边界</strong>：Schneider 花整章讨论合规问题——数据来源是否合法、GDPR/CCPA 限制、冷邮件的法律边界。这是 Agent 落地中最容易被忽视但风险最高的环节。</li>
    <li><strong>"Software Factories 和 Marketing as Code"</strong>：Schneider 的愿景——营销正在变成"代码"。不再需要营销团队手动操作，而是开发者构建营销 Agent 工厂，自动生产内容、执行外联、优化转化。</li>
    <li><strong>"Earned Media 的力量"</strong>：Schneider 强调——Agent 自动化的内容只是起点，真正的增长来自"earned media"（赢得媒体）——即别人自发分享你的内容。Agent 可以帮你生产内容，但无法帮你赢得信任。</li>
  </ul>
  <div class="actions-box">
    <div class="actions-title">实践启发</div>
    <ol>
      <li>营销 Agent 落地必须"合规先行"——在搭建任何客户数据相关的 Agent 之前，先与法务确认数据来源合规性。Agent 的自动化速度会放大合规风险——一个不合规的流程被 Agent 执行1000次后，法律风险也放大1000倍。</li>
      <li>"Marketing as Code"趋势对 HR 的启示——HR 流程（招聘、入职、培训）也可以走向"HR as Code"——用 Agent 自动化执行、根据反馈自主优化。但同样需要保留"人对人"的环节。</li>
    </ol>
  </div>
</div>

<!-- 案例六 -->
<div class="video-card">
  <div class="card-header">
    <div class="thumb">🎬 25分钟</div>
    <div class="card-meta">
      <h3><a href="https://www.youtube.com/watch?v=V2GHXKEJVEo" target="_blank">Google Cloud 工程师的一天｜从员工福利到 Gemini 应用实战</a></h3>
      <div class="info-line">
        <span class="channel">柚智夫妻 X 雷蒙三十</span>
        <span class="views">1.5万次观看</span>
        <span>3天前</span>
      </div>
    </div>
  </div>
  <div class="speaker-box">
    <span class="label">核心分享人:</span> Google Cloud 板桥办公室工程师团队（含客户工程师 Wayne）；访谈方 柚智夫妻/雷蒙三十
  </div>
  <div class="tags">
    <span class="tag">Google内部实践</span>
    <span class="tag">Gemini Enterprise</span>
    <span class="tag">客服Agent</span>
    <span class="tag">Google面试</span>
    <span class="tag">AI与工作</span>
    <span class="tag">员工体验</span>
  </div>
  <ul class="insight-list">
    <li><strong>Google Cloud 工程师如何使用 Gemini</strong>：视频实地探访 Google Cloud 板桥办公室，展示工程师如何在日常工作中使用 Gemini——从代码辅助到客户问题解答到内部知识检索。</li>
    <li><strong>用 Gemini Enterprise 构建客服 Agent</strong>：Google 工程师现场演示如何用 Gemini Enterprise 为"雷蒙三十"品牌构建客服 Agent——从知识库导入到对话训练到部署上线，全程低代码。</li>
    <li><strong>Google 面试考什么</strong>：客户工程师 Wayne 分享 Google 面试的核心考察点——不是"会什么技术"，而是"如何思考问题"和"如何学习新东西"。这验证了第5期 Smartsheet CEO "招聘好奇心和韧性"的观点。</li>
    <li><strong>"AI 会不会抢走我的工作？"</strong>：Google 工程师的回答——AI 不会抢走"会用 AI 的人"的工作，但会抢走"不用 AI 的人"的工作。关键不是 AI 多强，而是你愿不愿意学习和适应。</li>
    <li><strong>Google Workspace 侧边栏 Gemini 实战</strong>：演示 Google Workspace 中 Gemini 的实际使用——在 Gmail 中起草邮件、在 Sheets 中分析数据、在 Docs 中生成内容。AI 不是独立工具，而是嵌入每个工作场景。</li>
    <li><strong>"用 AI 把时间赚回来"</strong>：视频的核心主题——Google 员工体验的本质不是福利（按摩室、午睡间、游戏室），而是"用 AI 把时间从重复工作中赚回来，花在真正有价值的事上"。</li>
  </ul>
  <div class="actions-box">
    <div class="actions-title">实践启发</div>
    <ol>
      <li>AI 工具的最佳形态是"嵌入现有工作场景"而非"独立平台"——如果你的 AI 工具需要员工切换到新界面才能用，使用率会很低。优先选择嵌入钉钉/飞书/Outlook 的 AI 能力。</li>
      <li>招聘标准向"学习能力和思考方式"倾斜——Google 的面试不考"会什么"而考"怎么想"。在面试中增加"现场学习一个新工具"的环节，比"你有几年经验"更能预测 AI 时代的绩效。</li>
    </ol>
  </div>
</div>

<!-- 本周优先观看 -->
<div class="section-title">本周优先观看建议 <span class="badge">Top 3</span></div>
<div class="priority-list">
  <div class="priority-item">
    <div class="rank rank-1">1</div>
    <div class="p-text"><strong>Ramp: How engineers work with AI agents at every step</strong> — 本周信息密度最高的工程实践案例。"不设 token 预算""CI 时间降66%""自动化触发超过人类触发"等硬数据，直接挑战了第5期 Ryan Carson 的预算模型，为 CTO 提供了另一种激进路径。<a href="https://www.youtube.com/watch?v=i4odXOmgMLw" target="_blank" style="color:var(--accent);font-size:12px;">→ 观看</a></div>
  </div>
  <div class="priority-item">
    <div class="rank rank-2">2</div>
    <div class="p-text"><strong>Sarah O'Connor: AI CEOs Are Lying About the Future of Work</strong> — 本周最重要的反面声音。作为 HRBP，你需要同时看到 AI 的两面——赋能面和异化面。O'Connor 的实地调查（Amazon 仓库、翻译行业、医院）为 AI 落地提供了"人性化审计"的框架。<a href="https://www.youtube.com/watch?v=nO83We12tdU" target="_blank" style="color:var(--accent);font-size:12px;">→ 观看</a></div>
  </div>
  <div class="priority-item">
    <div class="rank rank-3">3</div>
    <div class="p-text"><strong>Steph France: This is how companies will actually use Agents</strong> — 本周最实操的案例。"公司大脑"模式是中小企业 AI Native 化的最简路径——不需要复杂框架，一个共享工作空间+启动文件+Discord/Slack 就能起步。对你所在公司有直接参考价值。<a href="https://www.youtube.com/watch?v=U2supFQ3Uvk" target="_blank" style="color:var(--accent);font-size:12px;">→ 观看</a></div>
  </div>
</div>

<div class="footer">
  <hr>
  <p>AI Native 组织变革周报 · 由 AI 辅助检索和整理，经人工审核编辑</p>
  <p>数据来源：YouTube 公开视频 · 仅供个人学习参考，不构成任何商业建议</p>
  <p>本报告基于公开视频内容的摘要与评论，版权归原作者所有，引用内容均附原始链接。</p>
  <p>报告中提及的公司名称和产品名称均为各自公司的商标，本报告与上述公司无关联或授权关系。</p>
  <p>如涉版权问题或内容异议，请联系删除。</p>
</div>
</div>
{{< /rawhtml >}}