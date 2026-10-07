---
page_id: about
layout: about
title: "Home"
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
/* ==================== Page Basics ==================== */
html,
body {
  overflow-x: hidden;
}

.profile-page {
  --profile-accent: var(--global-theme-color, #b509ac);
  --profile-surface: var(--global-card-bg-color, #ffffff);
  --profile-divider: var(--global-divider-color, #e6e6e6);
  --profile-muted: var(--global-text-color-light, #888888);
  --profile-hover-tint: rgba(181, 9, 172, 0.045);
  --profile-hover-shadow:
    0 14px 30px rgba(0, 0, 0, 0.085),
    0 5px 14px rgba(181, 9, 172, 0.12);

  max-width: 1120px;
  margin: 0 auto;
  line-height: 1.8;
}

/* Follow the existing dark theme. */
html[data-theme="dark"] .profile-page {
  --profile-hover-tint: rgba(181, 9, 172, 0.10);
  --profile-hover-shadow:
    0 14px 30px rgba(0, 0, 0, 0.30),
    0 5px 18px rgba(181, 9, 172, 0.20);
}

.profile-page,
.profile-page * {
  box-sizing: border-box;
}

/* Use Times New Roman throughout the English page. */
.profile-page,
.profile-page * {
  font-family: "Times New Roman", Times, serif !important;
}

/* ==================== Profile Header ==================== */
.profile-top {
  display: grid;
  grid-template-columns: 190px 1fr 190px;
  gap: 34px;
  align-items: center;
  margin-top: 8px;
  margin-bottom: 26px;
  padding: 24px 0 18px;
}

.profile-photo-wrap,
.profile-logo-wrap {
  text-align: center;
}

.profile-photo {
  width: 190px;
  max-width: 100%;
  height: auto;
  display: block;
  margin: 0 auto;
  border-radius: 8px;
  box-shadow: 0 6px 18px rgba(0, 0, 0, 0.08);
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
  flex: 0 0 100px;
  min-width: 100px;
  font-weight: 600;
}

.profile-info-row > span:last-child {
  flex: 1;
  min-width: 0;
  overflow-wrap: anywhere;
}

.profile-logo {
  width: 175px;
  max-width: 100%;
  height: auto;
  display: block;
  margin: 0 auto;
}

/* ==================== Name and Welcome ==================== */
.profile-name {
  margin: 4px 0;
  font-size: 2.05rem;
  font-weight: 700;
}

.profile-welcome {
  margin: 0 0 26px;
  font-size: 1rem;
  color: var(--profile-muted);
}

/* ==================== Sections and Body Text ==================== */
.profile-section {
  margin: 44px 0;
}

.profile-section-title {
  font-size: 1.62rem;
  font-weight: 700;
  margin-bottom: 22px;
  padding-bottom: 10px;
  border-bottom: 2px solid var(--profile-divider);
}

.profile-section-title::before {
  content: "";
  display: inline-block;
  width: 5px;
  height: 1.12em;
  margin-right: 11px;
  border-radius: 4px;
  background: var(--profile-accent);
  vertical-align: -0.12em;
}

.profile-text p {
  text-align: justify;
  text-align-last: left;
  text-justify: inter-word;
  hyphens: auto;
  line-height: 1.85;
  margin-top: 0;
  margin-bottom: 1.25em;
}

/* ==================== Biography Card ==================== */
.profile-intro-card {
  background: var(--profile-surface);
  border: 1px solid var(--profile-divider);
  border-radius: 14px;
  padding: 28px 30px;
  box-shadow: 0 5px 18px rgba(0, 0, 0, 0.045);
}

/* ==================== Academic Background ==================== */
.timeline {
  display: flex;
  flex-direction: column;
  gap: 18px;
}

.timeline-item {
  display: grid;
  grid-template-columns: 185px 1fr;
  gap: 24px;
  padding: 18px 20px;
  border: 1px solid var(--profile-divider);
  border-radius: 12px;
  background: var(--profile-surface);
}

.timeline-item > div {
  min-width: 0;
}

.timeline-date {
  font-family: "Times New Roman", Times, serif;
  font-weight: 700;
  color: var(--profile-accent);
}

.timeline-main {
  font-weight: 600;
  transition: color 0.22s ease;
}

.timeline-sub {
  margin-top: 3px;
  font-size: 0.94rem;
  color: var(--profile-muted);
}

/* ==================== Research Interest Tags ==================== */
.research-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
}

.research-tag {
  display: inline-block;
  padding: 7px 14px;
  border: 1px solid var(--profile-accent);
  border-radius: 999px;
  color: var(--profile-accent);
  font-size: 0.94rem;
  font-weight: 600;
  background: var(--profile-surface);
}

/* ==================== Academic Service ==================== */
.service-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 16px;
}

.service-card {
  padding: 18px 20px;
  border: 1px solid var(--profile-divider);
  border-radius: 12px;
  background: var(--profile-surface);
}

/* ==================== Publications ==================== */
.pub-note {
  margin-bottom: 20px;
  padding: 14px 18px;
  border-left: 4px solid var(--profile-accent);
  border-radius: 0 10px 10px 0;
  background: var(--profile-surface);
}

.pub-item {
  margin-bottom: 20px;
  padding: 18px 20px;
  border: 1px solid var(--profile-divider);
  border-radius: 12px;
  background: var(--profile-surface);
}

.pub-index {
  font-family: "Times New Roman", Times, serif;
  font-weight: 700;
  color: var(--profile-accent);
}

.pub-text {
  line-height: 1.75;
}

/* ==================== Patents ==================== */
.patent-list {
  display: flex;
  flex-direction: column;
  gap: 14px;
}

.patent-item {
  padding: 16px 18px;
  border: 1px solid var(--profile-divider);
  border-radius: 11px;
  background: var(--profile-surface);
}

/* ==================== Honors and Awards ==================== */
.award-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 14px 18px;
}

.award-item {
  padding: 15px 17px;
  border: 1px solid var(--profile-divider);
  border-radius: 11px;
  background: var(--profile-surface);
}

/* ==================== Prospective Students and Collaboration ==================== */
.coop-box {
  padding: 24px 28px;
  border-left: 4px solid var(--profile-accent);
  border-radius: 0 12px 12px 0;
  background: var(--profile-surface);
}

/* ==================== Visitor Counter ==================== */
.visit-counter {
  text-align: center;
  margin-top: 48px;
  padding-top: 22px;
  border-top: 1px solid var(--profile-divider);
  font-size: 0.9rem;
  color: var(--profile-muted);
}

/* =========================================================
   Individual Card Hover Effects
   Apply profile-hover-card to each card, not to its container.
   ========================================================= */
.profile-page .profile-hover-card {
  position: relative;
  z-index: 0;
  transition:
    transform 0.22s ease,
    border-color 0.22s ease,
    box-shadow 0.22s ease;
}

.profile-page .research-tag {
  position: relative;
  z-index: 0;
  transition:
    transform 0.22s ease,
    color 0.22s ease,
    background-color 0.22s ease,
    border-color 0.22s ease,
    box-shadow 0.22s ease;
}

/* Extend the hover area below lifted cards to prevent edge flicker. */
.profile-page .profile-hover-card::after,
.profile-page .research-tag::after {
  content: "";
  position: absolute;
  left: 0;
  right: 0;
  bottom: -6px;
  height: 6px;
  background: transparent;
  pointer-events: none;
}

/* Highlight cards when their links receive keyboard focus. */
.profile-page .profile-hover-card:focus-within {
  z-index: 1;
  border-color: var(--profile-accent);
  background-image: linear-gradient(
    var(--profile-hover-tint),
    var(--profile-hover-tint)
  );
  box-shadow: var(--profile-hover-shadow);
}

.profile-page a:focus-visible {
  outline: 2px solid var(--profile-accent);
  outline-offset: 3px;
  border-radius: 3px;
}

/* Enable hover effects on devices with a hover-capable pointer. */
@media (any-hover: hover) {
  .profile-page .profile-hover-card:hover {
    z-index: 1;
    transform: translateY(-4px);
    border-color: var(--profile-accent);
    background-image: linear-gradient(
      var(--profile-hover-tint),
      var(--profile-hover-tint)
    );
    box-shadow: var(--profile-hover-shadow);
  }

  .profile-page .timeline-item:hover .timeline-main {
    color: var(--profile-accent);
  }

  /* Only the hovered tag changes to a purple background with white text. */
  .profile-page .research-tag:hover {
    z-index: 1;
    transform: translateY(-3px);
    color: #ffffff;
    border-color: var(--profile-accent);
    background-color: var(--profile-accent);
    box-shadow: 0 7px 18px rgba(181, 9, 172, 0.24);
  }

  .profile-page .research-tag:hover * {
    color: inherit;
  }

  .profile-page .profile-hover-card:hover::after,
  .profile-page .research-tag:hover::after {
    pointer-events: auto;
  }
}

/* ==================== Responsive Layout ==================== */
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
    box-sizing: border-box;
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

  .profile-page .profile-info,
  .profile-page .profile-hover-card,
  .profile-page .research-tag {
    overflow-wrap: anywhere;
  }
}

/* Respect reduced-motion preferences while keeping color and shadow effects. */
@media (prefers-reduced-motion: reduce) {
  .profile-page .profile-hover-card,
  .profile-page .research-tag,
  .profile-page .timeline-main {
    transition: none !important;
  }

  .profile-page .profile-hover-card:hover,
  .profile-page .research-tag:hover {
    transform: none !important;
  }
}
</style>

<div class="profile-page" lang="en">

<!-- Profile Header -->

<div class="profile-top">

  <div class="profile-photo-wrap">
    <img
      src="{{ '/assets/img/Qian_Zhang_GitHub_2.png' | relative_url }}"
      class="profile-photo"
      alt="Qian Zhang">
  </div>

  <div class="profile-info">

    <div class="profile-info-row">
      <span class="profile-info-label">University:</span>
      <span>Northeastern University at Qinhuangdao</span>
    </div>

    <div class="profile-info-row">
      <span class="profile-info-label">School:</span>
      <span>School of Computer and Communication Engineering</span>
    </div>

    <div class="profile-info-row">
      <span class="profile-info-label">Position:</span>
      <span>Associate Professor</span>
    </div>

    <div class="profile-info-row">
      <span class="profile-info-label">Degree:</span>
      <span>Ph.D. in Engineering</span>
    </div>

    <div class="profile-info-row">
      <span class="profile-info-label">Alma Mater:</span>
      <span>Shandong University</span>
    </div>

    <div class="profile-info-row">
      <span class="profile-info-label">Email:</span>
      <span>zq869054246@163.com</span>
    </div>

  </div>

  <div class="profile-logo-wrap">
    <img
      src="{{ '/assets/img/Northeastern_University.png' | relative_url }}"
      class="profile-logo"
      alt="Northeastern University Logo">
  </div>

</div>

<!-- Name and Welcome -->

<h1 class="profile-name">Qian Zhang</h1>

<p class="profile-welcome">
  Welcome to my personal homepage!
  (<a href="https://scholar.google.com/citations?user=hs8KAR4AAAAJ&amp;hl=en">Google Scholar</a>)
</p>

<!-- Biography -->

<section class="profile-section">

  <h2 class="profile-section-title">👨‍🏫 Biography</h2>

  <div class="profile-intro-card profile-text profile-hover-card">

    <p>
      <strong>Qian Zhang</strong>, <strong>Ph.D. in Engineering</strong>, is an
      <strong>Associate Professor</strong> and a
      <strong>supervisor of master's students</strong>.
      He is a Member of IEEE, a member of the China Institute of Communications,
      and a member of the CSIG Technical Committee on Traffic Video.
      He received his Ph.D. in Engineering from Shandong University in June 2026
      through a direct-entry doctoral program, supervised by
      Prof. Ju Liu (Tier-2 Professor) and co-supervised by Prof. Zheng Dong.
      In 2024, he received funding from the
      <strong>China Scholarship Council (CSC)</strong> for joint Ph.D. training
      at the School of Electrical and Electronic Engineering (EEE),
      Nanyang Technological University, Singapore, under the supervision of
      Prof. Yong Liang Guan (Vice President) and
      Prof. Chau Yuen (IEEE Fellow).
    </p>

    <p>
      His research focuses on intelligent metasurfaces, convex optimization theory,
      and artificial intelligence algorithms for wireless communications and sensing.
      He has published more than 30 research papers in leading journals such as
      IEEE TWC and IEEE TCOM, and major conferences such as IEEE ICC and IEEE ICASSP,
      including <strong>18 papers as first author, co-first author,
      or corresponding author</strong>.
      Two of his first-authored papers have been recognized as
      <strong>🏆 ESI Highly Cited Papers</strong>.
      One first-authored paper was ranked among the
      <strong>Top 2 Most Popular Papers of the Year in IEEE CL</strong>,
      and four papers were listed among the
      <strong>Top 50 Monthly Most Popular Papers in IEEE TVT, IEEE WCL,
      and IEEE CL</strong>
      (one first-authored, two co-first-authored, and one second-authored paper).
      He holds three granted patents.
    </p>

    <p>
      He serves on the inaugural Young Editorial Board of
      <em>China Communications</em> (English edition) and as
      TPC Chair for IEEE PIMRC 2026.
      He has served as a Technical Program Committee (TPC) Member for
      international conferences including IEEE ICC, IEEE GLOBECOM,
      and IEEE WCNC.
      He also regularly reviews for more than ten international journals,
      including IEEE JSAC, IEEE TWC, IEEE TCOM, IEEE WCM, IEEE TIFS,
      IEEE TCCN, IEEE TVT, IEEE TITS, IEEE IoTJ, IEEE WCL, and IEEE CL.
    </p>

    <p>
      As a core team member, he has participated in several major national
      and provincial research projects, including projects supported by the
      National Key R&amp;D Program of China, the General Program of the
      National Natural Science Foundation of China, and the
      Shandong Provincial Key R&amp;D Program
      (Major Science and Technology Demonstration Projects).
      His honors include Outstanding Doctoral Dissertation and Bachelor's Thesis
      Awards, Outstanding Graduate awards from Shandong Province and
      Shandong University,
      <strong>two National Scholarships for Doctoral Students</strong>,
      a <strong>National Scholarship for Undergraduate Students</strong>,
      the <strong>2026 Shandong University Academic Star Award
      (the sole recipient in his school)</strong>,
      the <strong>2026 Shandong University Outstanding Graduate Research
      Achievement Award (the sole recipient in his school)</strong>,
      and first-class scholarships in all four undergraduate years.
      He has also received more than ten national and provincial awards
      in innovation, entrepreneurship, and academic competitions.
    </p>

  </div>

</section>

<!-- Academic Background -->

<section class="profile-section">

  <h2 class="profile-section-title">🎓 Academic Background</h2>

  <div class="timeline">

    <div class="timeline-item profile-hover-card">
      <div class="timeline-date">Jul. 2026 — Present</div>
      <div>
        <div class="timeline-main">
          Northeastern University at Qinhuangdao ·
          School of Computer and Communication Engineering
        </div>
        <div class="timeline-sub">Associate Professor</div>
      </div>
    </div>

    <div class="timeline-item profile-hover-card">
      <div class="timeline-date">Nov. 2024 — Nov. 2025</div>
      <div>
        <div class="timeline-main">
          Nanyang Technological University, Singapore ·
          School of Electrical and Electronic Engineering (EEE)
        </div>
        <div class="timeline-sub">
          Visiting Ph.D. Student (Joint Training) · Supervisors:
          Prof. Yong Liang Guan (Vice President) and
          Prof. Chau Yuen (IEEE Fellow)
        </div>
      </div>
    </div>

    <div class="timeline-item profile-hover-card">
      <div class="timeline-date">Sep. 2021 — Jun. 2026</div>
      <div>
        <div class="timeline-main">
          Shandong University · School of Information Science and Engineering
        </div>
        <div class="timeline-sub">
          Ph.D. in Engineering · Supervisor: Prof. Ju Liu (Tier-2 Professor);
          Co-supervisor: Prof. Zheng Dong
        </div>
      </div>
    </div>

  </div>

</section>

<!-- Research Interests -->

<section class="profile-section">

  <h2 class="profile-section-title">🔬 Research Interests</h2>

  <div class="research-tags">

    <span class="research-tag">
      Extremely Large-Scale MIMO (XL-MIMO)
    </span>

    <span class="research-tag">
      Intelligent Metasurfaces (IMS)
    </span>

    <span class="research-tag">
      Integrated Sensing and Communications (ISAC)
    </span>

    <span class="research-tag">
      Near-Field Wireless Communications
    </span>

    <span class="research-tag">
      Beam Training
    </span>

    <span class="research-tag">
      Deep Unfolding
    </span>

    <span class="research-tag">
      Deep Reinforcement Learning
    </span>

  </div>

</section>

<!-- Academic Service -->

<section class="profile-section">

  <h2 class="profile-section-title">🌐 Academic Service</h2>

  <div class="service-grid">

    <div class="service-card profile-hover-card">
      Member of the Inaugural Young Editorial Board,
      <em>China Communications</em> (English Edition)
    </div>

    <div class="service-card profile-hover-card">
      Member, CSIG Technical Committee on Traffic Video
    </div>

    <div class="service-card profile-hover-card">
      IEEE PIMRC 2026 TPC Chair
    </div>

    <div class="service-card profile-hover-card">
      IEEE ICC / GLOBECOM / WCNC TPC Member
    </div>

    <div class="service-card profile-hover-card" style="grid-column: 1 / -1;">
      Reviewer for IEEE JSAC, TWC, TCOM, WCM, TIFS, TCCN, TVT,
      TITS, IoTJ, WCL, CL, etc.
    </div>

  </div>

</section>

<!-- Selected Publications and Patents -->

<section class="profile-section">

  <h2 class="profile-section-title">📖 Selected Publications and Patents</h2>

  <div class="pub-note profile-hover-card">
    For the complete publication list, please visit the
    <a href="{{ '/publications/' | relative_url }}">
      <strong>Publications</strong>
    </a>
    page in the navigation menu.
  </div>

  <h3 style="margin-top: 28px;">Publications</h3>

  <div class="pub-item profile-hover-card">
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
      <strong>SCI, JCR Q1, IF = 10.7, 🏆 ESI Highly Cited Paper</strong>
    </div>
  </div>

  <div class="pub-item profile-hover-card">
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

  <div class="pub-item profile-hover-card">
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

  <div class="pub-item profile-hover-card">
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

  <div class="pub-item profile-hover-card">
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
        SCI, JCR Q2, IF = 4.5, 🏆 ESI Highly Cited Paper,
        Top 2 Most Popular Papers of the Year
      </strong>
    </div>
  </div>

  <h3 style="margin-top: 34px;">Patents</h3>

  <div class="patent-list">

    <div class="patent-item profile-hover-card">
      <strong>[1]</strong>
      Fuhui Sun; Qian Zhang; Xiaoyan Wang; Mingjie Shao; Ju Liu.
      A sum-rate optimization method and apparatus for RIS-assisted MIMO systems.
      (Invention Patent, Grant No.: CN117176214B)
    </div>

    <div class="patent-item profile-hover-card">
      <strong>[2]</strong>
      Ju Liu; Xuejun Cheng; Qian Zhang; Guanghui Luo; Yuhui Jiao.
      A beamforming method for practical intelligent metasurface-assisted RSMA systems.
      (Invention Patent, Publication No.: CN120110450A)
    </div>

    <div class="patent-item profile-hover-card">
      <strong>[3]</strong>
      Ju Liu; Xuejun Cheng; Guanghui Luo; Qian Zhang; Zheng Dong.
      A beamforming method for beyond-diagonal intelligent metasurface-assisted NOMA systems.
      (Invention Patent, Publication No.: CN119051703A)
    </div>

    <div class="patent-item profile-hover-card">
      <strong>[4]</strong>
      Ju Liu; Zhiying Peng; Xiangcheng Wang; Qian Zhang; Zhichao Gao; Ziyu Li.
      A joint task offloading and resource allocation method for multi-server MEC-D2D systems.
      (Invention Patent, Grant No.: CN116456497B)
    </div>

  </div>

</section>

<!-- Honors and Awards -->

<section class="profile-section">

  <h2 class="profile-section-title">🏆 Honors and Awards</h2>

  <div class="award-grid">

    <div class="award-item profile-hover-card">
      Recommended for Postgraduate Admission without Entrance Examination (2020)
    </div>

    <div class="award-item profile-hover-card">
      National Scholarship for Undergraduate Students
      (2020, Ranked 1st in the School)
    </div>

    <div class="award-item profile-hover-card">
      National Encouragement Scholarship (2018, 2019)
    </div>

    <div class="award-item profile-hover-card">
      National Scholarship for Doctoral Students (2024, 2025)
    </div>

    <div class="award-item profile-hover-card">
      Outstanding Graduate of Shandong Province (2021)
    </div>

    <div class="award-item profile-hover-card">
      Outstanding Graduate of Shandong University (2026)
    </div>

    <div class="award-item profile-hover-card">
      Shandong University Academic Star Award
      (2026, Sole Recipient in the School)
    </div>

    <div class="award-item profile-hover-card">
      Shandong University Outstanding Graduate Research Achievement Award
      (2026, Sole Recipient in the School)
    </div>

    <div class="award-item profile-hover-card">
      Outstanding Performance Award in the Ph.D. Midterm Assessment (Ranked 1st)
    </div>

    <div class="award-item profile-hover-card">
      First-Class Undergraduate Academic Scholarship
      (The Only Student in the Major to Receive It in All Four Years)
    </div>

    <div class="award-item profile-hover-card">
      Outstanding Incoming Ph.D. Student Scholarship;
      First-Class Scholarship for New Students
    </div>

  </div>

</section>

<!-- Prospective Students and Collaboration -->

<section class="profile-section">

  <h2 class="profile-section-title">🤝 Prospective Students and Collaboration</h2>

  <div class="coop-box profile-text profile-hover-card">

    <p>
      I maintain long-term research collaborations with leading universities
      in China and abroad, including Nanyang Technological University,
      Shandong University, the University of Electronic Science and Technology of China,
      Northwestern Polytechnical University, and
      Nanjing University of Science and Technology.
    </p>

    <p>
      Undergraduate, master's, and doctoral students interested in
      wireless communications, intelligent metasurfaces,
      integrated sensing and communications, or
      AI-driven optimization for communications are welcome to contact me
      to discuss research interests and opportunities.
    </p>

    <p>
      Email:
      <span>zhangqian@neuq.edu.cn</span>;
      <span>zq869054246@163.com</span>.
    </p>

  </div>

</section>

<!-- Visitor Counter -->

<div class="visit-counter">

  👁️ Total Page Views:
  <span id="busuanzi_site_pv">Loading...</span>

  &nbsp;&nbsp;|&nbsp;&nbsp;

  👤 Total Visitors:
  <span id="busuanzi_site_uv">Loading...</span>

</div>

<script
  src="https://cdn.busuanzi.cc/busuanzi/3.6.9/busuanzi.min.js"
  defer>
</script>

</div>
