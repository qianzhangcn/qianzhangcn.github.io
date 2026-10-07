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
   ICS Lab Research Group Page
   ========================================================= */

.ics-page {
  max-width: 1120px;
  margin: 0 auto;
  line-height: 1.8;
}

/* 所有英文统一 Times New Roman */
.ics-page .en,
.ics-page .en * {
  font-family: "Times New Roman", Times, serif !important;
}


/* =========================================================
   Hero
   ========================================================= */

.ics-hero {
  text-align: center;
  padding: 10px 20px 35px;
}

.ics-logo {
  width: min(320px, 88%);
  height: auto;
  display: block;
  margin: 0 auto 16px;
}

.ics-hero-title {
  margin: 0 0 4px;
  font-size: 2.1rem;
  font-weight: 700;
  letter-spacing: 0.02em;
}

.ics-hero-subtitle {
  margin: 0;
  font-size: 1.12rem;
  color: var(--global-text-color-light);
}


/* =========================================================
   Section
   ========================================================= */

.ics-section {
  margin: 46px 0;
}

.ics-section-title {
  font-size: 1.62rem;
  font-weight: 700;
  margin-bottom: 22px;
  padding-bottom: 10px;
  border-bottom: 2px solid var(--global-divider-color);
}

.ics-section-title::before {
  content: "";
  display: inline-block;
  width: 5px;
  height: 1.12em;
  background: var(--global-theme-color);
  margin-right: 11px;
  border-radius: 4px;
  vertical-align: -0.12em;
}

.ics-text {
  font-size: 1.01rem;
  text-align: justify;
  margin-bottom: 14px;
}


/* =========================================================
   Intro
   ========================================================= */

.ics-intro-box {
  background: var(--global-card-bg-color);
  border: 1px solid var(--global-divider-color);
  border-radius: 15px;
  padding: 28px 31px;
  box-shadow: 0 5px 18px rgba(0, 0, 0, 0.045);
}


/* =========================================================
   ICS Values
   ========================================================= */

.ics-values {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 22px;
  margin-top: 25px;
}

.ics-value-card {
  padding: 28px 22px 25px;
  text-align: center;
  border: 1px solid var(--global-divider-color);
  border-radius: 15px;
  background: var(--global-card-bg-color);
  transition: transform 0.25s ease, box-shadow 0.25s ease;
}

.ics-value-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 9px 25px rgba(0, 0, 0, 0.08);
}

.ics-value-letter {
  font-family: "Times New Roman", Times, serif;
  font-size: 2.55rem;
  font-weight: 700;
  color: var(--global-theme-color);
  line-height: 1;
  margin-bottom: 10px;
}

.ics-value-title {
  font-family: "Times New Roman", Times, serif;
  font-size: 1.25rem;
  font-weight: 700;
  margin-bottom: 5px;
}

.ics-value-cn {
  font-size: 1.02rem;
  font-weight: 650;
  margin-bottom: 8px;
}

.ics-value-desc {
  font-size: 0.93rem;
  color: var(--global-text-color-light);
  line-height: 1.7;
}


/* =========================================================
   Mission
   ========================================================= */

.ics-mission {
  border-left: 4px solid var(--global-theme-color);
  background: var(--global-card-bg-color);
  padding: 24px 29px;
  border-radius: 0 13px 13px 0;
}

.ics-mission-main {
  font-size: 1.10rem;
  font-weight: 600;
  line-height: 1.9;
  margin: 0;
}

 
/* =========================================================
   Research Areas
   ========================================================= */

.ics-research-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 18px;
}

.ics-research-item {
  border: 1px solid var(--global-divider-color);
  border-radius: 12px;
  padding: 20px 22px;
  background: var(--global-card-bg-color);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.ics-research-item:hover {
  transform: translateY(-3px);
  box-shadow: 0 7px 18px rgba(0, 0, 0, 0.06);
}

.ics-research-cn {
  font-weight: 650;
  font-size: 1.02rem;
  margin-bottom: 3px;
}

.ics-research-en {
  font-family: "Times New Roman", Times, serif;
  font-size: 0.95rem;
  color: var(--global-text-color-light);
}


/* =========================================================
   Visiting Scholars
   ========================================================= */

.ics-visitor {
  display: grid;
  grid-template-columns: 160px 1fr;
  gap: 28px;
  align-items: center;
  border: 1px solid var(--global-divider-color);
  border-radius: 15px;
  padding: 22px;
  margin-bottom: 22px;
  background: var(--global-card-bg-color);
}

.ics-visitor-photo {
  width: 160px;
  height: 195px;
  object-fit: cover;
  object-position: center top;
  border-radius: 10px;
}

.ics-visitor-name {
  font-size: 1.22rem;
  font-weight: 700;
  margin-bottom: 3px;
}

.ics-visitor-role {
  font-size: 0.95rem;
  color: var(--global-theme-color);
  font-weight: 600;
  margin-bottom: 9px;
}

.ics-visitor-status {
  font-size: 0.92rem;
  color: var(--global-text-color-light);
  margin-bottom: 8px;
}

.ics-visitor-desc {
  font-size: 0.97rem;
  margin: 0;
  line-height: 1.8;
  text-align: justify;
}


/* =========================================================
   Student Cards
   ========================================================= */

.ics-members {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 25px;
}

.ics-member-card {
  overflow: hidden;
  background: var(--global-card-bg-color);
  border: 1px solid var(--global-divider-color);
  border-radius: 15px;
  text-align: center;
  transition: transform 0.25s ease, box-shadow 0.25s ease;
}

.ics-member-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 9px 25px rgba(0, 0, 0, 0.08);
}

.ics-member-photo {
  width: 100%;
  height: 270px;
  object-fit: cover;
  object-position: center top;
  display: block;
}

.ics-member-info {
  padding: 18px 14px 21px;
}

.ics-member-name {
  font-size: 1.18rem;
  font-weight: 700;
  margin: 0 0 5px;
}

.ics-member-role {
  display: inline-block;
  padding: 3px 12px;
  margin: 4px 0 9px;
  border-radius: 20px;
  color: var(--global-theme-color);
  border: 1px solid var(--global-theme-color);
  font-size: 0.84rem;
  font-weight: 600;
}

.ics-member-status {
  font-size: 0.92rem;
  color: var(--global-text-color-light);
  margin: 2px 0;
}


/* =========================================================
   Ending
   ========================================================= */

.ics-ending {
  text-align: center;
  margin: 58px 0 25px;
  padding: 30px 15px 5px;
  border-top: 1px solid var(--global-divider-color);
}

.ics-ending-cn {
  font-size: 1.15rem;
  font-weight: 600;
}

.ics-ending-en {
  font-family: "Times New Roman", Times, serif;
  color: var(--global-text-color-light);
  margin-top: 4px;
}


/* =========================================================
   Responsive
   ========================================================= */

@media (max-width: 900px) {

  .ics-values {
    grid-template-columns: 1fr;
  }

  .ics-members {
    grid-template-columns: repeat(2, 1fr);
  }

  .ics-research-grid {
    grid-template-columns: 1fr;
  }

}

@media (max-width: 620px) {

  .ics-page {
    padding: 0 2px;
  }

  .ics-hero {
    padding: 5px 5px 25px;
  }

  .ics-logo {
    width: 280px;
    max-width: 80%;
  }

  .ics-members {
    grid-template-columns: 1fr;
  }

  .ics-member-photo {
    height: auto;
    max-height: 440px;
  }

  .ics-visitor {
    grid-template-columns: 1fr;
    text-align: center;
  }

  .ics-visitor-photo {
    margin: 0 auto;
  }

  .ics-visitor-desc {
    text-align: left;
  }

}

</style>


<div class="ics-page">


<!-- =======================================================
     实验室 Logo
     ======================================================= -->

<div class="ics-hero">

  <img
    src="/assets/img/ICS_Lab_LOGO.jpeg"
    class="ics-logo"
    alt="ICS Lab">

</div>


<!-- =======================================================
     课题组简介
     ======================================================= -->

<section class="ics-section">

  <h2 class="ics-section-title">课题组简介</h2>

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


<!-- =======================================================
     ICS 内涵
     ======================================================= -->

<section class="ics-section">

  <h2 class="ics-section-title"><span class="en">ICS</span> 的内涵</h2>

  <p class="ics-text">
    <span class="en">ICS</span> 不仅代表课题组所关注的智能协同系统及通信、感知与控制融合研究，
    同时也体现课题组共同坚持的科研理念：
    <span class="en">Innovation, Collaboration, and Synergy</span>。
  </p>


  <div class="ics-values">


    <div class="ics-value-card">

      <div class="ics-value-letter">I</div>

      <div class="ics-value-title">
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

      <div class="ics-value-letter">C</div>

      <div class="ics-value-title">
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

      <div class="ics-value-letter">S</div>

      <div class="ics-value-title">
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


<!-- =======================================================
     课题组宗旨与目标
     ======================================================= -->

<section class="ics-section">

  <h2 class="ics-section-title">课题组宗旨与目标</h2>

  <div class="ics-mission">

    <p class="ics-mission-main">
      以智能协作为核心，通过通信连接、感知理解和智能控制，
      共同探索通信—感知—控制深度融合的未来智能系统。
    </p>

  </div>

  <p class="ics-text" style="margin-top:22px;">
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


<!-- =======================================================
     主要研究方向
     ======================================================= -->

<section class="ics-section">

  <h2 class="ics-section-title">主要研究方向</h2>

  <div class="ics-research-grid">


    <div class="ics-research-item">

      <div class="ics-research-cn">
        通信感知一体化
      </div>

      <div class="ics-research-en">
        Integrated Sensing and Communication (ISAC)
      </div>

    </div>


    <div class="ics-research-item">

      <div class="ics-research-cn">
        通信–感知–控制一体化
      </div>

      <div class="ics-research-en">
        Integrated Communication, Sensing and Control
      </div>

    </div>


    <div class="ics-research-item">

      <div class="ics-research-cn">
        无人机通信与低空智能网络
      </div>

      <div class="ics-research-en">
        UAV Communications and Low-Altitude Intelligent Networks
      </div>

    </div>


    <div class="ics-research-item">

      <div class="ics-research-cn">
        多无人系统智能协同
      </div>

      <div class="ics-research-en">
        Intelligent Cooperation for Multi-UAV Systems
      </div>

    </div>


    <div class="ics-research-item">

      <div class="ics-research-cn">
        智能超表面与可重构无线环境
      </div>

      <div class="ics-research-en">
        RIS / SIM and Reconfigurable Wireless Environments
      </div>

    </div>


    <div class="ics-research-item">

      <div class="ics-research-cn">
        人工智能赋能无线通信
      </div>

      <div class="ics-research-en">
        Artificial Intelligence for Wireless Communications
      </div>

    </div>


  </div>

</section>


<!-- =======================================================
     合作学者
     ======================================================= -->

<section class="ics-section">

  <h2 class="ics-section-title">合作学者</h2>


  <!-- ==================== 合作学者 1 ==================== -->

  <div class="ics-visitor">

    <img
      src="/assets/img/group/chengxuejun.jpg"
      class="ics-visitor-photo"
      alt="程学军">

    <div>

      <div class="ics-visitor-name">
        程学军（<a href="https://scholar.google.com/citations?user=anxnepIAAAAJ&hl=zh-CN">谷歌学术主页</a>）
      </div>

      <div class="ics-visitor-role">
        合作学者 · 山东大学
      </div>

      <!--
      <div class="ics-visitor-status">
        访问时间：2026年XX月－2026年XX月
      </div>
      -->

      <p class="ics-visitor-desc">
        山东大学在读博士研究生，国家公派新加坡国立大学联培博士生，主要研究方向包括智能超表面波束赋形、通信感知一体化与多址技术。
      </p>

    </div>

  </div>

  <!-- ==================== 访问学者 2 ==================== -->

  <div class="ics-visitor">

    <img
      src="/assets/img/group/wangmaoyuan.png"
      class="ics-visitor-photo"
      alt="王茂源">

    <div>

      <div class="ics-visitor-name">
        王茂源
      </div>

      <div class="ics-visitor-role">
        合作学者 · 山东大学
      </div>

      <!--
      <div class="ics-visitor-status">
        访问时间：2026年XX月－2026年XX月
      </div>
      -->

      <p class="ics-visitor-desc">
        山东大学在读硕士研究生，主要研究方向包括柔性智能超表面、通信感知一体化与深度强化学习。
      </p>

    </div>

  </div>


  <!--
  如果有第二位访问学者，复制下面这一段并取消注释。

  <div class="ics-visitor">

    <img
      src="/assets/img/group/visitor-02.jpg"
      class="ics-visitor-photo"
      alt="访问学者姓名">

    <div>

      <div class="ics-visitor-name">
        访问学者姓名
      </div>

      <div class="ics-visitor-role">
        访问学者 · XXXX大学
      </div>

      <div class="ics-visitor-status">
        访问时间：2026年XX月－2026年XX月
      </div>

      <p class="ics-visitor-desc">
        主要从事 XXXX 方向研究。
        访问期间重点围绕 XXXX 开展合作研究与学术交流。
      </p>

    </div>

  </div>
  -->


</section>


<!-- =======================================================
     硕士研究生
     ======================================================= -->

<section class="ics-section">

  <h2 class="ics-section-title">硕士研究生</h2>

  <div class="ics-members">


    <!-- ==================== 硕士生 1 ==================== -->

    <div class="ics-member-card">

      <img
        src="/assets/img/group/master-01.jpg"
        class="ics-member-photo"
        alt="空缺">

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

    

    </div>


    <!--
    如果有第 2 位硕士生，直接复制一个 .ics-member-card 即可。
    -->


  </div>

</section>


<!-- =======================================================
     本科生
     ======================================================= -->

<section class="ics-section">

  <h2 class="ics-section-title">本科生</h2>

  <div class="ics-members">


    <!-- ==================== 本科生 1 ==================== -->

    <div class="ics-member-card">

      <img
        src="/assets/img/group/Luhan_Wang.jpg"
        class="ics-member-photo"
        alt="王鹿涵">

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
        src="/assets/img/group/Yilin_Wang.jpg"
        class="ics-member-photo"
        alt="王奕霖">

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


    </div>


    <!--
    如果还有更多本科生，直接复制一个 .ics-member-card 即可。
    -->


</section>


<!-- =======================================================
     Ending
     ======================================================= -->

<div class="ics-ending">

  <div class="ics-ending-cn">
    创新 · 合作 · 协同成长
  </div>

  <div class="ics-ending-en">
    Innovation · Collaboration · Synergy
  </div>

</div>


