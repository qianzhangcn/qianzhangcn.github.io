---
page_id: Publications
layout: page
title:
permalink: /Publications/
title: Publications
description: Main research achievements in the fields of wireless communication and sensing
nav: true
nav_order: 2
---
<style>

/* =========================================================
   Publications 标题 + ICS Logo
   Logo嵌入正常文本布局
   ========================================================= */

.publications-header {
    width: 100%;

    display: flex;
    flex-direction: row;

    align-items: center;
    justify-content: space-between;

    margin-top: 5px;
    margin-bottom: 15px;
}


/* Publications标题 */
.publications-header-title {
    flex: 1;
}


/* 标题本身 */
.publications-header-title h2 {
    margin-top: 0;
    margin-bottom: 0;
}


/* 右侧Logo */
.publications-header-logo {
    flex: 0 0 auto;

    margin-left: 40px;

    display: flex;
    align-items: center;
    justify-content: center;
}


/* Logo大小 */
.publications-header-logo img {
    width: 150px;
    height: auto;
    display: block;
}


/* =========================================================
   手机端
   ========================================================= */

@media screen and (max-width: 768px) {

    .publications-header {
        flex-direction: column;

        align-items: flex-start;

        gap: 15px;
    }


    .publications-header-logo {
        width: 100%;

        margin-left: 0;

        justify-content: center;
    }


    .publications-header-logo img {
        width: 90px;
    }

}

</style>


<style>
.pub-list {
  list-style: none;
  counter-reset: pub-counter;
  padding-left: 0;
  margin-left: 0;
  margin-top: 0;
}

.pub-list > li {
  counter-increment: pub-counter;
  position: relative;
  padding-left: 3.2em;

  /* 每篇论文之间的间距 */
  margin-bottom: 0.7em;

  /* 同一篇论文内部的行距 */
  line-height: 1.65;

  text-align: justify;
  font-family: "Times New Roman", "Songti SC", "SimSun", serif;
  font-size: 17px;
  font-weight: 400;
}

/* 自动生成 [1]、[2]、[3] ... */
.pub-list > li::before {
  content: "[" counter(pub-counter) "]";
  position: absolute;
  left: 0;
  top: 0;
  width: 2.5em;
  text-align: right;

  font-family: "Times New Roman", serif;
  font-size: 17px;
  font-weight: 400;
}

/* Qian Zhang：粗体正体 */
.pub-list .author-name {
  font-weight: 700 !important;
  font-style: normal !important;
}

/* 期刊名称：粗体 + 斜体 */
.pub-list .journal-name {
  font-weight: 700 !important;
  font-style: italic !important;
}

/* et al.：斜体 */
.pub-list .etal {
  font-style: italic !important;
  font-weight: 400 !important;
}

/* JCR、IF、论文状态等：加粗 */
.pub-list .paper-info {
  font-weight: 800 !important;
  font-style: normal !important;
}

/* 会议简称：加粗 */
.pub-list .conference-name {
  font-weight: 800 !important;
  font-style: normal !important;
}
</style>
  
<div class="publications-header">

  <div class="publications-header-title">
    <h2>📚 <strong>Publications</strong></h2>
    <div style="margin-top: 6px;">
      (†共同一作、*通讯作者)
    </div>
  </div>

  <div class="publications-header-logo">
    <img src="{{ '/assets/img/ICS_LOGO.png' | relative_url }}" alt="ICS Logo">
  </div>

</div>

---

### 📘 **Journal Papers**

<ol class="pub-list">

<li>
<span class="author-name">Qian Zhang</span>, 
<span class="etal">et al.</span>, 
"Hierarchical sub-array beam training for flexible intelligent metasurface-enabled hybrid near-far-field multiuser communications," 
<span class="journal-name">IEEE Journal on Selected Areas in Communications</span>, 
2026. 
  <span class="paper-info">(JCR Q1, IF = 16.8, 大修)</span>
</li>

<li>
<span class="author-name">Qian Zhang</span>, 
<span class="etal">et al.</span>, 
"RIS-assisted multiuser NOMA networks with imperfect CSI under transceiver hardware impairments," 
<span class="journal-name">IEEE Internet of Things Journal</span>, 
2026. 
  <span class="paper-info">(JCR Q1, IF = 8.33, 在修)</span>
</li>

<li>
<span class="author-name">Qian Zhang</span>, 
<span class="etal">et al.</span>, 
"Discrete-Phase RIS-Aided Covert Communications With Random Element-Control Failures and Residual Reflection," 
<span class="journal-name">IEEE Transactions on Wireless Communications </span>, 
2026. 
<span class="paper-info">(JCR Q1, IF = 10.3, 准备中)</span>
</li>

<li>
<span class="author-name">Qian Zhang</span>, 
Zheng Dong, 
<span class="etal">et al.</span>, 
"Multi-resolution codebook design and multiuser interference management for discrete XL-RIS-aided near-field MIMO systems," 
<span class="journal-name">IEEE Transactions on Wireless Communications</span>, 
vol. 25, pp. 2826-2842, 2026. 
<span class="paper-info">(JCR Q1, IF = 10.7, 🏆 ESI高被引)</span>
<a href="https://doi.org/10.1109/TWC.2025.3599514">DOI</a>
</li>

<li>
<span class="author-name">Qian Zhang</span>, 
Ju Liu, 
<span class="etal">et al.</span>, 
"Practical RIS-aided multiuser communications with imperfect CSI: Practical model, amplitude feedback, and beamforming optimization," 
<span class="journal-name">IEEE Transactions on Wireless Communications</span>, 
vol. 23, no. 10, pp. 15245-15260, Oct. 2024. 
  <span class="paper-info">(JCR Q1, IF = 10.7) </span>
<a href="https://doi.org/10.1109/TWC.2024.3427695">DOI</a>
</li>

<li>
<span class="author-name">Qian Zhang</span>, 
Ju Liu, 
<span class="etal">et al.</span>, 
"Two-Stage Coded-Sliding Beam Training and QoS-constrained sum-rate maximization for SIM-assisted wireless communications," 
<span class="journal-name">IEEE Transactions on Wireless Communications</span>, 
vol. 25, pp. 12162-12179, 2026. 
  <span class="paper-info">(JCR Q1, IF = 10.7) </span>
<a href="https://doi.org/10.1109/TWC.2026.3661858">DOI</a>
</li>

<li>
<span class="author-name">Qian Zhang</span>, 
Ju Liu, 
<span class="etal">et al.</span>, 
"Robust beamforming design for RIS-aided NOMA secure networks with transceiver hardware impairments," 
<span class="journal-name">IEEE Transactions on Communications</span>, 
vol. 71, no. 6, pp. 3637-3649, Jun. 2023. 
  <span class="paper-info">(JCR Q1, IF = 8.3) </span>
<a href="https://doi.org/10.1109/TCOMM.2023.3251345">DOI</a>
</li>

<li>
<span class="author-name">Qian Zhang</span>, 
Zhengfeng Du, 
<span class="etal">et al.</span>, 
"Joint power allocation and discrete phase-shift optimization for SIM-aided ISAC systems," 
<span class="journal-name">IEEE Transactions on Vehicular Technology</span>, 
vol. 74, no. 12, pp. 19795-19800, Dec. 2025. 
  <span class="paper-info">(JCR Q1, IF = 7.1)</span>
<a href="https://doi.org/10.1109/TVT.2025.3584064">DOI</a>
</li>

<li>
<span class="author-name">Qian Zhang</span>, 
Yufei Zhao, 
<span class="etal">et al.</span>, 
"Crem'er-Rao bound minimization for flexible intelligent metasurfaces enabled ISAC systems," 
<span class="journal-name">IEEE Transactions on Vehicular Technology</span>, 
2025. 
  <span class="paper-info">(JCR Q1, IF = 7.1)</span>
<a href="https://doi.org/10.1109/TVT.2026.3701078">DOI</a>
</li>

<li>
<span class="author-name">Qian Zhang</span>, 
Mingjie Shao, 
<span class="etal">et al.</span>, 
"An efficient sum-rate maximization algorithm for fluid antenna-assisted ISAC system," 
<span class="journal-name">IEEE Communications Letters</span>, 
vol. 29, no. 1, pp. 200-204, Jan. 2025. 
  <span class="paper-info">(JCR Q2, IF = 4.4, 🏆 ESI高被引, 年度最受欢迎论文TOP2) </span>
<a href="https://doi.org/10.1109/LCOMM.2024.3510334">DOI</a>
</li>

<li>
<span class="author-name">Qian Zhang</span>†, 
Guanghui Luo†, 
<span class="etal">et al.</span>, 
"Beyond-diagonal reconfigurable intelligent surface enhanced NOMA systems," 
<span class="journal-name">IEEE Wireless Communications Letters</span>, 
vol. 14, no. 1, pp. 118-122, Jan. 2025. 
   <span class="paper-info">(JCR Q1, IF = 5.5) </span>
<a href="https://doi.org/10.1109/LWC.2024.3489718">DOI</a>
</li>

<li>
Xuejun Cheng†, 
<span class="author-name">Qian Zhang</span>†, 
Yunnuo Xu, 
<span class="etal">et al.</span>, 
"Robust beamforming for non-ideal RIS enabled rate-splitting multiple access systems," 
<span class="journal-name">IEEE Transactions on Vehicular Technology</span>, 
2025. 
  <span class="paper-info">(共一, 主要指导人, JCR Q1, IF = 7.1) </span>
<a href="https://doi.org/10.1109/TVT.2026.3677351">DOI</a>
</li>

<li>
Maoyuan Wang†, 
<span class="author-name">Qian Zhang</span>†, 
<span class="etal">et al.</span>, 
"DRL-Based Antenna Position Optimization for MA-Assisted OTFS System Under Imperfect CSI," 
<span class="journal-name">IEEE Communications Letters</span>, 
vol. 30, pp. 1905-1909, 2026. 
  <span class="paper-info">(共一, 主要指导人, JCR Q2, IF = 4.4, 最受欢迎论文TOP 50) </span>
<a href="https://doi.org/10.1109/LCOMM.2026.3688633">DOI</a>
</li>

<li>
Yunxiao Li†, 
<span class="author-name">Qian Zhang</span>†, 
<span class="etal">et al.</span>, 
"Secure transmission for fluid antenna-aided ISAC systems," 
<span class="journal-name">IEEE Wireless Communications Letters</span>, 
2026. 
  <span class="paper-info">(共一，主要指导人, JCR Q1, IF = 5.5) </span>
<a href="https://doi.org/10.1109/LWC.2026.3672225">DOI</a>
</li>

<li>
Yuhui Jiao†, 
<span class="author-name">Qian Zhang</span>†, 
<span class="etal">et al.</span>, 
"Joint Power Allocation and Phase-Shift Design for Beyond-Diagonal Stacked Intelligent Metasurfaces-Aided ISAC Systems," 
<span class="journal-name">IEEE Wireless Communications Letters</span>, 
2026. 
  <span class="paper-info">(共一, 主要指导人, JCR Q1, IF = 5.5)</span>
<a href="https://ieeexplore.ieee.org/abstract/document/11614485">DOI</a>
</li>

<li>
Xuejun Cheng, 
<span class="author-name">Qian Zhang</span>, 
<span class="etal">et al.</span>, 
"Joint Beamforming and Phase Shifts Design for RIS-Enabled RSMA-ISAC Systems," 
<span class="journal-name">IEEE Wireless Communications Letters</span>, 
2026. 
  <span class="paper-info">(主要指导人, JCR Q1, IF = 5.5)</span>
<a href="https://doi.org/10.1109/LWC.2026.3725182">DOI</a>
</li>

<li>
Maoyuan Wang, 
<span class="author-name">Qian Zhang</span>, 
Jiancheng An, 
<span class="etal">et al.</span>, 
"DRL-Based Joint Beamforming and Surface Shape Optimization for Flexible Intelligent Metasurface-Aided ISAC Systems," 
<span class="journal-name">IEEE Wireless Communications Letters</span>. 
  <span class="paper-info">(主要指导人, JCR Q1, IF = 5.5) </span>
<a href="https://doi.org/10.1109/LWC.2026.3709756">DOI</a>
</li>

<li>
Zhichao Gao, 
<span class="author-name">Qian Zhang</span>, 
Ju Liu, 
<span class="etal">et al.</span>, 
"DRL-based AP selection in downlink cell-free massive MIMO network with pilot contamination," 
<span class="journal-name">IEEE Communications Letters</span>, 
vol. 28, no. 6, pp. 1432-1436, Jun. 2024. 
  <span class="paper-info">(JCR Q2, IF = 4.4) </span>
<a href="https://doi.org/10.1109/LCOMM.2024.3387095">DOI</a>
</li>

<li>
Ziyu Li, 
Lina Zheng, 
<span class="author-name">Qian Zhang</span>, 
<span class="etal">et al.</span>, 
"GNSS Jamming Attacks Recognition Based on Dual GCN With Adaptive Weight Learning," 
<span class="journal-name">IEEE Sensors Journal</span>, 
vol. 25, no. 13, pp. 26152-26168, 1 Jul., 2025. 
  <span class="paper-info">(JCR Q1, IF = 4.5) </span>
<a href="https://doi.org/10.1109/JSEN.2025.3571189">DOI</a>
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
  <span class="paper-info">(JCR Q1, IF = 5.9) </span>
<a href="https://doi.org/10.1109/TIM.2025.3644543">DOI</a>
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
  <span class="paper-info">(JCR Q1, IF = 6.3) </span>
<a href="https://doi.org/10.1109/MNET.2026.3685501">DOI</a>
</li>

<li>
Yufei Zhao, 
Deyu Lin, 
<span class="author-name">Qian Zhang</span>, 
<span class="etal">et al.</span>, 
"Enhanced information security via wave-field selectivity and structured wavefront manipulation," 
<span class="journal-name">IEEE Transactions on Wireless Communications</span>, 
2025. 
  <span class="paper-info">(JCR Q1, IF = 10.7, 大修)</span>
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
  <span class="paper-info">(主要指导人, JCR Q1, IF = 8.33, 在修)</span>
</li>

</ol>

---

### 🧑‍🏫 **Conference Papers**

<ol class="pub-list">

<li>
<span class="author-name">Qian Zhang</span>, 
Mingjie Shao, Qiang Li, and Ju Liu, 
"An efficient algorithm for multiuser sum-rate maximization of large-scale active RIS-aided MIMO system," 
ICASSP 2024 - 2024 IEEE International Conference on Acoustics, Speech and Signal Processing 
(<span class="conference-name">ICASSP</span>), 
Seoul, Korea, Republic of, 2024, pp. 9036-9040. 
<span class="paper-info">(EI, CCF B, IEEE SPS旗舰会议)</span> 
<a href="https://ieeexplore.ieee.org/document/10446199">DOI</a>
</li>

<li>
<span class="author-name">Qian Zhang</span>, 
Guanghui Luo, 
<span class="etal">et al.</span>, 
"RIS-aided MU-NOMA systems with imperfect CSI and generalized hardware impairments," 
2024 IEEE 99th Vehicular Technology Conference 
(<span class="conference-name">VTC2024-Spring</span>), 
Singapore, Singapore, 2024, pp. 1-6. 
<span class="paper-info">(EI, IEEE VTS旗舰会议)</span> 
<a href="https://ieeexplore.ieee.org/abstract/document/10683637">DOI</a>
</li>

<li>
Yuhui Jiao†, 
<span class="author-name">Qian Zhang</span>†, 
<span class="etal">et al.</span>, 
"Efficient beamforming for discrete SIM-aided multiuser systems under statistical CSI," 
<span class="conference-name">WCNC2026</span> - IEEE Wireless Communications and Networking Conference (WCNC). 
<span class="paper-info">(共一，主要指导人, IEEE通信协会旗舰会议)</span>
<a href="https://ieeexplore.ieee.org/document/11555646?denied=">DOI</a>
</li>

<li>
Xuejun Cheng†, 
<span class="author-name">Qian Zhang</span>†, 
<span class="etal">et al.</span>, 
"Joint precoding and phase shift optimization for beyond-diagonal RIS-aided ISAC system," 
<span class="conference-name">ICC2026</span> - IEEE International Conference on Communications (ICC). 
<span class="paper-info">(共一, 主要指导人, IEEE通信协会旗舰会议)</span> 
<a href="https://ieeexplore.ieee.org/abstract/document/11586512">DOI</a>
</li>

<li>
Xuejun Cheng, 
<span class="author-name">Qian Zhang</span>, 
<span class="etal">et al.</span>, 
"Robust Beamforming for Discrete RIS Enhanced RSMA-ISAC Systems," 
2025 IEEE/CIC International Conference on Communications in China 
(<span class="conference-name">ICCC</span>), 
Shanghai, China, 2025, pp. 1-6. 
<span class="paper-info">(主要指导人)</span> 
<a href="https://ieeexplore.ieee.org/document/11148732">DOI</a>
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
<span class="paper-info">(主要指导人)</span> 
<a href="https://ieeexplore.ieee.org/document/10693724">DOI</a>
</li>

<li>
Zhiying Peng, Ju Liu, Zheng Dong, Zhichao Gao, and 
<span class="author-name">Qian Zhang</span>, 
"Time and Energy optimization Scheme of Task Offloading for Single-Cell MEC-D2D Networks," 
2022 3rd Information Communication Technologies Conference 
(<span class="conference-name">ICTC</span>), 
Nanjing, China, 2022. 
<a href="https://ieeexplore.ieee.org/document/9778638">DOI</a>
</li>

<li>
Xiangcheng Wang, Ju Liu, Zheng Dong, Ziyu Li, 
<span class="author-name">Qian Zhang</span>, 
<span class="etal">et al.</span>, 
"Link State Based Routing and Scheduling Co-Design of Time-Triggered Traffic in Time-Sensitive Networking," 
2023 IEEE/CIC International Conference on Communications in China 
(<span class="conference-name">ICCC</span>), 
Dalian, China, 2023, pp. 1-6. 
<a href="https://ieeexplore.ieee.org/document/10233623">DOI</a>
</li>

</ol>
