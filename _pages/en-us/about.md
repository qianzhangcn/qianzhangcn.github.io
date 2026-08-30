---
page_id: about
layout: about
title: Profile
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
   页面整体
   ========================================================= */

html,
body {
    overflow-x: hidden;
}


/* =========================================================
   顶部区域：照片 + 个人信息 + Logo
   与中文主页保持一致
   ========================================================= */

.top-header-row {
    width: 100%;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    gap: 40px;
    margin-top: 10px;
    margin-bottom: 35px;

    /* Logo 使用绝对定位时必须保留 */
    position: relative;
}


/* =========================================================
   左侧照片
   ========================================================= */

.top-header-photo {
    flex: 0 0 auto;
}

.top-header-photo img {
    width: 190px;
    max-width: 100%;
    height: auto;
    display: block;
    border-radius: 4px;
}


/* =========================================================
   中间个人信息
   ========================================================= */

.top-header-info {
    flex: 1;
    min-width: 0;

    font-size: 16px;
    line-height: 2.0;

    /*
       给右侧 Logo 预留空间，
       避免英文较长时与 Logo 重叠
    */
    padding-right: 210px;
    box-sizing: border-box;
}

.top-header-info p {
    margin-top: 6px;
    margin-bottom: 6px;
}


/* =========================================================
   右侧 Logo
   可以通过 top 和 right 自定义位置
   ========================================================= */

.top-header-logo {
    position: absolute;

    top: 60px;      /* 越大越往下 */
    right: 40px;    /* 越大越往左 */

    z-index: 10;
}


/* Logo 大小 */

.top-header-logo img {
    width: 180px;
    height: auto;
    display: block;
}


/* =========================================================
   姓名与欢迎语
   ========================================================= */

.profile-name {
    margin-top: 5px;
    margin-bottom: 8px;
}

.profile-welcome {
    margin-top: 0;
    margin-bottom: 20px;
    font-size: 16px;
}


/* =========================================================
   正文排版
   ========================================================= */

.bio-justify p {
    text-align: justify;
    text-align-last: left;
    text-justify: inter-character;

    line-height: 1.8;

    margin-top: 0;
    margin-bottom: 1.3em;
}


/* =========================================================
   手机端适配
   ========================================================= */

@media screen and (max-width: 768px) {

    .container,
    .container.mt-5 {
        width: 100% !important;
        max-width: 100% !important;

        padding-left: 18px !important;
        padding-right: 18px !important;
    }


    /* =====================================================
       顶部区域手机端改为上下排列
       ===================================================== */

    .top-header-row {
        flex-direction: column;

        align-items: center;
        justify-content: center;

        gap: 18px;

        margin-top: 5px;
        margin-bottom: 28px;
    }


    /* 手机端照片 */

    .top-header-photo {
        width: 100%;
        text-align: center;
    }

    .top-header-photo img {
        width: 190px;
        max-width: 78%;

        margin-left: auto;
        margin-right: auto;
    }


    /* 手机端个人信息 */

    .top-header-info {
        width: 100%;

        font-size: 15px;
        line-height: 1.8;

        padding-right: 0;
    }

    .top-header-info p {
        margin-top: 4px;
        margin-bottom: 4px;
    }


    /* =====================================================
       手机端 Logo
       取消电脑端绝对定位
       ===================================================== */

    .top-header-logo {
        position: static;

        width: 100%;
        text-align: center;

        margin-top: 5px;
    }

    .top-header-logo img {
        width: 0px;

        margin-left: auto;
        margin-right: auto;
    }


    h2 {
        font-size: 24px;
    }


    html,
    body {
        overflow-x: hidden !important;
    }
}

</style>


<!-- =====================================================
     顶部区域：照片 + 英文个人信息 + Logo
     ===================================================== -->

<div class="top-header-row">

  <div class="top-header-photo">
    <img src="{{ '/assets/img/Qian_Zhang_GitHub.png' | relative_url }}" alt="Qian Zhang">
  </div>

  <div class="top-header-info">
    <p>- Institution: Northeastern University at Qinhuangdao</p>
    <p>- School: School of Computer and Communication Engineering</p>
    <p>- Academic Rank: Associate Professor</p>
    <p>- Degree: Ph.D. in Engineering</p>
    <p>- Alma Mater: Shandong University</p>
    <p>- Email: zq869054246@163.com</p>
  </div>

  <div class="top-header-logo">
    <img src="{{ '/assets/img/ICS_LOGO.png' | relative_url }}" alt="ICS Logo">
  </div>

</div>


# **Qian Zhang**

Welcome to my personal homepage!

---

## 👨‍🏫 **Basic Information**

<div class="bio-justify" markdown="1">

**Qian Zhang**, **Ph.D. in Engineering**, **Associate Professor**, IEEE Member, Member of the China Institute of Communications, Committee Member of the CSIG Traffic Video Special Committee.  
In 2021, he was recommended for admission to the direct Ph.D. program at Shandong University, under the supervision of Prof. Ju Liu (Level-II Professor) and Prof. Zheng Dong.  
In 2024, supported by the **China Scholarship Council**, he joined the School of Electrical and Electronic Engineering at Nanyang Technological University (NTU), Singapore, as a visiting Ph.D. student, under the joint supervision of Prof. Yong Liang Guan (Vice President of NTU) and Prof. Chau Yuen (IEEE Fellow).  
He received the Ph.D. degree in Engineering from Shandong University in June 2026.

His current research interests include intelligent metasurfaces, convex optimization theory, and artificial intelligence algorithms for wireless communications and sensing.  
He has published nearly 30 academic papers in top-tier journals and conferences in wireless communications, including IEEE TWC, IEEE TCOM, IEEE ICC, and IEEE ICASSP, among which 15 papers were published as the first or co-first author.  
Two of his first-authored papers were recognized as **🏆ESI Highly Cited Papers**. One of his first-authored papers was selected as one of the **Top 2 Most Popular Papers of the Year in IEEE CL**, and four papers were ranked in the **Top 50 Most Popular Papers of the Month by IEEE TVT, WCL, and CL**, respectively (1 first-authored paper, 2 co-first-authored papers, and 1 second-authored paper).  
He has been granted three patents. He serves as a **Young Editorial Board Member of China Communications** and a **TPC Chair for IEEE PIMRC 2026**. He has also served multiple times as a TPC Member for international conferences, including IEEE ICC, IEEE GLOBECOM, and IEEE WCNC. He regularly serves as a reviewer for more than ten international journals, including IEEE JSAC, TWC, TCOM, WCM, TIFS, TCCN, TVT, TITS, IOTJ, WCL, and CL.

As a core member, he has participated in several major national- and provincial-level projects, including the National Key Research and Development Program of China, the General Program of the National Natural Science Foundation of China, and the Key Research and Development Program of Shandong Province (Major Science and Technology Demonstration Project).  
He has received the Outstanding Doctoral/Bachelor's Thesis Award, the Outstanding Graduate Awards of Shandong Province and Shandong University, **two National Scholarships for Doctoral Students**, **the National Scholarship for Undergraduate Students**, the **2026 Academic Star Award of Shandong University as the sole recipient from his school**, the **2026 Outstanding Graduate Research Achievement Award of Shandong University as the sole recipient from his school**, First-Class Scholarships throughout his four undergraduate years, and more than ten awards in national- and provincial-level innovation, entrepreneurship, and disciplinary competitions.

</div>

---

## 🎓 **Academic Background**

- 2026.07—Present  School of Computer and Communication Engineering, Northeastern University at Qinhuangdao, **Associate Professor**
- 2024.11—2025.11  School of Electrical and Electronic Engineering, Nanyang Technological University, Singapore, **Visiting Ph.D. Student**, Supervisors: Yong Liang Guan (Vice President) and Chau Yuen (IEEE Fellow)
- 2021.09—2026.06  School of Information Science and Engineering, Shandong University, **Ph.D. in Engineering**, Supervisor: Prof. Ju Liu (Level-II Professor)

---

## 🔬 **Research Interests**

- Extremely Large-Scale MIMO Communications (XL-MIMO)
- Intelligent Metasurfaces (IMS)
- Integrated Sensing and Communication (ISAC)
- Near-Field Wireless Communications
- Beam Training
- Deep Unfolding

---

## 🌐 **Academic Services**

- Young Editorial Board Member of China Communications
- Committee Member of the CSIG Traffic Video Special Committee
- TPC Chair, IEEE PIMRC 2026
- TPC Member for international conferences, including IEEE ICC, GLOBECOM, and WCNC
- Reviewer for more than ten international journals, including IEEE JSAC, TWC, TCOM, WCM, TIFS, TCCN, TVT, TITS, IOTJ, WCL, and CL

---

## 📖 **Representative Achievements**

**-** **For details, please refer to the Publications page at the top**

**-** **Authored 11 papers as the first author**: 10 published papers (3 in IEEE TWC, 1 in IEEE TCOM, 2 in IEEE TVT, 1 in IEEE WCL, 1 in IEEE CL, 1 in ICASSP, and 1 in VTC); 1 paper under review (1 IEEE JSAC paper under major revision). Among them, 2 papers were recognized as ESI Highly Cited Papers, 1 paper was ranked among the Top 2 Most Popular Papers of the Year in IEEE CL, and 1 paper was ranked among the Top 50 Most Popular Papers in IEEE CL.

**-** **Authored 6 papers as a co-first author**: 5 published papers (1 in IEEE TVT, 1 in IEEE WCL, 1 in IEEE CL, 1 in ICC, and 1 in WCNC); 1 paper under review (1 IEEE WCL paper under review).


**-** **Patent Applications**

[1] Fuhui Sun; Qian Zhang; Xiaoyan Wang; Mingjie Shao; Ju Liu; Sum-Rate Optimization Method and Apparatus for RIS-Assisted MIMO Systems. (Invention Patent, Grant No.: CN117176214B)

[2] Ju Liu; Xuejun Cheng; Qian Zhang; Guanghui Luo; Yuhui Jiao; A Beamforming Method for Practical Intelligent Metasurface-Assisted RSMA Systems. (Invention Patent, Publication No.: CN120110450A)

[3] Ju Liu; Xuejun Cheng; Guanghui Luo; Qian Zhang; Zheng Dong; A Beamforming Method for Beyond-Diagonal Intelligent Metasurface-Assisted NOMA Systems. (Invention Patent, Publication No.: CN119051703A)

[4] Ju Liu; Zhiying Peng; Xiangcheng Wang; Qian Zhang; Zhichao Gao; Ziyu Li; A Joint Task Offloading and Resource Allocation Method for Multi-Server MEC-D2D Systems. (Invention Patent, Publication No.: CN116456497A)

---

## 🏆 **Honors and Awards**

- Recommended Admission to Graduate Study without Entrance Examination (2020)
- National Scholarship for Undergraduate Students (2020, ranked first in the school)
- National Encouragement Scholarship (2018, 2019)
- National Scholarship for Doctoral Students (2024, 2025)
- Outstanding Graduate of Shandong Province (2021)
- Outstanding Graduate of Shandong University (2026)
- Academic Star of Shandong University (2026, the sole recipient from the school)
- Outstanding Graduate Research Achievement Award of Shandong University (2026, the sole recipient from the school)
- Excellence Award in the Ph.D. Midterm Assessment (ranked first)
- First-Class Undergraduate Academic Scholarship (the sole recipient in the major throughout all four years)
- Outstanding Ph.D. Student Source Scholarship and First-Class Scholarship for New Graduate Students

---

## 🤝 **Student Recruitment and Collaboration**

Undergraduate, master's, and doctoral students interested in wireless communications, intelligent metasurfaces, integrated sensing and communication, and AI-enabled communication optimization are welcome to contact me for academic exchange and collaboration.

Email: zhangqian@neuq.edu.cn; zq869054246@163.com.

---

<div style="text-align: center; margin-top: 30px; font-size: 14px; opacity: 0.75;">
  👁️ Total Visits:
  <span id="busuanzi_site_pv">Loading...</span>
  &nbsp;&nbsp;|&nbsp;&nbsp;
  👤 Total Visitors:
  <span id="busuanzi_site_uv">Loading...</span>
</div>

<script src="https://cdn.busuanzi.cc/busuanzi/3.6.9/busuanzi.min.js" defer></script>
