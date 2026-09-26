---
title: "给智能体写一份岗位说明书，比Prompt技巧管用"
slug: "gei-zhi-neng-ti-xie-yi-fen-gang-wei-shuo-ming-shu-bi-prompt-ji-qiao-guan-yong"
date: 2026-10-01T15:00:00+08:00
draft: false
categories: ["ai-native"]
tags: ["AI Native", "智能体", "岗位说明书", "Prompt", "Agent设计"]
description: "这两年我陆陆续续搭了不少智能体：简历初筛的、会议纪要的、培训需求调研的。有一阵子我特别热衷收集Prompt技巧，什么“给它一个身份”、“让它一步步思考”，每一条都认真试过。效果嘛，时好时坏，好一阵坏一阵，我也说不清为什么。直到有一次，我盯着屏幕上又一份格式全错的初筛报告，突然愣住了：这个场景我太熟了..."
---

{{< rawhtml >}}
<div class="article-content">
<style>

  * { margin: 0; padding: 0; box-sizing: border-box; }
  .article-content {
    background: #FAFAFA;
    color: #171717;
    font-family: -apple-system, BlinkMacSystemFont, "PingFang SC", "Hiragino Sans GB", "Microsoft YaHei", sans-serif;
    line-height: 1.8;
  }
  .article-content-inner { margin: 0; padding: 2rem 1rem; }
  h1 { font-size: 2.25rem; line-height: 1.45; font-weight: 700; margin-bottom: 2rem; }
  h2 {
    font-size: 1.5rem;
    line-height: 1.6;
    font-weight: 600;
    border-left: 4px solid #0D9488;
    padding-left: 0.75rem;
    margin: 2.6rem 0 1rem;
  }
  p { margin-bottom: 1.1rem; }
  .notice {
    background: #F0FDFA;
    border-left: 4px solid #14B8A6;
    padding: 1rem 1.25rem;
    border-radius: 0 6px 6px 0;
    color: #134E4A;
    font-size: 0.95rem;
    margin-bottom: 2.2rem;
  }
  pre {
    background: #F4F4F5;
    border: 1px solid #E4E4E7;
    border-radius: 6px;
    padding: 1rem;
    font-family: "SF Mono", Menlo, Consolas, "Courier New", monospace;
    font-size: 0.85rem;
    line-height: 1.7;
    overflow-x: auto;
    white-space: pre-wrap;
    word-break: break-word;
    margin: 1.25rem 0 1.5rem;
  }
  strong { color: #0D9488; font-weight: 600; }
  .tags { margin-top: 3rem; }
  .tag-row { display: flex; flex-wrap: wrap; gap: 0.6rem; align-items: baseline; margin-bottom: 0.8rem; }
  .tag-label { flex: 0 0 auto; font-size: 0.85rem; color: #71717A; }
  .pills { display: flex; flex-wrap: wrap; gap: 0.4rem; }
  .pill {
    background: #F4F4F5;
    color: #71717A;
    border-radius: 9999px;
    padding: 0.15rem 0.8rem;
    font-size: 0.8rem;
    display: inline-block;
  }

</style>
<div class="article-content-inner">
<h1>给智能体写一份岗位说明书，比Prompt技巧管用</h1>

<div class="notice">本文案例与数据均做示意性处理，请勿对号入座。</div>

<p>这两年我陆陆续续搭了不少智能体：简历初筛的、会议纪要的、培训需求调研的。有一阵子我特别热衷收集Prompt技巧，什么“给它一个身份”、“让它一步步思考”，每一条都认真试过。效果嘛，时好时坏，好一阵坏一阵，我也说不清为什么。直到有一次，我盯着屏幕上又一份格式全错的初筛报告，突然愣住了：这个场景我太熟了。这不就是招了个新员工，入职第一天什么都没交代，就让人直接上手干活吗？我干了这么多年HR，遇到这种情况的第一反应就是——岗位说明书没给。</p>

<h2>一、Prompt时好时坏，根子在没讲清楚“这个岗位是干嘛的”</h2>

<p>市面上大部分Prompt技巧，教的都是“怎么说话”：要具体、要举例、要分步骤。这些没错，但它们全都建立在同一个前提上——你已经想清楚了要让智能体干什么。现实是，多数人恰恰没想清楚。</p>

<p>这就跟招聘一个道理。JD写得含糊，面试官再会问问题，也容易招错人；JD写得清楚，哪怕面试官水平一般，踩坑的概率也会小很多。智能体也一样，它不是不够聪明，而是我们在布置工作的时候，自己脑子里还是一团浆糊。技巧解决的是表达问题，岗位说明书解决的是想清楚的问题。顺序反了，再好的技巧也是白搭。</p>

<h2>二、我把写JD的老办法，原样搬给了智能体</h2>

<p>写岗位说明书有几样经典要素：岗位目标、职责边界、汇报关系、任职要求、考核标准。我照着这个框架，给简历初筛的智能体重写了一份“说明书”，大意是这样的：</p>

<pre>【岗位名称】简历初筛助理
【岗位目标】从每天新到的简历中，筛出符合岗位要求的候选人，供HR复核
【职责边界】只做初筛打分和理由说明；不做最终录用判断；不直接回复候选人
【汇报关系】每天上午向HR提交初筛清单，按“推荐 / 待定 / 不推荐”三档标注并附理由
【任职要求】依据《岗位画像模板》和《筛选标准库》工作；材料不全时标注“信息不足”
【考核标准】初筛遗漏率低于5%；每份简历给出不超过三条理由；拿不准的必须标“待定”，不许猜</pre>

<p>改完之后，变化最明显的其实不是输出质量——质量本来就不算差——而是<strong>稳定</strong>。以前十次里总有那么两三次格式跑偏、口径不一，现在基本没有了。原因想通了也简单：以前我只告诉它“做什么”，没告诉它“做到什么程度算好”、“哪些事不该碰”。人缺了这两样会瞎猜，智能体缺了这两样，猜得比人还起劲。</p>

<h2>三、真正难写的，是“边界”和“考核标准”这两段</h2>

<p>目标好写，一句话的事。难的是边界。我踩过一个实打实的坑：最早我图省事，让初筛智能体“顺便”给候选人排个优先级，后来复核时发现，它排序的依据里混进了年龄、性别这类根本不该碰的信息。不是它学坏了，是我没把边界画清楚——你没说不行，它就默认行。做过员工关系的同事应该都有体会，制度里没写死的那部分，永远是最危险的部分。对智能体来说更是如此，因为它执行得比任何新员工都彻底。</p>

<p>考核标准也难。“初筛遗漏率低于5%”这一条，不是我提前想出来的，而是被业务部门追着问“AI筛掉的简历里有没有漏掉的好人”之后，倒逼着补上的。有意思的是，补上之后还有个意外收获：智能体遇到两头简历都沾边的候选人，会主动标“待定”并说明纠结点，而不是硬给一个答案。你看，把标准讲清楚，它反而更敢承认自己拿不准。这个规律，跟带团队一模一样。</p>

<h2>四、别忘了给它留一条“求助通道”</h2>

<p>还有一个教训：说明书写得太满，智能体就什么都想答，答不上来也硬编。后来我在任职要求里固定加了一条——遇到材料不全或拿不准的，标注“信息不足”并提交给HR处理，不要自行补全。这一条本质上就是我做员工关系时常讲的那句话：允许下属说“我处理不了”，比逼着他硬撑，要安全得多。智能体不会累，但它会一本正经地编。这条求助通道，就是给它装的安全阀。</p>

<h2>写在最后</h2>

<p>这一路折腾下来，我最大的体会是：管理智能体和管理人，底层逻辑惊人地一致，都逃不过“把期望讲清楚”这六个字。区别只在于，人会察言观色、会主动补位，智能体只会老老实实按你写的执行。所以在某种意义上，智能体是一面镜子：它输出的每一次混乱、每一次跑偏，照出来的都是我们自己没想明白的地方。</p>

<p>写岗位说明书这件事，我写了十几年，以前觉得是案头苦差，现在换了个对象接着写，越写越觉得，这门手艺在AI时代不但没有贬值，反而更值钱了。下一次如果你搭的智能体总是不听话，先别急着换技巧，试试给它写份岗位说明书——毕竟，把人用好的经验，大概率也把机器用得好。</p>

<div class="tags">
  <div class="tag-row">
    <span class="tag-label">适合读者：</span>
    <span class="pills">
      <span class="pill">非技术背景的高科技行业职场人</span>
      <span class="pill">想搭智能体的HR</span>
      <span class="pill">总觉得AI不好用的运营同学</span>
    </span>
  </div>
  <div class="tag-row">
    <span class="tag-label">关键词：</span>
    <span class="pills">
      <span class="pill">智能体</span>
      <span class="pill">岗位说明书</span>
      <span class="pill">Prompt设计</span>
      <span class="pill">人机分工</span>
      <span class="pill">非技术人AI实战</span>
    </span>
  </div>
</div>
</div>
</div>
{{< /rawhtml >}}
