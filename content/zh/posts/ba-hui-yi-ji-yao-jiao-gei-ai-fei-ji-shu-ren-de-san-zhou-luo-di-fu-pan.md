---
title: "把会议纪要交给AI：非技术人的三周落地复盘"
slug: "ba-hui-yi-ji-yao-jiao-gei-ai-fei-ji-shu-ren-de-san-zhou-luo-di-fu-pan"
date: 2026-09-26T15:00:00+08:00
draft: false
categories: ["ai-native"]
tags: ["AI Native", "会议纪要", "非技术人", "落地复盘", "AI工作流"]
description: "我这种支持多条业务线的HR，一周里将近一半时间在会里泡着。开会本身不可怕，可怕的是会后：纪要没人想写，写了没人细看，看的人也记不住自己认领过什么。我花了三周，把纪要这活交给AI跑了一遍，中间翻过几次车，今天把整个过程掰开讲讲。"
---

{{< rawhtml >}}
<div class="article-content">
<style>

  * { box-sizing: border-box; }
  .article-content {
    background: #FAFAFA;
    color: #171717;
    font-family: -apple-system, BlinkMacSystemFont, "PingFang SC", "Hiragino Sans GB", "Microsoft YaHei", "Segoe UI", sans-serif;
    margin: 0;
    padding: 0;
    -webkit-font-smoothing: antialiased;
  }
  .article-content-inner { margin: 0; padding: 2rem 1rem; }
  h1 {
    font-size: 2.25rem;
    line-height: 1.35;
    font-weight: 700;
    margin: 0 0 1.5rem;
    color: #171717;
  }
  h2 {
    font-size: 1.5rem;
    line-height: 1.5;
    font-weight: 700;
    color: #171717;
    border-left: 4px solid #0D9488;
    padding-left: 0.75rem;
    margin: 2.75rem 0 1.25rem;
  }
  p {
    margin: 0 0 1.25rem;
    text-align: justify;
  }
  .notice {
    background: #F0FDFA;
    border-left: 4px solid #14B8A6;
    border-radius: 4px;
    padding: 1rem 1.25rem;
    margin: 0 0 2rem;
    color: #134E4A;
    font-size: 0.95rem;
    line-height: 1.7;
  }
  .code-card {
    background: #F4F4F5;
    border: 1px solid #E4E4E7;
    border-radius: 6px;
    font-family: "SF Mono", Menlo, Consolas, monospace;
    padding: 1rem;
    margin: 1.5rem 0;
    font-size: 0.875rem;
    line-height: 1.7;
    color: #3F3F46;
    white-space: pre-wrap;
    word-break: break-word;
  }
  .meta {
    margin-top: 3rem;
    padding-top: 1.75rem;
    border-top: 1px solid #E4E4E7;
  }
  .meta-row {
    display: flex;
    flex-wrap: wrap;
    align-items: baseline;
    margin-bottom: 0.85rem;
  }
  .meta-label {
    flex: 0 0 auto;
    font-size: 0.9rem;
    color: #71717A;
    margin-right: 0.75rem;
    font-weight: 600;
  }
  .tag {
    display: inline-block;
    background: #F4F4F5;
    color: #71717A;
    border-radius: 999px;
    padding: 0.25rem 0.85rem;
    font-size: 0.85rem;
    margin: 0.25rem 0.4rem 0.25rem 0;
    line-height: 1.5;
  }
  a { color: #0D9488; text-decoration: none; }

</style>
<div class="article-content-inner">
<h1>把会议纪要交给AI：非技术人的三周落地复盘</h1>

<div class="notice">
本文案例与数据均做示意性处理，请勿对号入座。
</div>

<p>我这种支持多条业务线的HR，一周里将近一半时间在会里泡着。开会本身不可怕，可怕的是会后：纪要没人想写，写了没人细看，看的人也记不住自己认领过什么。我花了三周，把纪要这活交给AI跑了一遍，中间翻过几次车，今天把整个过程掰开讲讲。</p>

<h2>先想清楚：纪要的问题不是写得慢，是没人用</h2>

<p>以前的套路大家都熟：散会前指定一位同学记纪要，他当晚憋出一份流水账，三天后发到群里，从此无人点开。后来我琢磨明白了，纪要真正的价值就三样——定了什么、谁负责、截止什么时候。剩下的基本是气氛组内容。手写纪要的问题是，写的人很累，但这三样还经常记不全。所以把这事交给AI，本质上不是偷懒，是把人力从"记录"挪到"判断"上。判断，才是人该干的活。</p>

<h2>我的土办法，一共三步</h2>

<p>我没有追求全自动，先用手动方式把流程跑通，这比什么都重要。</p>

<p>第一步，转写。把会议录音转成文字，现在主流工具对中文会议的识别准确率已经够用，但人名和内部术语一定会错，这一步必须自己过一遍耳朵。</p>

<p>第二步，喂给AI做结构化。这一步的胜负手在提示词，我贴一下自己打磨过几版的版本：</p>

<div class="code-card">你是一个会议纪要助手。请根据下面的转写文本输出纪要，格式如下：
1. 会议结论：逐条列出，每条不超过两句话，只写真正达成的共识，没定下来的事不算结论。
2. 行动项：包含"事项 / 负责人 / 截止时间"三项。负责人没明确说的，标"待定"，不要替会上的人猜。
3. 悬而未决：列出讨论过但没有结论的话题，一句话一条。
注意：只基于文本本身，不要补充、推测或润色任何观点。转写里听不清的部分，标注[不确定]。</div>

<p>第三步，人工核对十分钟。重点核四样东西：名字、数字、金额、期限。别的内容错一点无伤大雅，这四样错一点就是事故。</p>

<h2>三周里踩的四个坑</h2>

<p>第一个坑，AI会"补齐"会议里没有的逻辑。有一次它把两个讨论过但毫无关联的话题，写成了一条因果关系，读起来特别顺，其实是编的。所以我后来在提示词里加了"不要补充、推测或润色"那句话。这句话看着多余，实际上是保命的。</p>

<p>第二个坑，行动项缺主或缺期限，AI会照单全收。会议文化里有大量"我们后续看看吧"这类话，AI老老实实全记下来，但这种项等于没有。我现在的做法是让它把模糊承诺单独标出来，逼着会上把话说死。这里有个意外的副作用：现在我们组的会，散会前必须每件事问一句"谁来做、什么时候交"，不然纪要上会很难看。会议纪律反而被这个工具管出来了。</p>

<p>第三个坑，敏感内容别往上放。涉及薪酬、人员调整、个人评价的会，我全程手写要点，或者干脆不录音。工具好用不等于什么都能放进去，这是底线问题，不是洁癖。另外录音前先跟与会人打个招呼，这一步省不得。</p>

<p>第四个坑，转写质量决定上限。方言重、抢话多、多人同时开口的会，转写出来一塌糊涂，AI再聪明也是白搭。这类会我反而回到手写关键点，工具不是万能钥匙。</p>

<h2>真正值钱的不是纪要，是会后那三天</h2>

<p>三周下来，写纪要的时间从一小时压到十五分钟，但这不是最大的收获。最大的变化是纪要变成了一份活的清单：每条行动项有主、有期限，下次开会前，我把上次的行动项贴回给AI，让它生成一张核对表，会上逐条过。逃不掉，也赖不掉。我们组一个例行会议的状态，从"聊了很多"慢慢变成了"关掉了很多"。</p>

<p>从HR的视角再往深看一层：当纪要这类程序性劳动被AI接走，每个人在会里的角色其实变了。以前你可以在会里走神，反正有别人记；现在纪要的质量取决于会上有没有把话说清楚——说不清楚的事，AI会诚实地把它暴露成"悬而未决"。某种意义上，AI在逼着我们的会议文化变得诚实。这个变化，比省下来的几十分钟重要得多。</p>

<p>如果你也想试，我的建议就一句：别一上来追求全自动。先用最笨的方式完整跑通一次，把提示词和核对习惯养出来，再谈自动化。工具会一直换，但"把话说清楚、把责任定死"这个内核，换什么工具都值钱。</p>

<div class="meta">
  <div class="meta-row">
    <span class="meta-label">适合读者</span>
    <span class="tag">高科技行业职场人</span>
    <span class="tag">经常组织或参与会议的非技术岗同学</span>
    <span class="tag">想把重复事务交给AI的HR同行</span>
  </div>
  <div class="meta-row">
    <span class="meta-label">关键词</span>
    <span class="tag">会议纪要</span>
    <span class="tag">AI工作流</span>
    <span class="tag">提示词设计</span>
    <span class="tag">行动项追踪</span>
    <span class="tag">非技术人AI实战</span>
  </div>
</div>
</div>
</div>
{{< /rawhtml >}}
