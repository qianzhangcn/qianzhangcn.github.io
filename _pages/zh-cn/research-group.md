---
layout: page
title: "课题组"
permalink: /research-group/
description:
nav: true
nav_order: 3
---

<style>

/* =========================================================
   页面基础：所有样式仅作用于课题组页面
   ========================================================= */

.ics-page {
  --ics-accent: var(--global-theme-color, #b509ac);
  --ics-text: var(--global-text-color, #222222);
  --ics-muted: var(--global-text-color-light, #6b7280);
  --ics-border: var(--global-divider-color, #e5e7eb);
  --ics-surface: var(--global-card-bg-color, var(--global-bg-color, #ffffff));

  width: 100%;
  max-width: 1120px;
  margin: 0 auto;
  padding-bottom: 40px;

  color: var(--ics-text);
  line-height: 1.8;
  overflow-wrap: break-word;
}

/* 英文优先使用 Times New Roman，中文使用后备中文字体 */

.ics-page,
.ics-page * {
  box-sizing: border-box;
  font-family: "Times New Roman", "Songti SC", "SimSun", serif !important;
}

.ics-page .en,
.ics-page .en * {
  font-family: "Times New Roman", Times, serif !important;
}

.ics-page a {
  color: var(--ics-accent);
}

.ics-page a:focus-visible {
  outline: 2px solid var(--ics-accent);
  outline-offset: 4px;
}


/* =========================================================
   首屏：左侧实验室介绍，右侧 Logo
   ========================================================= */

.ics-page .ics-hero {
  display: grid;
  grid-template-columns: minmax(0, 1fr) minmax(220px, 300px);
  align-items: center;
  gap: 36px;

  margin: 8px 0 40px;
  padding: 32px;

  border: 1px solid var(--ics-border);
  border-radius: 18px;
  background: var(--ics-surface);

  box-shadow: 0 6px 24px rgba(0, 0, 0, 0.035);
}

.ics-page .ics-hero-text {
  min-width: 0;
}

/* ICS Lab 标识 */

.ics-page .ics-hero-badge {
  display: inline-block;

  margin-bottom: 12px;
  padding: 3px 13px;

  border: 1px solid var(--ics-accent);
  border-radius: 999px;

  color: var(--ics-accent);
  font-size: 0.96rem;
  font-weight: 700;
  letter-spacing: 0.04em;
}

/* 实验室中文名称 */

.ics-page .ics-hero-title {
  margin: 0 0 8px;

  font-size: clamp(1.7rem, 2.8vw, 2.15rem);
  font-weight: 700;
  line-height: 1.4;
}

/* 实验室英文名称 */

.ics-page .ics-hero-subtitle {
  margin: 0 0 16px;

  color: var(--ics-muted);
  font-size: 1.02rem;
  line-height: 1.6;
}

/* 首屏简短介绍 */

.ics-page .ics-hero-lead {
  margin: 0 0 18px;

  font-size: 1rem;
  line-height: 1.9;
  text-align: left;
}

/* 研究主题标签 */

.ics-page .ics-hero-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
}

.ics-page .ics-hero-tag {
  display: inline-block;

  padding: 4px 11px;

  border: 1px solid var(--ics-border);
  border-radius: 7px;

  font-size: 0.88rem;
  line-height: 1.6;
}

/* 页面内导航按钮 */

.ics-page .ics-hero-actions {
  display: flex;
  flex-wrap: wrap;
  gap: 12px;

  margin-top: 22px;
}

.ics-page .ics-hero-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;

  min-height: 42px;
  padding: 7px 20px;

  border: 1px solid var(--ics-accent);
  border-radius: 8px;

  color: var(--ics-accent);
  font-size: 0.94rem;
  font-weight: 700;
  text-decoration: none;

  transition: box-shadow 0.2s ease;
}

.ics-page .ics-hero-button-primary {
  background: var(--ics-accent);
  color: var(--global-bg-color, #ffffff);
}

.ics-page .ics-hero-button:hover {
  text-decoration: none;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.09);
}

.ics-page .ics-hero-button-primary:hover {
  color: var(--global-bg-color, #ffffff);
}

/* Logo 区域：保持原图比例，避免占满整个首屏 */

.ics-page .ics-hero-logo-wrap {
  display: flex;
  align-items: center;
  justify-content: center;
  justify-self: end;

  width: 100%;
  max-width: 300px;
  padding: 10px;

  border-radius: 14px;
  background: #ffffff;
}

.ics-page .ics-logo {
  display: block;

  width: 100%;
  max-width: 280px;
  height: auto;

  margin: 0 auto;
  object-fit: contain;
}


/* =========================================================
   通用章节
   ========================================================= */

.ics-page .ics-section {
  margin: 42px 0 0;

  /* 点击首屏导航后，避免标题被固定导航栏遮挡 */
  scroll-margin-top: 100px;
}

.ics-page .ics-section-title {
  position: relative;

  margin: 0 0 22px;
  padding: 0 0 12px 17px;

  border-bottom: 2px solid var(--ics-border);

  font-size: 1.55rem;
  font-weight: 700;
  line-height: 1.45;
}

.ics-page .ics-section-title::before {
  content: "";
  position: absolute;

  top: 0.16em;
  left: 0;

  width: 5px;
  height: 1.05em;

  border-radius: 4px;
  background: var(--ics-accent);
}

.ics-page .ics-text {
  margin: 0 0 14px;

  font-size: 1.01rem;
  line-height: 1.9;
  text-align: justify;
}


/* =========================================================
   课题组简介
   ========================================================= */

.ics-page .ics-intro-box {
  padding: 26px 30px;

  border: 1px solid var(--ics-border);
  border-radius: 15px;

  background: var(--ics-surface);
  box-shadow: 0 5px 18px rgba(0, 0, 0, 0.035);
}

.ics-page .ics-intro-box .ics-text:last-child,
.ics-page .ics-section > .ics-text:last-child {
  margin-bottom: 0;
}


/* =========================================================
   ICS 核心价值
   ========================================================= */

.ics-page .ics-values {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 22px;

  margin-top: 24px;
}

.ics-page .ics-value-card {
  min-width: 0;
  padding: 26px 22px;

  border: 1px solid var(--ics-border);
  border-radius: 15px;

  background: var(--ics-surface);
  text-align: center;
}

.ics-page .ics-value-letter {
  margin-bottom: 10px;

  color: var(--ics-accent);
  font-size: 2.55rem;
  font-weight: 700;
  line-height: 1;
}

.ics-page .ics-value-title {
  margin-bottom: 5px;

  font-size: 1.25rem;
  font-weight: 700;
}

.ics-page .ics-value-cn {
  margin-bottom: 8px;

  font-size: 1.02rem;
  font-weight: 700;
}

.ics-page .ics-value-desc {
  color: var(--ics-muted);
  font-size: 0.94rem;
  line-height: 1.8;
}


/* =========================================================
   宗旨与目标
   ========================================================= */

.ics-page .ics-mission {
  margin-bottom: 22px;
  padding: 23px 27px;

  border-left: 4px solid var(--ics-accent);
  border-radius: 0 13px 13px 0;

  background: var(--ics-surface);
}

.ics-page .ics-mission-main {
  margin: 0;

  font-size: 1.1rem;
  font-weight: 700;
  line-height: 1.9;
}


/* =========================================================
   研究方向
   ========================================================= */

.ics-page .ics-research-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 18px;
}

.ics-page .ics-research-item {
  min-width: 0;
  padding: 20px 22px;

  border: 1px solid var(--ics-border);
  border-radius: 12px;

  background: var(--ics-surface);
}

.ics-page .ics-research-cn {
  margin-bottom: 5px;

  font-size: 1.02rem;
  font-weight: 700;
}

.ics-page .ics-research-en {
  color: var(--ics-muted);
  font-size: 0.95rem;
  line-height: 1.65;
}


/* =========================================================
   合作学者
   ========================================================= */

.ics-page .ics-visitor {
  display: grid;
  grid-template-columns: 160px minmax(0, 1fr);
  gap: 28px;
  align-items: center;

  margin-bottom: 22px;
  padding: 24px;

  border: 1px solid var(--ics-border);
  border-radius: 15px;

  background: var(--ics-surface);
}

.ics-page .ics-visitor:last-child {
  margin-bottom: 0;
}

.ics-page .ics-visitor-photo {
  display: block;

  width: 160px;
  max-width: 100%;
  height: 195px;

  margin: 0 auto;

  border-radius: 10px;

  object-fit: contain;
  object-position: center;
}

.ics-page .ics-visitor-name {
  margin-bottom: 5px;

  font-size: 1.22rem;
  font-weight: 700;
  line-height: 1.7;
}

.ics-page .ics-visitor-role {
  margin-bottom: 10px;

  color: var(--ics-accent);
  font-size: 0.95rem;
  font-weight: 700;
}

.ics-page .ics-visitor-desc {
  margin: 0;

  font-size: 0.97rem;
  line-height: 1.85;
  text-align: justify;
}


/* =========================================================
   学生卡片
   已合并：照片完整显示、照片上方和左右留白
   ========================================================= */

.ics-page .ics-members {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 25px;
  align-items: stretch;
}

.ics-page .ics-member-card {
  min-width: 0;

  /* 照片上方留白 24px，左右留白 20px */
  padding: 24px 20px 0;

  overflow: hidden;

  border: 1px solid var(--ics-border);
  border-radius: 15px;

  background: var(--ics-surface);
  text-align: center;
}

/* 固定照片展示区域，完整显示原图，不裁剪、不拉伸 */

.ics-page .ics-member-photo {
  display: block;

  width: 100%;
  height: 320px;
  max-height: none;

  margin: 0 auto;
  padding: 0;

  object-fit: contain;
  object-position: center;

  background: var(--ics-surface);
}

.ics-page .ics-member-info {
  padding: 18px 0 24px;
}

.ics-page .ics-member-name {
  margin: 0 0 5px;

  font-size: 1.18rem;
  font-weight: 700;
}

.ics-page .ics-member-role {
  display: inline-block;
  max-width: 100%;

  margin: 4px 0 9px;
  padding: 3px 12px;

  border: 1px solid var(--ics-accent);
  border-radius: 20px;

  color: var(--ics-accent);
  font-size: 0.87rem;
  font-weight: 700;
}

.ics-page .ics-member-status {
  margin: 3px 0;

  color: var(--ics-muted);
  font-size: 0.93rem;
  line-height: 1.75;
}


/* =========================================================
   页尾
   ========================================================= */

.ics-page .ics-ending {
  margin: 54px 0 0;
  padding: 28px 15px 8px;

  border-top: 1px solid var(--ics-border);
  text-align: center;
}

.ics-page .ics-ending-cn {
  font-size: 1.15rem;
  font-weight: 700;
}

.ics-page .ics-ending-en {
  margin-top: 5px;

  color: var(--ics-muted);
}


/* =========================================================
   交互效果
   不移动卡片，避免照片看起来上下错位
   ========================================================= */

.ics-page .ics-value-card,
.ics-page .ics-research-item,
.ics-page .ics-member-card {
  transition:
    border-color 0.2s ease,
    box-shadow 0.2s ease;
}

@media (hover: hover) and (pointer: fine) {

  .ics-page .ics-value-card:hover,
  .ics-page .ics-research-item:hover,
  .ics-page .ics-member-card:hover {
    border-color: var(--ics-accent);
    box-shadow: 0 7px 22px rgba(0, 0, 0, 0.06);
  }

}


/* =========================================================
   平板端
   ========================================================= */

@media screen and (max-width: 900px) {

  .ics-page .ics-hero {
    grid-template-columns: minmax(0, 1fr) 230px;
    gap: 24px;
    padding: 26px;
  }

  .ics-page .ics-hero-title {
    font-size: 1.8rem;
  }

  .ics-page .ics-members {
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }

  .ics-page .ics-research-grid {
    grid-template-columns: minmax(0, 1fr);
  }

}


/* =========================================================
   窄屏：首屏改为上下布局
   ========================================================= */

@media screen and (max-width: 760px) {

  .ics-page .ics-hero {
    grid-template-columns: minmax(0, 1fr);
    gap: 24px;
  }

  .ics-page .ics-hero-text {
    text-align: center;
  }

  .ics-page .ics-hero-lead {
    text-align: left;
  }

  .ics-page .ics-hero-tags,
  .ics-page .ics-hero-actions {
    justify-content: center;
  }

  .ics-page .ics-hero-logo-wrap {
    max-width: 240px;
    justify-self: center;
  }

  .ics-page .ics-values {
    grid-template-columns: minmax(0, 1fr);
  }

}


/* =========================================================
   手机端
   ========================================================= */

@media screen and (max-width: 620px) {

  .ics-page .ics-hero {
    padding: 22px 18px;
    margin-bottom: 32px;
    border-radius: 14px;
  }

  .ics-page .ics-hero-title {
    font-size: 1.65rem;
  }

  .ics-page .ics-hero-subtitle {
    font-size: 0.95rem;
  }

  .ics-page .ics-hero-lead {
    font-size: 0.97rem;
  }

  .ics-page .ics-hero-logo-wrap {
    max-width: 210px;
  }

  .ics-page .ics-section {
    margin-top: 34px;
  }

  .ics-page .ics-section-title {
    font-size: 1.35rem;
    margin-bottom: 18px;
  }

  .ics-page .ics-intro-box,
  .ics-page .ics-value-card,
  .ics-page .ics-research-item {
    padding: 20px 18px;
  }

  .ics-page .ics-mission {
    padding: 20px 18px;
  }

  .ics-page .ics-text,
  .ics-page .ics-visitor-desc {
    text-align: left;
  }

  .ics-page .ics-visitor {
    grid-template-columns: minmax(0, 1fr);
    gap: 18px;

    padding: 22px 18px;
    text-align: center;
  }

  .ics-page .ics-members {
    grid-template-columns: minmax(0, 1fr);

    width: 100%;
    max-width: 380px;
    margin: 0 auto;
  }

  .ics-page .ics-member-card {
    padding: 20px 16px 0;
  }

  .ics-page .ics-member-photo {
    height: 300px;
    max-height: none;
  }

  .ics-page .ics-ending {
    margin-top: 40px;
  }

}


/* =========================================================
   减少动态效果的系统偏好
   ========================================================= */

@media (prefers-reduced-motion: reduce) {

  .ics-page .ics-hero-button,
  .ics-page .ics-value-card,
  .ics-page .ics-research-item,
  .ics-page .ics-member-card {
    transition: none;
  }

}

</style>


<div class="ics-page" lang="zh-CN">


<!-- =========================================================
     首屏：左侧实验室介绍，右侧 Logo
     ========================================================= -->

<section class="ics-hero" aria-labelledby="ics-hero-title">

  <div class="ics-hero-text">

    <div class="ics-hero-badge en">
      ICS Lab
    </div>

    <h2 class="ics-hero-title" id="ics-hero-title">
      智能协同系统实验室
    </h2>

    <p class="ics-hero-subtitle en">
      Intelligent Cooperative Systems Laboratory
    </p>

    <p class="ics-hero-lead">
      以智能协作为核心，聚焦通信、感知与控制深度融合，
      面向未来智能无线网络与无人系统开展研究。
    </p>

    <div class="ics-hero-tags" aria-label="研究主题">

      <span class="ics-hero-tag">
        通感控一体化
      </span>

      <span class="ics-hero-tag">
        智能超表面
      </span>

      <span class="ics-hero-tag">
        无人机通信
      </span>

      <span class="ics-hero-tag">
        人工智能赋能通信
      </span>

    </div>

    <nav class="ics-hero-actions" aria-label="课题组页面导航">

      <a
        class="ics-hero-button ics-hero-button-primary"
        href="#ics-research">
        研究方向
      </a>

      <a
        class="ics-hero-button"
        href="#ics-members">
        团队成员
      </a>

    </nav>

  </div>


  <div class="ics-hero-logo-wrap">

    <img
      src="{{ '/assets/img/ICS_Lab_LOGO.png' | relative_url }}"
      class="ics-logo"
      alt="ICS Lab 智能协同系统实验室标志"
      decoding="async">

  </div>

</section>


<!-- =========================================================
     课题组简介
     ========================================================= -->

<section
  class="ics-section"
  id="ics-about"
  aria-labelledby="ics-about-title">

  <h2 class="ics-section-title" id="ics-about-title">
    课题组简介
  </h2>

  <div class="ics-intro-box">

    <p class="ics-text">
      <span class="en">ICS Lab</span>（智能协同系统实验室，
      <span class="en">Intelligent Cooperative Systems Laboratory</span>）
      聚焦未来智能无线系统中的通信、感知与控制深度融合，
      面向复杂动态环境下的智能信息获取、可靠连接与自主协同问题，
      开展基础理论、关键算法与系统应用研究。
    </p>

    <p class="ics-text">
      课题组以“智能协作”为核心，通过通信实现高效可靠的信息连接，
      通过感知实现对无线环境、目标状态及系统状态的理解，
      通过智能控制实现网络与无人系统的自主决策和协同行为，
      共同探索面向未来智能无线网络与无人系统的
      <span class="en">Integrated Communication, Sensing and Control Systems</span>。
    </p>

  </div>

</section>


<!-- =========================================================
     ICS 的内涵
     ========================================================= -->

<section
  class="ics-section"
  id="ics-values"
  aria-labelledby="ics-values-title">

  <h2 class="ics-section-title" id="ics-values-title">
    <span class="en">ICS</span> 的内涵
  </h2>

  <p class="ics-text">
    <span class="en">ICS</span>
    不仅代表课题组所关注的智能协同系统及通信、感知与控制融合研究，
    同时也体现课题组共同坚持的科研理念：
    <span class="en">Innovation, Collaboration, and Synergy</span>。
  </p>


  <div class="ics-values">

    <div class="ics-value-card">

      <div class="ics-value-letter en">I</div>

      <div class="ics-value-title en">
        Innovation
      </div>

      <div class="ics-value-cn">
        创新
      </div>

      <div class="ics-value-desc">
        坚持面向学科前沿和关键科学问题开展原创研究，
        鼓励提出新问题、探索新理论、设计新方法。
      </div>

    </div>


    <div class="ics-value-card">

      <div class="ics-value-letter en">C</div>

      <div class="ics-value-title en">
        Collaboration
      </div>

      <div class="ics-value-cn">
        合作
      </div>

      <div class="ics-value-desc">
        重视课题组协作、开放交流与相互支持，
        通过充分讨论与优势互补共同推进科研工作。
      </div>

    </div>


    <div class="ics-value-card">

      <div class="ics-value-letter en">S</div>

      <div class="ics-value-title en">
        Synergy
      </div>

      <div class="ics-value-cn">
        协同
      </div>

      <div class="ics-value-desc">
        促进不同成员和不同研究方向之间的协同融合，
        在共同探索中实现能力提升与持续成长。
      </div>

    </div>

  </div>

</section>


<!-- =========================================================
     课题组宗旨与目标
     ========================================================= -->

<section
  class="ics-section"
  id="ics-mission"
  aria-labelledby="ics-mission-title">

  <h2 class="ics-section-title" id="ics-mission-title">
    课题组宗旨与目标
  </h2>

  <div class="ics-mission">

    <p class="ics-mission-main">
      以智能协作为核心，通过通信连接、感知理解和智能控制，
      共同探索通信—感知—控制深度融合的未来智能系统。
    </p>

  </div>

  <p class="ics-text">
    课题组坚持问题驱动与前沿探索并重，注重基础理论、算法设计与实际应用的有机结合。
    我们希望围绕未来无线网络、低空智能网络、无人系统及智能协同系统中的关键问题，
    构建从理论建模、算法设计到系统验证的完整研究体系。
  </p>

  <p class="ics-text">
    在人才培养方面，课题组注重培养成员独立思考、科研创新、课题组合作与持续学习能力，
    鼓励成员在开放、严谨和相互支持的科研环境中不断探索，
    逐步形成具有长期发展潜力的研究方向和科研能力。
  </p>

</section>


<!-- =========================================================
     主要研究方向
     ========================================================= -->

<section
  class="ics-section"
  id="ics-research"
  aria-labelledby="ics-research-title">

  <h2 class="ics-section-title" id="ics-research-title">
    主要研究方向
  </h2>

  <div class="ics-research-grid">


    <div class="ics-research-item">

      <div class="ics-research-cn">
        通信感知一体化
      </div>

      <div class="ics-research-en en">
        Integrated Sensing and Communication (ISAC)
      </div>

    </div>


    <div class="ics-research-item">

      <div class="ics-research-cn">
        通信–感知–控制一体化
      </div>

      <div class="ics-research-en en">
        Integrated Communication, Sensing and Control
      </div>

    </div>


    <div class="ics-research-item">

      <div class="ics-research-cn">
        无人机通信与低空智能网络
      </div>

      <div class="ics-research-en en">
        UAV Communications and Low-Altitude Intelligent Networks
      </div>

    </div>


    <div class="ics-research-item">

      <div class="ics-research-cn">
        多无人系统智能协同
      </div>

      <div class="ics-research-en en">
        Intelligent Cooperation for Multi-UAV Systems
      </div>

    </div>


    <div class="ics-research-item">

      <div class="ics-research-cn">
        智能超表面与可重构无线环境
      </div>

      <div class="ics-research-en en">
        RIS / SIM and Reconfigurable Wireless Environments
      </div>

    </div>


    <div class="ics-research-item">

      <div class="ics-research-cn">
        人工智能赋能无线通信
      </div>

      <div class="ics-research-en en">
        Artificial Intelligence for Wireless Communications
      </div>

    </div>


  </div>

</section>


<!-- =========================================================
     合作学者
     ========================================================= -->

<section
  class="ics-section"
  id="ics-members"
  aria-labelledby="ics-members-title">

  <h2 class="ics-section-title" id="ics-members-title">
    合作学者
  </h2>

  <!-- ==================== 合作学者 1 ==================== -->

  <div class="ics-visitor">

    <img
      src="{{ '/assets/img/group/Hui_Wang.jpg' | relative_url }}"
      class="ics-visitor-photo"
      alt="王辉"
      loading="lazy"
      decoding="async">

    <div>

      <div class="ics-visitor-name">
        王辉
      </div>

      <div class="ics-visitor-role">
        合作学者 · 浙江大学
      </div>

      <p class="ics-visitor-desc">
        浙江大学良渚实验室博士后。2025年博士毕业于山东大学，主要研究方向包括脑机接口、语言解码、脑电大模型和图神经网络等，已在Expert Systems with Applications、IEEE Transactions on Affective Computing等期刊发表多篇论文。
      </p>

    </div>

  </div>

  <!-- ==================== 合作学者 2 ==================== -->

  <div class="ics-visitor">

    <img
      src="{{ '/assets/img/group/Yunxiao_Li.png' | relative_url }}"
      class="ics-visitor-photo"
      alt="李云潇"
      loading="lazy"
      decoding="async">

    <div>

      <div class="ics-visitor-name">
        李云潇
      </div>

      <div class="ics-visitor-role">
        合作学者 · 山东大学
      </div>

      <p class="ics-visitor-desc">
        山东大学在读博士生，主要研究方向包括通信感知一体化、流体天线、无人机轨迹优化、以及物理层安全。
      </p>

    </div>

  </div>


  <!-- ==================== 合作学者 3 ==================== -->

  <div class="ics-visitor">

    <img
      src="{{ '/assets/img/group/chengxuejun.jpg' | relative_url }}"
      class="ics-visitor-photo"
      alt="程学军"
      loading="lazy"
      decoding="async">

    <div>

      <div class="ics-visitor-name">
        程学军（<a href="https://scholar.google.com/citations?user=anxnepIAAAAJ&amp;hl=zh-CN">谷歌学术主页</a>）
      </div>

      <div class="ics-visitor-role">
        合作学者 · 山东大学
      </div>

      <p class="ics-visitor-desc">
        山东大学在读博士研究生，国家公派新加坡国立大学联培博士生，
        主要研究方向包括智能超表面波束赋形、通信感知一体化与多址技术。
      </p>

    </div>

  </div>


  <!-- ==================== 合作学者 4 ==================== -->

  <div class="ics-visitor">

    <img
      src="{{ '/assets/img/group/wangmaoyuan.png' | relative_url }}"
      class="ics-visitor-photo"
      alt="王茂源"
      loading="lazy"
      decoding="async">

    <div>

      <div class="ics-visitor-name">
        王茂源
      </div>

      <div class="ics-visitor-role">
        合作学者 · 山东大学
      </div>

      <p class="ics-visitor-desc">
        山东大学在读硕士研究生，
        主要研究方向包括柔性智能超表面、通信感知一体化与深度强化学习。
      </p>

    </div>

  </div>

  <!-- 增加合作学者时，在本 section 内复制一个完整的 .ics-visitor。 -->

</section>


<!-- =========================================================
     硕士研究生
     ========================================================= -->

<section
  class="ics-section"
  id="ics-masters"
  aria-labelledby="ics-masters-title">

  <h2 class="ics-section-title" id="ics-masters-title">
    硕士研究生
  </h2>

  <div class="ics-members">


    <!-- ==================== 硕士生空缺 ==================== -->

    <div class="ics-member-card">

      <img
        src="{{ '/assets/img/group/Master_Vacant.png' | relative_url }}"
        class="ics-member-photo"
        alt="硕士研究生名额空缺，尚未招录"
        loading="lazy"
        decoding="async">

      <div class="ics-member-info">

        <div class="ics-member-name">
          空缺
        </div>

        <div class="ics-member-role">
          硕士研究生
        </div>

        <div class="ics-member-status">
          2026级 · 待招录
        </div>

        <div class="ics-member-status">
          学术型/专业型硕士
        </div>

      </div>

    </div>

    <!-- 增加硕士生时，在本 .ics-members 内复制一个完整的 .ics-member-card。 -->

  </div>

</section>


<!-- =========================================================
     本科生
     ========================================================= -->

<section
  class="ics-section"
  id="ics-undergraduates"
  aria-labelledby="ics-undergraduates-title">

  <h2 class="ics-section-title" id="ics-undergraduates-title">
    本科生
  </h2>

  <div class="ics-members">


    <!-- ==================== 本科生 1 ==================== -->

    <div class="ics-member-card">

      <img
        src="{{ '/assets/img/group/Luhan_Wang.jpg' | relative_url }}"
        class="ics-member-photo"
        alt="王鹿涵"
        loading="lazy"
        decoding="async">

      <div class="ics-member-info">

        <div class="ics-member-name">
          王鹿涵
        </div>

        <div class="ics-member-role">
          本科生
        </div>

        <div class="ics-member-status">
          2025级 · 在读
        </div>

        <div class="ics-member-status">
          本科科研成员
        </div>

      </div>

    </div>


    <!-- ==================== 本科生 2 ==================== -->

    <div class="ics-member-card">

      <img
        src="{{ '/assets/img/group/Yilin_Wang.jpeg' | relative_url }}"
        class="ics-member-photo"
        alt="王奕霖"
        loading="lazy"
        decoding="async">

      <div class="ics-member-info">

        <div class="ics-member-name">
          王奕霖
        </div>

        <div class="ics-member-role">
          本科生
        </div>

        <div class="ics-member-status">
          2026级 · 在读
        </div>

        <div class="ics-member-status">
          本科科研成员
        </div>

      </div>

    </div>

    <!-- 增加本科生时，在本 .ics-members 内复制一个完整的 .ics-member-card。 -->

  </div>

</section>


<!-- =========================================================
     页尾
     ========================================================= -->

<div class="ics-ending">

  <div class="ics-ending-cn">
    创新 · 合作 · 协同成长
  </div>

  <div class="ics-ending-en en">
    Innovation · Collaboration · Synergy
  </div>

</div>


</div>



<style>

/* =========================================================
   两个导航按钮：默认透明背景、紫色文字和描边
   同时覆盖“研究方向”按钮原来的默认紫色填充
   ========================================================= */

.ics-page .ics-hero-actions .ics-hero-button {
  background: transparent;
  color: var(--ics-accent, #b509ac);
  border: 1px solid var(--ics-accent, #b509ac);

  box-shadow: none;
  text-decoration: none;

  transition:
    background-color 0.2s ease,
    color 0.2s ease;
}


/* =========================================================
   鼠标悬停：当前按钮变为紫色背景、白色文字
   移开鼠标后自动恢复
   ========================================================= */

@media (hover: hover) and (pointer: fine) {

  .ics-page .ics-hero-actions .ics-hero-button:hover {
    background: var(--ics-accent, #b509ac);
    color: #ffffff;
    border-color: var(--ics-accent, #b509ac);

    text-decoration: none;
  }

}


/* 键盘操作：保留焦点边框，不保持紫色填充 */

.ics-page .ics-hero-actions .ics-hero-button:focus-visible {
  outline: 2px solid var(--ics-accent, #b509ac);
  outline-offset: 4px;
}


/* 尊重系统的减少动态效果设置 */

@media (prefers-reduced-motion: reduce) {

  .ics-page .ics-hero-actions .ics-hero-button {
    transition: none;
  }

}

</style>












