---
title: "老员工离职前的经验萃取，让AI当记录员"
slug: "lao-yuan-gong-li-zhi-qian-de-jing-yan-cui-qu-rang-ai-dang-ji-lu-yuan"
date: 2026-09-27T15:00:00+08:00
draft: false
categories: ["ai-native"]
tags: ["AI Native", "经验萃取", "离职交接", "AI记录员", "知识管理"]
description: "做HR这些年，最让我心里发紧的时刻之一，是收到一封资深员工的离职邮件。不是流程难办，而是那一瞬间我会想到：这个人脑子里十几年的项目经验、踩坑记忆、对客户的判断，可能三个工作日内就跟着工牌一起交回来了。"
---

{{< rawhtml >}}
<div class="article-content">
<style>

  .article-content {background:#FAFAFA;color:#171717;font-family:-apple-system,"PingFang SC","Hiragino Sans GB","Microsoft YaHei",sans-serif;line-height:1.8;margin:0;padding:2rem 1rem;}
  .article-content-inner { margin: 0; padding: 2rem 1rem; }
  h1{font-size:2.25rem;line-height:1.4;margin:0 0 1.5rem;}
  h2{font-size:1.5rem;line-height:1.5;border-left:4px solid #0D9488;padding-left:0.75rem;margin:2.5rem 0 1rem;}
  p{margin:0 0 1.2rem;}
  .notice{background:#F0FDFA;border-left:4px solid #14B8A6;padding:1rem 1.25rem;border-radius:4px;margin:0 0 2rem;font-size:0.95rem;}
  pre{background:#F4F4F5;border:1px solid #E4E4E7;border-radius:6px;font-family:monospace;padding:1rem;overflow-x:auto;font-size:0.9rem;line-height:1.7;margin:0 0 1.5rem;white-space:pre-wrap;}
  .tags{margin-top:3rem;font-size:0.85rem;}
  .tag-row{margin:0.4rem 0;}
  .pill{display:inline-block;background:#F4F4F5;color:#71717A;border-radius:999px;padding:0.2rem 0.9rem;margin:0.25rem 0.25rem 0.25rem 0;}
  strong{color:#0D9488;}

</style>
<div class="article-content-inner">
<h1>老员工离职前的经验萃取，让AI当记录员</h1>

<div class="notice">本文案例与数据均做示意性处理，请勿对号入座。</div>

<p>做HR这些年，最让我心里发紧的时刻之一，是收到一封资深员工的离职邮件。不是流程难办，而是那一瞬间我会想到：这个人脑子里十几年的项目经验、踩坑记忆、对客户的判断，可能三个工作日内就跟着工牌一起交回来了。</p>

<p>以前我们也搞过经验萃取。做法通常是组织一场欢送会性质的访谈，HR拿着提纲问两小时，回去整理出一份"岗位经验总结"，存进共享盘，然后就没有然后了。那份文档大概率没人再看第二眼。问题不在于老员工不想讲，而在于传统萃取这件事本身太贵、太慢、太依赖访谈者的水平。人走了，萃取往往也就不了了之。</p>

<p>今年我在支持的一条业务线上试了另一个路子：把AI请进来当记录员和追问者，HR退到编排的位置。这篇复盘讲讲具体怎么做的，以及哪些环节AI碰不得。</p>

<h2>先想清楚：经验萃取到底难在哪</h2>

<p>我的体会是难在三处。第一，老员工的时间贵，走之前那一两周排满了交接，没人愿意再坐下来陪你聊两小时"人生经验"。第二，最有价值的经验往往是隐性的，你直接问"你有什么经验"，他答不上来；得靠具体场景去钩。第三，传统访谈产出的文档是"一次性"的，写完就沉底，后来的人根本搜不到、也不会想到去搜。</p>

<p>这三条，恰好对应了AI能干的事：异步、不知疲倦地追问、以及把碎片内容结构化成可检索的知识。但它干不了的那件事同样关键——判断哪些经验值得留、留下的话怎么用。这件事还是得人来。</p>

<h2>具体做法：三步走，AI只占两步</h2>

<p>第一步是HR做的：花二十分钟，把这个人的岗位拆成四到六个典型任务场景。比如做交付管理的老员工，场景就是"项目延期了怎么跟客户谈""供应商突然掉链子怎么兜底"这类。不需要精雕细琢，列出来就行。这一步的价值在于把"你的经验"这种空泛问题，变成"那个具体场景下你做了什么"的具体问题。</p>

<p>第二步交给AI：把场景列表和一个访谈指令喂给它，让它对每个场景生成追问式的访谈提纲，然后老员工用打字或语音异步回答，AI负责追问两到三轮。我给智能体的指令大意是这样的：</p>

<pre>角色：你是一名经验访谈助手，帮即将离职的资深员工整理岗位经验。

规则：
1. 一次只问一个问题，基于对方的回答继续追问，最多追问三轮。
2. 追问优先问具体案例：当时的情况、你做了什么、结果如何、如果重来会怎么改。
3. 对方回答空泛时，用一个假设场景把问题落地，例如"如果客户当场翻脸，你第一句话会说什么"。
4. 不评价、不建议，只提问和记录。
5. 访谈结束后，把所有内容按场景整理成结构化文档：做法、原因、例外情况、新人最容易犯的错。</pre>

<p>这一段指令本身没什么高深的，我调了两版才稳定。关键是第四条——AI很忍不住要"给建议"，一旦它开始输出观点，老员工就不想说了。访谈这个东西，人只对"认真听的人"讲真话，机器也一样。</p>

<p>第三步又回到HR手上：拿着AI整理出来的结构化文档，跟老员工约一次三十分钟的当面确认。这一步不能省，因为AI整理的内容里总有几处理解偏差，而当面确认的过程本身会让老员工再补充出最有价值的那些"没被问到的东西"。确认完的文档放进团队知识库，挂到对应岗位和场景的标签下。</p>

<h2>跑下来的真实感受</h2>

<p>成本上，过去一场两小时的访谈加整理，HR要投入大半天；现在HR的净投入大概一小时，老员工的投入是碎片时间里的四十分钟到一小时。产出的质量反而更好，因为AI的追问比我现场发挥稳定，不会漏问题，也不会因为聊嗨了跑题。</p>

<p>但有两个坑值得说。一是别指望全自动。我试过让AI直接约时间、发链接、催回答，老员工体验很差，觉得被机器人催命。离职前的情绪是敏感的，所有"人对人"的触点还是HR亲自来，AI只藏在背后干活。二是萃取出的经验要有人"接管"。我们后来把每份经验文档指定了一位在职的接手人，负责一个月内基于文档做一次实操演练并反馈哪里不管用。没有这个闭环，文档照样会沉底——AI解决的是记录成本，解决不了使用意愿。</p>

<h2>这件事改变了我对"组织记忆"的看法</h2>

<p>以前我觉得经验流失是个无解的事，本质上是因为记录成本高于任何人的动力。AI把这个成本压下来之后，组织的记忆第一次有了低成本沉淀的可能。而HR在这件事里的角色，从"访谈者"变成了"场景设计者加质量把关人"——你越懂业务，拆出来的场景越准，AI的产出就越有价值。说到底，AI接走的是记录这个动作，接不走的，是知道"什么值得被记录"的那双眼睛。</p>

<div class="tags">
  <div class="tag-row">适合读者：<span class="pill">高科技行业职场人</span><span class="pill">HR与团队管理者</span></div>
  <div class="tag-row">关键词：<span class="pill">经验萃取</span><span class="pill">智能体</span><span class="pill">组织记忆</span><span class="pill">知识库</span></div>
</div>
</div>
</div>
{{< /rawhtml >}}
