---
page_id: about
layout: about
title: "个人主页"
permalink: /
subtitle: >
  <br>

selected_papers: false
social: false

announcements:
  enabled: false

latest_posts:
  enabled: false
---

<style>

/* =========================================================
   Global
   ========================================================= */

html,
body {
  overflow-x: hidden;
}

.profile-page {
  max-width: 1120px;
  margin: 0 auto;
  line-height: 1.8;
}

/* 英文统一 Times New Roman */
.profile-page .en,
.profile-page .en * {
  font-family: "Times New Roman", Times, serif !important;
}


/* =========================================================
   Top Header
   ========================================================= */

.profile-top {
  display: grid;
  grid-template-columns: 190px 1fr 190px;
  gap: 34px;
  align-items: center;

  margin-top: 8px;
  margin-bottom: 26px;

  padding: 24px 0 18px;
}

.profile-photo-wrap {
  text-align: center;
}

.profile-photo {
  width: 190px;
  max-width: 100%;
  height: auto;
  display: block;
  margin: 0 auto;

  border-radius: 8px;
  box-shadow: 0 6px 18px rgba(0,0,0,0.08);
}

.profile-info {
  min-width: 0;
  font-size: 1rem;
  line-height: 2;
}

.profile-info-row {
  display: flex;
  align-items: baseline;
  gap: 8px;
  margin: 4px 0;
}

.profile-info-label {
  min-width: 72px;
  font-weight: 600;
}

.profile-logo-wrap {
  text-align: center;
}

.profile-logo {
  width: 175px;
  max-width: 100%;
  height: auto;
  display: block;
  margin: 0 auto;
}


/* =========================================================
   Name & Welcome
   ========================================================= */

.profile-name {
  margin: 4px 0 4px;
  font-size: 2.05rem;
  font-weight: 700;
}

.profile-welcome {
  margin: 0 0 26px;
  font-size: 1rem;
  color: var(--global-text-color-light);
}


/* =========================================================
   Section
   ========================================================= */

.profile-section {
  margin: 44px 0;
}

.profile-section-title {
  font-size: 1.62rem;
  font-weight: 700;

  margin-bottom: 22px;
  padding-bottom: 10px;

  border-bottom: 2px solid var(--global-divider-color);
}

.profile-section-title::before {
  content: "";
  display: inline-block;

  width: 5px;
  height: 1.12em;

  margin-right: 11px;

  border-radius: 4px;
  background: var(--global-theme-color);

  vertical-align: -0.12em;
}

.profile-text p {
  text-align: justify;
  text-align-last: left;
  text-justify: inter-character;

  line-height: 1.85;

  margin-top: 0;
  margin-bottom: 1.25em;
}


/* =========================================================
   Intro Card
   ========================================================= */

.profile-intro-card {
  background: var(--global-card-bg-color);

  border: 1px solid var(--global-divider-color);
  border-radius: 14px;

  padding: 28px 30px;

  box-shadow: 0 5px 18px rgba(0,0,0,0.045);
}


/* =========================================================
   Timeline
   ========================================================= */

.timeline {
  display: flex;
  flex-direction: column;
  gap: 18px;
}

.timeline-item {
  display: grid;
  grid-template-columns: 165px 1fr;
  gap: 24px;

  padding: 18px 20px;

  border: 1px solid var(--global-divider-color);
  border-radius: 12px;

  background: var(--global-card-bg-color);
}

.timeline-date {
  font-family: "Times New Roman", Times, serif;
  font-weight: 700;
  color: var(--global-theme-color);
}

.timeline-main {
  font-weight: 600;
}

.timeline-sub {
  margin-top: 3px;
  font-size: 0.94rem;
  color: var(--global-text-color-light);
}


/* =========================================================
   Research Tags
   ========================================================= */

.research-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
}

.research-tag {
  display: inline-block;

  padding: 7px 14px;

  border: 1px solid var(--global-theme-color);
  border-radius: 999px;

  color: var(--global-theme-color);

  font-size: 0.94rem;
  font-weight: 600;

  background: var(--global-card-bg-color);
}


/* =========================================================
   Service Cards
   ========================================================= */

.service-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 16px;
}

.service-card {
  padding: 18px 20px;

  border: 1px solid var(--global-divider-color);
  border-radius: 12px;

  background: var(--global-card-bg-color);
}


/* =========================================================
   Publications
   ========================================================= */

.pub-note {
  margin-bottom: 20px;

  padding: 14px 18px;

  border-left: 4px solid var(--global-theme-color);
  background: var(--global-card-bg-color);

  border-radius: 0 10px 10px 0;
}

.pub-item {
  margin-bottom: 20px;

  padding: 18px 20px;

  border: 1px solid var(--global-divider-color);
  border-radius: 12px;

  background: var(--global-card-bg-color);
}

.pub-index {
  font-family: "Times New Roman", Times, serif;
  font-weight: 700;
  color: var(--global-theme-color);
}

.pub-text {
  line-height: 1.75;
}


/* =========================================================
   Patent
   ========================================================= */

.patent-list {
  display: flex;
  flex-direction: column;
  gap: 14px;
}

.patent-item {
  padding: 16px 18px;

  border: 1px solid var(--global-divider-color);
  border-radius: 11px;

  background: var(--global-card-bg-color);
}


/* =========================================================
   Awards
   ========================================================= */

.award-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 14px 18px;
}

.award-item {
  padding: 15px 17px;

  border: 1px solid var(--global-divider-color);
  border-radius: 11px;

  background: var(--global-card-bg-color);
}


/* =========================================================
   Cooperation
   ========================================================= */

.coop-box {
  padding: 24px 28px;

  border-left: 4px solid var(--global-theme-color);
  border-radius: 0 12px 12px 0;

  background: var(--global-card-bg-color);
}


/* =========================================================
   Visitor Counter
   ========================================================= */

.visit-counter {
  text-align: center;

  margin-top: 48px;
  padding-top: 22px;

  border-top: 1px solid var(--global-divider-color);

  font-size: 0.9rem;
  color: var(--global-text-color-light);
}


/* =========================================================
   Responsive
   ========================================================= */

@media screen and (max-width: 900px) {

  .profile-top {
    grid-template-columns: 170px 1fr;
  }

  .profile-logo-wrap {
    grid-column: 1 / -1;
  }

  .profile-logo {
    width: 155px;
  }

  .service-grid,
  .award-grid {
    grid-template-columns: 1fr;
  }

}

@media screen and (max-width: 650px) {

  .container,
  .container.mt-5 {
    width: 100% !important;
    max-width: 100% !important;

    padding-left: 18px !important;
    padding-right: 18px !important;
  }

  .profile-top {
    grid-template-columns: 1fr;
    gap: 18px;

    text-align: center;
  }

  .profile-photo {
    width: 190px;
  }

  .profile-logo {
    display: none;
  }

  .profile-info {
    text-align: left;
  }

  .profile-info-row {
    display: block;
  }

  .profile-info-label {
    display: inline;
    min-width: 0;
  }

  .timeline-item {
    grid-template-columns: 1fr;
    gap: 5px;
  }

  .profile-section {
    margin: 36px 0;
  }

  .profile-section-title {
    font-size: 1.4rem;
  }

}

</style>


<div class="profile-page">


<!-- =========================================================
     顶部个人信息
     ========================================================= -->

<div class="profile-top">

  <div class="profile-photo-wrap">
    <img
      src="{{ '/assets/img/Qian_Zhang_GitHub_2.png' | relative_url }}"
      class="profile-photo"
      alt="Qian Zhang">
  </div>


  <div class="profile-info">

      <div class="profile-info-row">
        <span class="profile-info-label">学　　校：</span>
        <span>东北大学秦皇岛分校</span>
      </div>
      
      <div class="profile-info-row">
        <span class="profile-info-label">学　　院：</span>
        <span>计算机与通信工程学院</span>
      </div>
      
      <div class="profile-info-row">
        <span class="profile-info-label">职　　称：</span>
        <span>副教授</span>
      </div>
      
      <div class="profile-info-row">
        <span class="profile-info-label">学　　历：</span>
        <span>工学博士</span>
      </div>
      
      <div class="profile-info-row">
        <span class="profile-info-label">毕业院校：</span>
        <span>山东大学</span>
      </div>
      
      <div class="profile-info-row">
        <span class="profile-info-label">邮　　箱：</span>
        <span class="en">zq869054246@163.com</span>
      </div>

  </div>


  <div class="profile-logo-wrap">
    <img
      src="{{ '/assets/img/Northeastern_University.png' | relative_url }}"
      class="profile-logo"
      alt="ICS Logo">
  </div>

</div>


<!-- =========================================================
     姓名
     ========================================================= -->

<h1 class="profile-name">张迁</h1>

<p class="profile-welcome">
  欢迎访问我的个人主页！
  （<a href="https://scholar.google.com/citations?user=hs8KAR4AAAAJ&hl=zh-CN">谷歌学术主页</a>）
</p>


<!-- =========================================================
     基本信息
     ========================================================= -->

<section class="profile-section">

  <h2 class="profile-section-title">👨‍🏫 基本信息</h2>

  <div class="profile-intro-card profile-text">

    <p>
      <strong>张迁</strong>，<strong>工学博士</strong>，<strong>副教授</strong>，
      <strong>硕士生导师</strong>，<span class="en">IEEE Member</span>，
      中国通信学会会员，<span class="en">CSIG</span>交通视频专委会委员。
      2026年6月于山东大学获得工学博士学位（直博），师从刘琚教授（二级），
      合作导师董郑教授；2024年受<strong>国家留学基金委资助</strong>赴新加坡南洋理工大学
      <span class="en">EEE</span>学院联合培养，
      师从<span class="en">Prof. Yong Liang Guan</span>（副校长）和
      <span class="en">Prof. Chau Yuen</span>（<span class="en">IEEE Fellow</span>）。
    </p>

    <p>
      目前主要从事智能超表面、凸优化理论、人工智能算法在无线通信和感知领域应用的相关研究。
      在通信领域顶级期刊
      <span class="en">IEEE TWC</span>、<span class="en">TCOM</span>
      和顶级会议
      <span class="en">IEEE ICC</span>、<span class="en">ICASSP</span>
      等发表学术论文30余篇，其中
      <strong>第一/共一/通讯作者论文18篇</strong>。
      2篇论文入选<strong>🏆 ESI高被引论文</strong>（一作），
      1篇论文位列<strong><span class="en">IEEE CL</span>年度最受欢迎论文 TOP 2</strong>（一作），
      4篇论文分别位列
      <strong><span class="en">IEEE TVT</span>、<span class="en">WCL</span>、<span class="en">CL</span>月度最受欢迎论文 TOP 50</strong>
      （1篇一作、2篇共一、1篇第二）。
      授权专利3项。
    </p>

    <p>
      担任《中国通信》（英文版）首届青年编委，
      担任<span class="en">2026 PIMRC TPC Chair</span>；
      多次担任<span class="en">IEEE ICC</span>、<span class="en">GLOBECOM</span>、
      <span class="en">WCNC</span>等国际会议<span class="en">TPC Member</span>；
      常年担任<span class="en">IEEE JSAC</span>、<span class="en">TWC</span>、
      <span class="en">TCOM</span>、<span class="en">WCM</span>、
      <span class="en">TIFS</span>、<span class="en">TCCN</span>、
      <span class="en">TVT</span>、<span class="en">TITS</span>、
      <span class="en">IOTJ</span>、<span class="en">WCL</span>、
      <span class="en">CL</span>等十余家国际期刊审稿人。
    </p>

    <p>
      作为核心成员参与国家重点研发计划项目、国家自然科学基金面上项目、
      山东省重点研发计划（重大科技示范工程）项目等多项国家级省级重点项目。
      曾获优秀博士/学士毕业论文、山东省/山东大学优秀毕业生、
      <strong>博士国家奖学金2次</strong>、<strong>本科国家奖学金</strong>、
      2026年<strong>山东大学学术之星（学院唯一）</strong>、
      2026年<strong>山东大学研究生优秀成果奖（学院唯一）</strong>、
      一等奖学金（本科4年），以及国家级省级创新创业类及学科类竞赛奖项十余项。
    </p>

  </div>

</section>


<!-- =========================================================
     学术背景
     ========================================================= -->

<section class="profile-section">

  <h2 class="profile-section-title">🎓 学术背景</h2>

  <div class="timeline">

    <div class="timeline-item">
      <div class="timeline-date">2026.07 — 至今</div>
      <div>
        <div class="timeline-main">东北大学秦皇岛分校 · 计算机与通信工程学院</div>
        <div class="timeline-sub">副教授</div>
      </div>
    </div>

    <div class="timeline-item">
      <div class="timeline-date">2024.11 — 2025.11</div>
      <div>
        <div class="timeline-main">新加坡南洋理工大学 · <span class="en">EEE</span></div>
        <div class="timeline-sub">
          联合培养博士 · 导师：
          <span class="en">Yong Liang Guan</span>（副校长）、
          <span class="en">Chau Yuen</span>（<span class="en">IEEE Fellow</span>）
        </div>
      </div>
    </div>

    <div class="timeline-item">
      <div class="timeline-date">2021.09 — 2026.06</div>
      <div>
        <div class="timeline-main">山东大学 · 信息科学与工程学院</div>
        <div class="timeline-sub">工学博士 · 导师：刘琚教授（二级）、合作导师：董郑教授</div>
      </div>
    </div>

  </div>

</section>


<!-- =========================================================
     研究方向
     ========================================================= -->

<section class="profile-section">

  <h2 class="profile-section-title">🔬 研究方向</h2>

  <div class="research-tags">

    <span class="research-tag">
      超大规模阵列通信XL-MIMO
    </span>

    <span class="research-tag">
      智能超表面IMS
    </span>

    <span class="research-tag">
      通感一体化ISAC
    </span>

    <span class="research-tag">
      近场无线通信
    </span>

    <span class="research-tag">
      波束训练
    </span>

    <span class="research-tag en">
      Deep Unfolding
    </span>

    <span class="research-tag en">
      Deep Reinforcement Learning
    </span>

  </div>

</section>


<!-- =========================================================
     学术服务
     ========================================================= -->

<section class="profile-section">

  <h2 class="profile-section-title">🌐 学术服务</h2>

  <div class="service-grid">

    <div class="service-card">
      《中国通信》（英文版）首届青年编委
    </div>

    <div class="service-card">
      <span class="en">CSIG</span>交通视频专委会委员
    </div>

    <div class="service-card">
      <span class="en">IEEE PIMRC 2026 TPC Chair</span>
    </div>

    <div class="service-card">
      <span class="en">IEEE ICC / GLOBECOM / WCNC TPC Member</span>
    </div>

    <div class="service-card" style="grid-column: 1 / -1;">
      <span class="en">
        Reviewer for IEEE JSAC, TWC, TCOM, WCM, TIFS, TCCN, TVT,
        TITS, IOTJ, WCL, CL, etc.
      </span>
    </div>

  </div>

</section>


<!-- =========================================================
     代表性成果
     ========================================================= -->

<section class="profile-section">

  <h2 class="profile-section-title">📖 代表性成果</h2>

  <div class="pub-note">
    完整论文列表请见顶部
    <a href="{{ '/publications/' | relative_url }}">
      <strong><span class="en">Publications</span></strong>
    </a>
    页面。
  </div>


  <h3 style="margin-top: 28px;">论文</h3>


  <div class="pub-item">
    <div class="pub-text en">
      <span class="pub-index">[1]</span>
      <strong>Qian Zhang</strong>, Zheng Dong, Yufei Zhao, Yao Ge,
      Yong Liang Guan, Ju Liu, and Chau Yuen,
      “Multi-resolution codebook design and multiuser interference management
      for discrete XL-RIS-aided near-field MIMO systems,”
      <strong><em>IEEE Transactions on Wireless Communications</em></strong>,
      vol. 25, pp. 2826–2842, 2026.
    </div>
    <div style="margin-top: 6px;">
      <strong>SCI, JCR Q1, IF = 10.7, 🏆 ESI高被引论文</strong>
    </div>
  </div>


  <div class="pub-item">
    <div class="pub-text en">
      <span class="pub-index">[2]</span>
      <strong>Qian Zhang</strong>, Ju Liu, Haoge Tang, Zheng Dong,
      and Yonghui Li,
      “Practical RIS-aided multiuser communications with imperfect CSI:
      Practical model, amplitude feedback, and beamforming optimization,”
      <strong><em>IEEE Transactions on Wireless Communications</em></strong>,
      vol. 23, no. 10, pp. 15245–15260, Oct. 2024.
    </div>
    <div style="margin-top: 6px;">
      <strong>SCI, JCR Q1, IF = 10.7</strong>
    </div>
  </div>


  <div class="pub-item">
    <div class="pub-text en">
      <span class="pub-index">[3]</span>
      <strong>Qian Zhang</strong>, Ju Liu, Yao Ge, Yufei Zhao,
      Wali Ullah Khan, Zheng Dong, Yong Liang Guan, Chau Yuen,
      “Two-stage coded-sliding beam training and QoS-constrained sum-rate maximization
      for SIM-assisted wireless communications,”
      <strong><em>IEEE Transactions on Wireless Communications</em></strong>,
      vol. 25, pp. 12162–12179, 2026.
    </div>
    <div style="margin-top: 6px;">
      <strong>SCI, JCR Q1, IF = 10.7</strong>
    </div>
  </div>


  <div class="pub-item">
    <div class="pub-text en">
      <span class="pub-index">[4]</span>
      <strong>Qian Zhang</strong>, Ju Lui, Zhichao Gao, Ziyu Li,
      Zhiying Peng, Zheng Dong, and Hongji Xu,
      “Robust beamforming design for RIS-aided NOMA secure networks
      with transceiver hardware impairments,”
      <strong><em>IEEE Transactions on Communications</em></strong>,
      vol. 71, no. 6, pp. 3637–3649, June 2023.
    </div>
    <div style="margin-top: 6px;">
      <strong>SCI, JCR Q1, IF = 8.3</strong>
    </div>
  </div>


  <div class="pub-item">
    <div class="pub-text en">
      <span class="pub-index">[5]</span>
      <strong>Qian Zhang</strong>, Mingjie Shao, Tong Zhang, Gaojie Chen,
      Ju Liu and Pak Chung Ching,
      “An efficient sum-rate maximization algorithm for fluid antenna-assisted ISAC system,”
      <strong><em>IEEE Communications Letters</em></strong>,
      vol. 29, no. 1, pp. 200–204, Jan. 2025.
    </div>
    <div style="margin-top: 6px;">
      <strong>
        SCI, JCR Q2, IF = 4.5, 🏆 ESI高被引论文，
        年度最受欢迎论文 TOP 2
      </strong>
    </div>
  </div>


  <h3 style="margin-top: 34px;">专利</h3>

  <div class="patent-list">

    <div class="patent-item">
      <strong>[1]</strong>
      孙福辉；张迁；王晓燕；邵明杰；刘琚；
      RIS辅助的MIMO系统的和速率优化方法及装置。
      （发明专利，授权号：<span class="en">CN117176214B</span>）
    </div>

    <div class="patent-item">
      <strong>[2]</strong>
      刘琚；程学军；张迁；罗广惠；焦钰辉；
      一种实际智能超表面辅助RSMA系统波束成形方法。
      （发明专利，公开号：<span class="en">CN120110450A</span>）
    </div>

    <div class="patent-item">
      <strong>[3]</strong>
      刘琚；程学军；罗广惠；张迁；董郑；
      一种超对角智能超表面辅助NOMA系统波束成形方法。
      （发明专利，公开号：<span class="en">CN119051703A</span>）
    </div>

    <div class="patent-item">
      <strong>[4]</strong>
      刘琚；彭志颖；王祥丞；张迁；高智超；李紫宇；
      一种多服务器MEC-D2D系统联合任务卸载与资源分配方法。
      （发明专利，授权号：<span class="en">CN116456497B</span>）
    </div>

  </div>

</section>


<!-- =========================================================
     荣誉奖励
     ========================================================= -->

<section class="profile-section">

  <h2 class="profile-section-title">🏆 荣誉奖励</h2>

  <div class="award-grid">

    <div class="award-item">推荐免试攻读研究生资格（2020）</div>

    <div class="award-item">本科国家奖学金（2020，学院排名第一）</div>

    <div class="award-item">国家励志奖学金（2018、2019）</div>

    <div class="award-item">博士国家奖学金（2024、2025）</div>

    <div class="award-item">山东省优秀毕业生（2021）</div>

    <div class="award-item">山东大学优秀毕业生（2026）</div>

    <div class="award-item">山东大学学术之星（2026，学院唯一）</div>

    <div class="award-item">山东大学研究生优秀成果奖（2026，学院唯一）</div>

    <div class="award-item">博士中期考核优秀奖（排名第一）</div>

    <div class="award-item">本科一等学业奖学金（四年专业唯一）</div>

    <div class="award-item">
      博士优秀生源奖学金、新生一等奖学金
    </div>

  </div>

</section>


<!-- =========================================================
     招生与合作
     ========================================================= -->

<section class="profile-section">

  <h2 class="profile-section-title">🤝 招生与合作</h2>

  <div class="coop-box profile-text">

    <p>
      长期与新加坡南洋理工大学、山东大学、电子科技大学、
      西北工业大学、南京理工大学等国内外知名高校保持科研合作。
    </p>

    <p>
      欢迎对无线通信、智能超表面、通感一体化、
      人工智能通信优化等方向感兴趣的本科生、硕士生及博士生联系交流。
    </p>

    <p>
      个人邮箱：
      <span class="en">zhangqian@neuq.edu.cn</span>；
      <span class="en">zq869054246@163.com</span>。
    </p>

  </div>

</section>


<!-- =========================================================
     访问量
     ========================================================= -->

<div class="visit-counter">

  👁️ 本站总访问量：
  <span id="busuanzi_site_pv">加载中...</span> 次

  &nbsp;&nbsp;|&nbsp;&nbsp;

  👤 本站总访客数：
  <span id="busuanzi_site_uv">加载中...</span> 人

</div>


<script
  src="https://cdn.busuanzi.cc/busuanzi/3.6.9/busuanzi.min.js"
  defer>
</script>


</div>
