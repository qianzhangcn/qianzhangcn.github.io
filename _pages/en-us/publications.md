---
page_id: Publications
layout: page
title: "Publications"
permalink: /Publications/
description: Main research achievements in wireless communications and sensing
nav: true
nav_order: 2
---

<style>

/* =========================================================
   Publications Page
   ========================================================= */

.publications-page {
  max-width: 1120px;
  margin: 0 auto;
  line-height: 1.75;
}

/* Entire page uses Times New Roman */
.publications-page,
.publications-page * {
  font-family: "Times New Roman", Times, serif !important;
}


/* =========================================================
   Header
   ========================================================= */

.publications-header {
  display: grid;
  grid-template-columns: 1fr 170px;
  align-items: center;
  gap: 35px;

  margin-top: 5px;
  margin-bottom: 34px;

  padding-bottom: 25px;
  border-bottom: 1px solid var(--global-divider-color);
}

.publications-title {
  min-width: 0;
}

.publications-title-main {
  margin: 0 0 8px;

  font-size: 2rem;
  font-weight: 700;
}

.publications-subtitle {
  font-size: 0.98rem;
  color: var(--global-text-color-light);
  line-height: 1.7;
}

.publications-note {
  display: inline-block;

  margin-top: 12px;
  padding: 6px 13px;

  border-radius: 20px;
  border: 1px solid var(--global-divider-color);

  font-size: 0.89rem;
  color: var(--global-text-color-light);

  background: var(--global-card-bg-color);
}

.publications-logo {
  display: flex;
  justify-content: center;
  align-items: center;
}

.publications-logo img {
  width: 160px;
  max-width: 100%;
  height: auto;
  display: block;
}


/* =========================================================
   Section
   ========================================================= */

.pub-section {
  margin: 45px 0 55px;
}

.pub-section-header {
  display: flex;
  align-items: center;
  gap: 12px;

  margin-bottom: 25px;
  padding-bottom: 11px;

  border-bottom: 2px solid var(--global-divider-color);
}

.pub-section-bar {
  width: 5px;
  height: 30px;

  flex: 0 0 auto;

  border-radius: 5px;
  background: var(--global-theme-color);
}

.pub-section-title {
  margin: 0;

  font-size: 1.58rem;
  font-weight: 700;
}

.pub-section-description {
  margin-left: auto;

  font-size: 0.93rem;
  color: var(--global-text-color-light);
}


/* =========================================================
   Publication List
   ========================================================= */

.pub-list {
  list-style: none;

  counter-reset: pub-counter;

  margin: 0;
  padding: 0;

  display: flex;
  flex-direction: column;
  gap: 16px;
}

.pub-list > li {
  counter-increment: pub-counter;

  position: relative;

  margin: 0;
  padding: 19px 22px 19px 66px;

  border: 1px solid var(--global-divider-color);
  border-radius: 13px;

  background: var(--global-card-bg-color);

  font-size: 16.5px;
  font-weight: 400;

  line-height: 1.72;

  text-align: justify;

  transition:
    transform 0.22s ease,
    box-shadow 0.22s ease,
    border-color 0.22s ease;
}

.pub-list > li:hover {
  transform: translateY(-2px);

  box-shadow: 0 7px 20px rgba(0, 0, 0, 0.06);

  border-color: var(--global-theme-color);
}


/* =========================================================
   Automatic Numbering
   ========================================================= */

.pub-list > li::before {
  content: "[" counter(pub-counter) "]";

  position: absolute;

  left: 17px;
  top: 19px;

  width: 34px;

  text-align: center;

  font-size: 16px;
  font-weight: 700;

  color: var(--global-theme-color);
}


/* =========================================================
   Author / Journal / Conference
   ========================================================= */

.pub-list .author-name {
  font-weight: 700 !important;
  font-style: normal !important;
}

.pub-list .journal-name {
  font-weight: 700 !important;
  font-style: italic !important;
}

.pub-list .etal {
  font-style: italic !important;
  font-weight: 400 !important;
}

.pub-list .conference-name {
  font-weight: 700 !important;
  font-style: normal !important;
}


/* =========================================================
   Paper Information
   ========================================================= */

.pub-list .paper-info {
  display: inline-block;

  margin-top: 7px;
  margin-right: 6px;

  padding: 3px 9px;

  border-radius: 6px;

  background: rgba(128, 128, 128, 0.09);

  font-size: 0.88rem;
  font-weight: 700 !important;
  font-style: normal !important;

  color: var(--global-text-color);
}


/* =========================================================
   Full Paper Link
   ========================================================= */

.pub-list a {
  display: inline-block;

  margin-top: 7px;
  margin-left: 2px;

  padding: 3px 10px;

  border: 1px solid var(--global-theme-color);
  border-radius: 6px;

  color: var(--global-theme-color) !important;

  font-size: 0.88rem;
  font-weight: 700;

  text-decoration: none !important;

  transition:
    background 0.18s ease,
    color 0.18s ease;
}

.pub-list a:hover {
  background: var(--global-theme-color);
  color: white !important;
}


/* =========================================================
   Footer Note
   ========================================================= */

.publications-footer-note {
  margin-top: 42px;

  padding: 18px 22px;

  border-left: 4px solid var(--global-theme-color);
  border-radius: 0 10px 10px 0;

  background: var(--global-card-bg-color);

  font-size: 0.93rem;
  color: var(--global-text-color-light);
}


/* =========================================================
   Mobile
   ========================================================= */

@media screen and (max-width: 768px) {

  .publications-header {
    grid-template-columns: 1fr;
    gap: 18px;
    text-align: left;
  }

  .publications-logo {
    display: none;
  }

  .publications-title-main {
    font-size: 1.8rem;
  }

  .pub-section-header {
    align-items: flex-start;
  }

  .pub-section-description {
    display: none;
  }

  .pub-list > li {
    padding: 18px 16px 18px 50px;

    font-size: 15.5px;
    line-height: 1.68;

    text-align: left;
  }

  .pub-list > li::before {
    left: 10px;
    top: 18px;

    width: 32px;
  }

}


/* =========================================================
   Very Small Screens
   ========================================================= */

@media screen and (max-width: 480px) {

  .pub-list > li {
    padding-left: 16px;
    padding-top: 48px;
  }

  .pub-list > li::before {
    left: 16px;
    top: 15px;

    text-align: left;
  }

}

</style>


<div class="publications-page">


<!-- =========================================================
     Header
     ========================================================= -->

<div class="publications-header">

  <div class="publications-title">

    <h1 class="publications-title-main">
      Publications
    </h1>

    <div class="publications-subtitle">
      Main research achievements in wireless communications, intelligent metasurfaces,
      integrated sensing and communication, near-field communications, movable antennas,
      and AI-enabled wireless networks.
    </div>

    <div class="publications-note">
      † Co-first author &nbsp;&nbsp; | &nbsp;&nbsp; * Corresponding author
    </div>

  </div>


  <div class="publications-logo">

    <img
      src="{{ '/assets/img/ICS_LOGO.png' | relative_url }}"
      alt="ICS Lab Logo">

  </div>

</div>


<!-- =========================================================
     Journal Papers
     ========================================================= -->

<section class="pub-section">

  <div class="pub-section-header">

    <div class="pub-section-bar"></div>

    <h2 class="pub-section-title">
      Journal Papers
    </h2>

    <div class="pub-section-description">
      Peer-Reviewed Journal Articles
    </div>

  </div>


<ol class="pub-list">


<li>
<span class="author-name">Qian Zhang</span>,
<span class="etal">et al.</span>,
"Hierarchical sub-array beam training for flexible intelligent metasurface-enabled hybrid near-far-field multiuser communications,"
<span class="journal-name">IEEE Journal on Selected Areas in Communications</span>,
2026.
<span class="paper-info">(JCR Q1, IF = 16.8, Major Revision)</span>
</li>


<li>
<span class="author-name">Qian Zhang</span>,
<span class="etal">et al.</span>,
"RIS-aided covert communications with discrete phase control, element control failures, and element activation states,"
<span class="journal-name">IEEE Transactions on Wireless Communications</span>,
2026.
<span class="paper-info">(JCR Q1, IF = 10.3, Under Review)</span>
</li>


<li>
Yufei Zhao*,
Deyu Lin,
<span class="author-name">Qian Zhang*</span>,
<span class="etal">et al.</span>,
"Enhanced information security via wave-field selectivity and structured wavefront manipulation,"
<span class="journal-name">IEEE Transactions on Wireless Communications</span>,
2026.
<span class="paper-info">(JCR Q1, IF = 10.7)</span>
<a href="https://ieeexplore.ieee.org/document/11720371">Full Paper</a>
</li>


<li>
<span class="author-name">Qian Zhang</span>,
<span class="etal">et al.</span>,
"RIS-assisted multiuser NOMA networks with imperfect CSI under transceiver hardware impairments,"
<span class="journal-name">IEEE Internet of Things Journal</span>,
2026.
<span class="paper-info">(JCR Q1, IF = 8.33)</span>
<a href="https://ieeexplore.ieee.org/document/11720371">Full Paper</a>
</li>


<li>
<span class="author-name">Qian Zhang</span>,
Zheng Dong,
<span class="etal">et al.</span>,
"Multi-resolution codebook design and multiuser interference management for discrete XL-RIS-aided near-field MIMO systems,"
<span class="journal-name">IEEE Transactions on Wireless Communications</span>,
vol. 25, pp. 2826-2842, 2026.
<span class="paper-info">(JCR Q1, IF = 10.7, 🏆 ESI Highly Cited Paper)</span>
<a href="https://doi.org/10.1109/TWC.2025.3599514">Full Paper</a>
</li>


<li>
<span class="author-name">Qian Zhang</span>,
Ju Liu,
<span class="etal">et al.</span>,
"Practical RIS-aided multiuser communications with imperfect CSI: Practical model, amplitude feedback, and beamforming optimization,"
<span class="journal-name">IEEE Transactions on Wireless Communications</span>,
vol. 23, no. 10, pp. 15245-15260, Oct. 2024.
<span class="paper-info">(JCR Q1, IF = 10.7)</span>
<a href="https://doi.org/10.1109/TWC.2024.3427695">Full Paper</a>
</li>


<li>
<span class="author-name">Qian Zhang</span>,
Ju Liu,
<span class="etal">et al.</span>,
"Two-Stage Coded-Sliding Beam Training and QoS-constrained sum-rate maximization for SIM-assisted wireless communications,"
<span class="journal-name">IEEE Transactions on Wireless Communications</span>,
vol. 25, pp. 12162-12179, 2026.
<span class="paper-info">(JCR Q1, IF = 10.7)</span>
<a href="https://doi.org/10.1109/TWC.2026.3661858">Full Paper</a>
</li>


<li>
<span class="author-name">Qian Zhang</span>,
Ju Liu,
<span class="etal">et al.</span>,
"Robust beamforming design for RIS-aided NOMA secure networks with transceiver hardware impairments,"
<span class="journal-name">IEEE Transactions on Communications</span>,
vol. 71, no. 6, pp. 3637-3649, Jun. 2023.
<span class="paper-info">(JCR Q1, IF = 8.3)</span>
<a href="https://doi.org/10.1109/TCOMM.2023.3251345">Full Paper</a>
</li>


<li>
<span class="author-name">Qian Zhang</span>,
Zhengfeng Du,
<span class="etal">et al.</span>,
"Joint power allocation and discrete phase-shift optimization for SIM-aided ISAC systems,"
<span class="journal-name">IEEE Transactions on Vehicular Technology</span>,
vol. 74, no. 12, pp. 19795-19800, Dec. 2025.
<span class="paper-info">(JCR Q1, IF = 7.1)</span>
<a href="https://doi.org/10.1109/TVT.2025.3584064">Full Paper</a>
</li>


<li>
<span class="author-name">Qian Zhang</span>,
Yufei Zhao,
<span class="etal">et al.</span>,
"Crem'er-Rao bound minimization for flexible intelligent metasurfaces enabled ISAC systems,"
<span class="journal-name">IEEE Transactions on Vehicular Technology</span>,
2025.
<span class="paper-info">(JCR Q1, IF = 7.1)</span>
<a href="https://doi.org/10.1109/TVT.2026.3701078">Full Paper</a>
</li>


<li>
<span class="author-name">Qian Zhang</span>,
Mingjie Shao,
<span class="etal">et al.</span>,
"An efficient sum-rate maximization algorithm for fluid antenna-assisted ISAC system,"
<span class="journal-name">IEEE Communications Letters</span>,
vol. 29, no. 1, pp. 200-204, Jan. 2025.
<span class="paper-info">(JCR Q2, IF = 4.4, 🏆 ESI Highly Cited Paper, Top 2 Most Popular Papers of the Year)</span>
<a href="https://doi.org/10.1109/LCOMM.2024.3510334">Full Paper</a>
</li>


<li>
<span class="author-name">Qian Zhang</span>†,
Guanghui Luo†,
<span class="etal">et al.</span>,
"Beyond-diagonal reconfigurable intelligent surface enhanced NOMA systems,"
<span class="journal-name">IEEE Wireless Communications Letters</span>,
vol. 14, no. 1, pp. 118-122, Jan. 2025.
<span class="paper-info">(JCR Q1, IF = 5.5)</span>
<a href="https://doi.org/10.1109/LWC.2024.3489718">Full Paper</a>
</li>


<li>
Xuejun Cheng†,
<span class="author-name">Qian Zhang</span>†,
Yunnuo Xu,
<span class="etal">et al.</span>,
"Robust beamforming for non-ideal RIS enabled rate-splitting multiple access systems,"
<span class="journal-name">IEEE Transactions on Vehicular Technology</span>,
2025.
<span class="paper-info">(Co-first Author, Primary Supervisor, JCR Q1, IF = 7.1)</span>
<a href="https://doi.org/10.1109/TVT.2026.3677351">Full Paper</a>
</li>


<li>
Maoyuan Wang†,
<span class="author-name">Qian Zhang</span>†,
<span class="etal">et al.</span>,
"DRL-Based Antenna Position Optimization for MA-Assisted OTFS System Under Imperfect CSI,"
<span class="journal-name">IEEE Communications Letters</span>,
vol. 30, pp. 1905-1909, 2026.
<span class="paper-info">(Co-first Author, Primary Supervisor, JCR Q2, IF = 4.4, Top 50 Most Popular Papers)</span>
<a href="https://doi.org/10.1109/LCOMM.2026.3688633">Full Paper</a>
</li>


<li>
Yunxiao Li†,
<span class="author-name">Qian Zhang</span>†,
<span class="etal">et al.</span>,
"Secure transmission for fluid antenna-aided ISAC systems,"
<span class="journal-name">IEEE Wireless Communications Letters</span>,
2026.
<span class="paper-info">(Co-first Author, Primary Supervisor, JCR Q1, IF = 5.5)</span>
<a href="https://doi.org/10.1109/LWC.2026.3672225">Full Paper</a>
</li>


<li>
Yuhui Jiao†,
<span class="author-name">Qian Zhang</span>†,
<span class="etal">et al.</span>,
"Joint Power Allocation and Phase-Shift Design for Beyond-Diagonal Stacked Intelligent Metasurfaces-Aided ISAC Systems,"
<span class="journal-name">IEEE Wireless Communications Letters</span>,
2026.
<span class="paper-info">(Co-first Author, Primary Supervisor, JCR Q1, IF = 5.5)</span>
<a href="https://ieeexplore.ieee.org/abstract/document/11614485">Full Paper</a>
</li>


<li>
Xuejun Cheng,
<span class="author-name">Qian Zhang</span>,
<span class="etal">et al.</span>,
"Joint Beamforming and Phase Shifts Design for RIS-Enabled RSMA-ISAC Systems,"
<span class="journal-name">IEEE Wireless Communications Letters</span>,
2026.
<span class="paper-info">(Primary Supervisor, JCR Q1, IF = 5.5)</span>
<a href="https://doi.org/10.1109/LWC.2026.3725182">Full Paper</a>
</li>


<li>
Maoyuan Wang,
<span class="author-name">Qian Zhang</span>,
Jiancheng An,
<span class="etal">et al.</span>,
"DRL-Based Joint Beamforming and Surface Shape Optimization for Flexible Intelligent Metasurface-Aided ISAC Systems,"
<span class="journal-name">IEEE Wireless Communications Letters</span>.
<span class="paper-info">(Primary Supervisor, JCR Q1, IF = 5.5)</span>
<a href="https://doi.org/10.1109/LWC.2026.3709756">Full Paper</a>
</li>


<li>
Zhichao Gao,
<span class="author-name">Qian Zhang</span>,
Ju Liu,
<span class="etal">et al.</span>,
"DRL-based AP selection in downlink cell-free massive MIMO network with pilot contamination,"
<span class="journal-name">IEEE Communications Letters</span>,
vol. 28, no. 6, pp. 1432-1436, Jun. 2024.
<span class="paper-info">(JCR Q2, IF = 4.4)</span>
<a href="https://doi.org/10.1109/LCOMM.2024.3387095">Full Paper</a>
</li>


<li>
Ziyu Li,
Lina Zheng,
<span class="author-name">Qian Zhang</span>,
<span class="etal">et al.</span>,
"GNSS Jamming Attacks Recognition Based on Dual GCN With Adaptive Weight Learning,"
<span class="journal-name">IEEE Sensors Journal</span>,
vol. 25, no. 13, pp. 26152-26168, 1 Jul., 2025.
<span class="paper-info">(JCR Q1, IF = 4.5)</span>
<a href="https://doi.org/10.1109/JSEN.2025.3571189">Full Paper</a>
</li>


<li>
Ziyu Li,
Ju Liu,
Hui Wang,
<span class="author-name">Qian Zhang</span>,
<span class="etal">et al.</span>,
"Angle-Optimized Aided Dual Stream Harmonized Network for GNSS Jamming Recognition,"
<span class="journal-name">IEEE Transaction on Instrumentation and Measurement</span>,
2025.
<span class="paper-info">(JCR Q1, IF = 5.9)</span>
<a href="https://doi.org/10.1109/TIM.2025.3644543">Full Paper</a>
</li>


<li>
Jinyuan Liu,
Yong Liang Guan,
Hong Niu,
<span class="author-name">Qian Zhang</span>,
<span class="etal">et al.</span>,
"Fluid antennas meet rate-splitting multiple access: A new path forward for 6G networks,"
<span class="journal-name">IEEE Network</span>,
2025.
<span class="paper-info">(JCR Q1, IF = 6.3)</span>
<a href="https://doi.org/10.1109/MNET.2026.3685501">Full Paper</a>
</li>


<li>
Yufei Zhao,
Haoyang Shi,
<span class="author-name">Qian Zhang</span>,
<span class="etal">et al.</span>,
"Skin-inspired minimalist stacked intelligent meta-surfaces: from concept to prototype,"
<span class="journal-name">IEEE Communications Magazine</span>.
<span class="paper-info">(JCR Q1, IF = 8.3, Submitted)</span>
</li>


<li>
Xuejun Cheng,
<span class="author-name">Qian Zhang</span>,
<span class="etal">et al.</span>,
"Crem'er-Rao bound minimization for discrete SIM-aided ISAC systems,"
<span class="journal-name">IEEE Internet of Things Journal</span>,
2026.
<span class="paper-info">(Primary Supervisor, JCR Q1, IF = 8.33, Major Revision)</span>
</li>


</ol>

</section>


<!-- =========================================================
     Conference Papers
     ========================================================= -->

<section class="pub-section">

  <div class="pub-section-header">

    <div class="pub-section-bar"></div>

    <h2 class="pub-section-title">
      Conference Papers
    </h2>

    <div class="pub-section-description">
      Conference Proceedings
    </div>

  </div>


<ol class="pub-list">


<li>
<span class="author-name">Qian Zhang</span>,
Mingjie Shao, Qiang Li, and Ju Liu,
"An efficient algorithm for multiuser sum-rate maximization of large-scale active RIS-aided MIMO system,"
2024 IEEE International Conference on Acoustics, Speech and Signal Processing
(<span class="conference-name">ICASSP 2024</span>),
Seoul, Republic of Korea, 2024, pp. 9036-9040.
<span class="paper-info">(EI, CCF B, IEEE SPS Flagship Conference)</span>
<a href="https://ieeexplore.ieee.org/document/10446199">Full Paper</a>
</li>


<li>
<span class="author-name">Qian Zhang</span>,
Guanghui Luo,
<span class="etal">et al.</span>,
"RIS-aided MU-NOMA systems with imperfect CSI and generalized hardware impairments,"
2024 IEEE 99th Vehicular Technology Conference
(<span class="conference-name">VTC2024-Spring</span>),
Singapore, 2024, pp. 1-6.
<span class="paper-info">(EI, IEEE VTS Flagship Conference)</span>
<a href="https://ieeexplore.ieee.org/abstract/document/10683637">Full Paper</a>
</li>


<li>
Yuhui Jiao†,
<span class="author-name">Qian Zhang</span>†,
<span class="etal">et al.</span>,
"Efficient beamforming for discrete SIM-aided multiuser systems under statistical CSI,"
IEEE Wireless Communications and Networking Conference
(<span class="conference-name">WCNC 2026</span>).
<span class="paper-info">(Co-first Author, Primary Supervisor, IEEE Communications Society Flagship Conference)</span>
<a href="https://ieeexplore.ieee.org/document/11555646?denied=">Full Paper</a>
</li>


<li>
Xuejun Cheng†,
<span class="author-name">Qian Zhang</span>†,
<span class="etal">et al.</span>,
"Joint precoding and phase shift optimization for beyond-diagonal RIS-aided ISAC system,"
IEEE International Conference on Communications
(<span class="conference-name">ICC 2026</span>).
<span class="paper-info">(Co-first Author, Primary Supervisor, IEEE Communications Society Flagship Conference)</span>
<a href="https://ieeexplore.ieee.org/abstract/document/11586512">Full Paper</a>
</li>


<li>
Xuejun Cheng,
<span class="author-name">Qian Zhang</span>,
<span class="etal">et al.</span>,
"Robust Beamforming for Discrete RIS Enhanced RSMA-ISAC Systems,"
2025 IEEE/CIC International Conference on Communications in China
(<span class="conference-name">ICCC</span>),
Shanghai, China, 2025, pp. 1-6.
<span class="paper-info">(Primary Supervisor)</span>
<a href="https://ieeexplore.ieee.org/document/11148732">Full Paper</a>
</li>


<li>
Yunxiao Li,
<span class="author-name">Qian Zhang</span>,
Guanghui Luo,
<span class="etal">et al.</span>,
"Robust max-min SINR for active RIS aided multiuser MISO system with outage constraints,"
2024 IEEE/CIC International Conference on Communications in China
(<span class="conference-name">ICCC Workshops</span>),
Hangzhou, China, 2024, pp. 401-406.
<span class="paper-info">(Primary Supervisor)</span>
<a href="https://ieeexplore.ieee.org/document/10693724">Full Paper</a>
</li>


<li>
Zhiying Peng, Ju Liu, Zheng Dong, Zhichao Gao, and
<span class="author-name">Qian Zhang</span>,
"Time and Energy optimization Scheme of Task Offloading for Single-Cell MEC-D2D Networks,"
2022 3rd Information Communication Technologies Conference
(<span class="conference-name">ICTC</span>),
Nanjing, China, 2022.
<a href="https://ieeexplore.ieee.org/document/9778638">Full Paper</a>
</li>


<li>
Xiangcheng Wang, Ju Liu, Zheng Dong, Ziyu Li,
<span class="author-name">Qian Zhang</span>,
<span class="etal">et al.</span>,
"Link State Based Routing and Scheduling Co-Design of Time-Triggered Traffic in Time-Sensitive Networking,"
2023 IEEE/CIC International Conference on Communications in China
(<span class="conference-name">ICCC</span>),
Dalian, China, 2023, pp. 1-6.
<a href="https://ieeexplore.ieee.org/document/10233623">Full Paper</a>
</li>


<li>
Liangcheng Qiu, Yao Ge, Yisheng Chen,
<span class="author-name">Qian Zhang</span>,
<span class="etal">et al.</span>,
"AFDM-based grant-free random access with structured sparse Bayesian learning receiver,"
2026 IEEE Globecom Workshops
(<span class="conference-name">GC Wkshps</span>).
</li>


</ol>

</section>


<!-- =========================================================
     Footer
     ========================================================= -->

<div class="publications-footer-note">

  The publication list is continuously updated.
  Full texts can be accessed through the
  <strong>Full Paper</strong>
  links to IEEE Xplore or the corresponding DOI pages.
  † denotes co-first authorship, and * denotes corresponding authorship.

</div>


</div>
