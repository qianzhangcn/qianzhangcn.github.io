---
layout: page
title: "Research Group"
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

/* Entire English page: Times New Roman */
.ics-page,
.ics-page *,
.ics-page p,
.ics-page div,
.ics-page span,
.ics-page h1,
.ics-page h2,
.ics-page h3,
.ics-page a,
.ics-page strong {
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
   Introduction
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
  font-size: 2.55rem;
  font-weight: 700;
  color: var(--global-theme-color);
  line-height: 1;
  margin-bottom: 10px;
}

.ics-value-title {
  font-size: 1.25rem;
  font-weight: 700;
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

.ics-research-title {
  font-weight: 650;
  font-size: 1.02rem;
  margin-bottom: 3px;
}

.ics-research-desc {
  font-size: 0.95rem;
  color: var(--global-text-color-light);
}


/* =========================================================
   Collaborative Scholars
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

.ics-ending-main {
  font-size: 1.15rem;
  font-weight: 600;
}

.ics-ending-sub {
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
     ICS Lab Logo
     ======================================================= -->

<div class="ics-hero">

  <img
    src="/assets/img/ICS_Lab_LOGO.jpeg"
    class="ics-logo"
    alt="ICS Lab">

</div>


<!-- =======================================================
     Group Introduction
     ======================================================= -->

<section class="ics-section">

  <h2 class="ics-section-title">Group Introduction</h2>

  <div class="ics-intro-box">

    <p class="ics-text">
      <strong>ICS Lab</strong>
      (<strong>Intelligent Cooperative Systems Laboratory</strong>)
      focuses on the deep integration of communications, sensing,
      and control in future intelligent wireless systems.
      Our research addresses intelligent information acquisition,
      reliable connectivity, autonomous decision-making,
      and cooperative operation in complex and dynamic environments,
      covering fundamental theory, advanced algorithms,
      and system-level applications.
    </p>

    <p class="ics-text">
      With <strong>intelligent cooperation</strong> as its core concept,
      the group investigates reliable information connectivity through communications,
      environment and system awareness through sensing,
      and autonomous decision-making and cooperation through intelligent control.
      Our long-term goal is to explore
      <strong>Integrated Communication, Sensing and Control Systems</strong>
      for future intelligent wireless networks and autonomous systems.
    </p>

  </div>

</section>


<!-- =======================================================
     Meaning of ICS
     ======================================================= -->

<section class="ics-section">

  <h2 class="ics-section-title">The Meaning of ICS</h2>

  <p class="ics-text">
    <strong>ICS</strong> not only represents our research vision in
    intelligent cooperative systems and integrated communication,
    sensing, and control, but also reflects the core values shared
    by our group:
    <strong>Innovation, Collaboration, and Synergy</strong>.
  </p>


  <div class="ics-values">


    <div class="ics-value-card">

      <div class="ics-value-letter">I</div>

      <div class="ics-value-title">
        Innovation
      </div>

      <div class="ics-value-desc">
        We pursue original research on fundamental and emerging scientific problems,
        encouraging new questions, new theories, and new methodologies.
      </div>

    </div>


    <div class="ics-value-card">

      <div class="ics-value-letter">C</div>

      <div class="ics-value-title">
        Collaboration
      </div>

      <div class="ics-value-desc">
        We value open communication, teamwork, and mutual support,
        and promote research progress through discussion and complementary expertise.
      </div>

    </div>


    <div class="ics-value-card">

      <div class="ics-value-letter">S</div>

      <div class="ics-value-title">
        Synergy
      </div>

      <div class="ics-value-desc">
        We encourage synergy among group members and research directions,
        enabling shared progress, mutual inspiration, and long-term growth.
      </div>

    </div>


  </div>

</section>


<!-- =======================================================
     Mission and Goals
     ======================================================= -->

<section class="ics-section">

  <h2 class="ics-section-title">Mission and Goals</h2>

  <div class="ics-mission">

    <p class="ics-mission-main">
      Centered on intelligent cooperation, we aim to explore future intelligent systems
      through reliable communication, comprehensive sensing,
      and intelligent control, with a particular focus on the deep integration
      of communication, sensing, and control.
    </p>

  </div>


  <p class="ics-text" style="margin-top:22px;">
    Our group combines problem-driven research with exploration of emerging technologies.
    We emphasize the integration of fundamental theory, algorithm design,
    and practical applications.
    Our research focuses on key challenges in future wireless networks,
    low-altitude intelligent networks, autonomous systems,
    and intelligent cooperative systems,
    with the goal of developing an integrated research framework
    from theoretical modeling and algorithm design to system validation.
  </p>


  <p class="ics-text">
    In student training, we emphasize independent thinking,
    research creativity, teamwork, and lifelong learning.
    We encourage every member to explore challenging research problems
    in an open, rigorous, and supportive environment,
    and to gradually establish independent research capabilities
    and sustainable research directions.
  </p>

</section>


<!-- =======================================================
     Research Areas
     ======================================================= -->

<section class="ics-section">

  <h2 class="ics-section-title">Research Areas</h2>

  <div class="ics-research-grid">


    <div class="ics-research-item">

      <div class="ics-research-title">
        Integrated Sensing and Communication
      </div>

      <div class="ics-research-desc">
        Integrated Sensing and Communication (ISAC)
      </div>

    </div>


    <div class="ics-research-item">

      <div class="ics-research-title">
        Integrated Communication, Sensing and Control
      </div>

      <div class="ics-research-desc">
        Communication-Sensing-Control Integration
      </div>

    </div>


    <div class="ics-research-item">

      <div class="ics-research-title">
        UAV Communications and Low-Altitude Intelligent Networks
      </div>

      <div class="ics-research-desc">
        UAV Communications and Networking
      </div>

    </div>


    <div class="ics-research-item">

      <div class="ics-research-title">
        Intelligent Cooperation for Multi-UAV Systems
      </div>

      <div class="ics-research-desc">
        Multi-UAV Cooperation and Autonomous Coordination
      </div>

    </div>


    <div class="ics-research-item">

      <div class="ics-research-title">
        Intelligent Metasurfaces and Reconfigurable Wireless Environments
      </div>

      <div class="ics-research-desc">
        RIS / SIM and Reconfigurable Wireless Environments
      </div>

    </div>


    <div class="ics-research-item">

      <div class="ics-research-title">
        Artificial Intelligence for Wireless Communications
      </div>

      <div class="ics-research-desc">
        AI-Enabled Wireless Communications and Optimization
      </div>

    </div>


  </div>

</section>


<!-- =======================================================
     Collaborative Scholars
     ======================================================= -->

<section class="ics-section">

  <h2 class="ics-section-title">Collaborative Scholars</h2>


  <!-- ==================== Scholar 1 ==================== -->

  <div class="ics-visitor">

    <img
      src="/assets/img/group/chengxuejun.jpg"
      class="ics-visitor-photo"
      alt="Xuejun Cheng">

    <div>

      <div class="ics-visitor-name">
        Xuejun Cheng (<a href="https://scholar.google.com/citations?user=anxnepIAAAAJ&hl=zh-CN">谷歌学术主页</a>)
      </div>

      <div class="ics-visitor-role">
        Collaborative Scholar · Shandong University
      </div>

      <p class="ics-visitor-desc">
        Xuejun Cheng is currently pursuing the Ph.D. degree at Shandong University
        and is a CSC-sponsored visiting Ph.D. student at the National University
        of Singapore.
        His research interests include intelligent metasurface beamforming,
        integrated sensing and communication, and multiple-access technologies.
      </p>

    </div>

  </div>


  <!-- ==================== Scholar 2 ==================== -->

  <div class="ics-visitor">

    <img
      src="/assets/img/group/wangmaoyuan.png"
      class="ics-visitor-photo"
      alt="Maoyuan Wang">

    <div>

      <div class="ics-visitor-name">
        Maoyuan Wang
      </div>

      <div class="ics-visitor-role">
        Collaborative Scholar · Shandong University
      </div>

      <p class="ics-visitor-desc">
        Maoyuan Wang is currently pursuing the Master's degree at Shandong University.
        His research interests include flexible intelligent metasurfaces,
        integrated sensing and communication,
        and deep reinforcement learning.
      </p>

    </div>

  </div>


</section>


<!-- =======================================================
     Master's Students
     ======================================================= -->

<section class="ics-section">

  <h2 class="ics-section-title">Master's Students</h2>

  <div class="ics-members">


    <!-- ==================== Master's Student 1 ==================== -->

    <div class="ics-member-card">

      <img
        src="/assets/img/group/master-01.jpg"
        class="ics-member-photo"
        alt="Vacant">

      <div class="ics-member-info">

        <div class="ics-member-name">
          Vacant
        </div>

        <div class="ics-member-role">
          Master's Student
        </div>

        <div class="ics-member-status">
          Class of 2026 · Vacant
        </div>

        <div class="ics-member-status">
          Academic Master's Program
        </div>

      </div>

    </div>


   

    </div>


  </div>

</section>


<!-- =======================================================
     Undergraduate Students
     ======================================================= -->

<section class="ics-section">

  <h2 class="ics-section-title">Undergraduate Students</h2>

  <div class="ics-members">


    <!-- ==================== Undergraduate Student 1 ==================== -->

    <div class="ics-member-card">

      <img
        src="/assets/img/group/Luhan_Wang.jpg"
        class="ics-member-photo"
        alt="Luhan Wang">

      <div class="ics-member-info">

        <div class="ics-member-name">
          Luhan Wang
        </div>

        <div class="ics-member-role">
          Undergraduate Student
        </div>

        <div class="ics-member-status">
          Class of 2025 · Current
        </div>

        <div class="ics-member-status">
          Undergraduate Research Member
        </div>

      </div>

    </div>


    <!-- ==================== Undergraduate Student 2 ==================== -->

    <div class="ics-member-card">

      <img
        src="/assets/img/group/Yilin_Wang.jpg"
        class="ics-member-photo"
        alt="Yilin Wang">

      <div class="ics-member-info">

        <div class="ics-member-name">
          Yilin Wang
        </div>

        <div class="ics-member-role">
          Undergraduate Student
        </div>

        <div class="ics-member-status">
          Class of 2026 · Current
        </div>

        <div class="ics-member-status">
          Undergraduate Research Member
        </div>

      </div>

    </div>


  </div>

</section>


<!-- =======================================================
     Ending
     ======================================================= -->

<div class="ics-ending">

  <div class="ics-ending-main">
    Innovation · Collaboration · Synergy
  </div>

  <div class="ics-ending-sub">
    Explore Together · Grow Together
  </div>

</div>


</div>
