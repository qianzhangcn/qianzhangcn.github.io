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
   顶部：照片 + 右侧个人信息
   让两边上下高度更协调
   ========================================================= */

.top-profile-row {
    width: 100%;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: flex-start;
    gap: 50px;
    margin-top: 10px;
    margin-bottom: 35px;
}

/* 左侧照片区域 */
.top-profile-photo {
    flex: 0 0 auto;
}

.top-profile-photo img {
    height: 320px;          /* 核心：控制照片高度 */
    width: auto;
    max-width: 100%;
    display: block;
    border-radius: 4px;
}

/* 右侧个人信息区域 */
.top-profile-info {
    min-height: 320px;      /* 核心：与照片高度对应 */
    display: flex;
    flex-direction: column;
    justify-content: center;
    font-size: 16px;
    line-height: 2.0;
}

.top-profile-info p {
    margin-top: 5px;
    margin-bottom: 5px;
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
   基本信息正文 + 右侧 Logo
   ========================================================= */

.basic-info-wrapper {
    width: 100%;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: flex-start;
    gap: 35px;
}

.basic-info-text {
    flex: 1;
    min-width: 0;
}

.basic-info-text p {
    text-align: justify;
    text-align-last: left;
    text-justify: inter-character;
    line-height: 1.8;
    margin-top: 0;
    margin-bottom: 1.3em;
}

.basic-info-logo {
    flex: 0 0 180px;
    display: flex;
    align-items: center;
    justify-content: center;
}

.basic-info-logo img {
    width: 170px;           /* 核心：控制Logo大小 */
    max-width: 100%;
    height: auto;
    display: block;
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

    /* 顶部区域手机端改为上下排列 */
    .top-profile-row {
        flex-direction: column;
        align-items: center;
        gap: 18px;
        margin-top: 5px;
        margin-bottom: 28px;
    }

    .top-profile-photo {
        width: 100%;
        text-align: center;
    }

    .top-profile-photo img {
        height: auto;
        width: 220px;
        max-width: 80%;
        margin-left: auto;
        margin-right: auto;
    }

    .top-profile-info {
        min-height: auto;
        width: 100%;
        font-size: 15px;
        line-height: 1.8;
    }

    .top-profile-info p {
        margin-top: 4px;
        margin-bottom: 4px;
    }

    /* 基本信息区域手机端改为上下排列 */
    .basic-info-wrapper {
        flex-direction: column;
        align-items: center;
        gap: 18px;
    }

    .basic-info-text {
        width: 100%;
    }

    .basic-info-logo {
        width: 100%;
    }

    .basic-info-logo img {
        width: 95px;
        margin: 0 auto;
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
     页面顶部：左照片 + 右个人信息
     ===================================================== -->

<div class="top-profile-row">

  <div class="top-profile-photo">
    <img src="{{ '/assets/img/Qian_Zhang_GitHub.png' | relative_url }}" alt="Qian Zhang">
  </div>

  <div class="top-profile-info">
    <p>- 学校: 东北大学秦皇岛分校</p>
    <p>- 学院: 计算机与通信工程学院</p>
    <p>- 职称: 副教授</p>
    <p>- 学历: 工学博士</p>
    <p>- 毕业院校: 山东大学</p>
    <p>- 邮箱: zq869054246@163.com</p>
  </div>

</div>


# 张迁

欢迎访问我的个人主页！

---

## 👨‍🏫 **基本信息**

<div class="basic-info-wrapper">

  <div class="basic-info-text">

  <p><strong>张迁</strong>，<strong>工学博士</strong>，<strong>副教授</strong>，IEEE Member，中国通信学会会员，CSIG交通视频专委会委员。2026年6月于山东大学获得工学博士学位（直博），师从刘琚教授（二级），合作导师董郑教授；2024年受<strong>国家留学基金委资助</strong>赴新加坡南洋理工大学EEE学院联合培养，师从Prof. Yong Liang Guan（副校长）和Prof. Chau Yuen（IEEE Fellow）。</p>

  <p>目前主要从事智能超表面、凸优化理论、人工智能算法在无线通信和感知领域应用的相关研究。在通信领域顶级期刊IEEE TWC、TCOM和顶级会议IEEE ICC、ICASSP等发表学术论文近30篇，其中第一/共一作者论文15篇。2篇论文入选<strong>🏆ESI高被引论文</strong>（一作），1篇论文位列<strong>IEEE CL年度最受欢迎论文TOP 2</strong>（一作），4篇论文分别位列<strong>IEEE TVT、WCL、CL月度最受欢迎论文TOP 50</strong>（1篇一作、2篇共一、1篇第二）。授权专利3项。担任《<strong>中国通信</strong>》(<strong>英文版</strong>)<strong>首届青年编委</strong>，担任2026 PIMRC TPC Chair；多次担任IEEE ICC、Globecom、WCNC等国际会议TPC Member；常年担任IEEE JSAC、TWC、TCOM、WCM、TIFS、TCCN、TVT、TITS、IOTJ、WCL、CL等十余家国际期刊审稿人。</p>

  <p>作为核心成员参与国家重点研发计划项目、国家自然科学基金面上项目、山东省重点研发计划（重大科技示范工程）项目等多项国家级省级重点项目。曾获优秀博士/学士毕业论文、山东省/山东大学优秀毕业生、<strong>博士国家奖学金2次</strong>、<strong>本科国家奖学金</strong>、2026年<strong>山东大学学术之星（学院唯一）</strong>、2026年<strong>山东大学研究生优秀成果奖（学院唯一）</strong>、一等奖学金（本科4年）、以及国家级省级创新创业类及学科类竞赛奖项十余项。</p>

  </div>

  <div class="basic-info-logo">
    <img src="{{ '/assets/img/ICS_LOGO.png' | relative_url }}" alt="ICS Logo">
  </div>

</div>

---

## 🎓 **学术背景**

- 2026.07—至今     东北大学秦皇岛分校 计算机与通信工程学院， 副教授
- 2024.11—2025.11  新加坡南洋理工大学EEE，            联合培养博士，   导师：Yong Liang Guan（副校长）、Chau Yuen（IEEE Fellow）
- 2021.09—2026.06  山东大学信息科学与工程学院，        工学博士，      导师: 刘琚教授（二级）

---

## 🔬 **研究方向**

- 超大规模阵列通信（XL-MIMO）
- 智能超表面（IMS）
- 通感一体化（ISAC）
- 近场无线通信
- 波束训练
- Deep Unfolding

---

## 🌐 **学术服务**

- 《中国通信》(英文版)首届青年编委
- CSIG交通视频专委会委员
- IEEE PIMRC 2026 TPC Chair
- IEEE ICC、GLOBECOM、WCNC 等国际会议 TPC Member
- IEEE JSAC、TWC、TCOM、WCM、TIFS、TCCN、TVT、TITS、IOTJ、WCL、CL等十余家国际期刊审稿人

---

## 📖 **代表性成果**

**-** **详情见顶部Publications页面**

**-** **以第一作者完成论文11篇**：已发表10篇 (3篇IEEE TWC、1篇IEEE TCOM、2篇IEEE TVT、1篇IEEE WCL、1篇IEEE CL、1篇ICASSP、1篇VTC)；在审1篇 (1篇IEEE JSAC大修)；其中2篇论文获得ESI高被引论文、1篇论文位列IEEE CL年度最受欢迎论文TOP 2、1篇论文位列IEEE CL最受欢迎论文TOP 50

**-** **以共同第一作者完成论文6篇**：已发表5篇 (1篇IEEE TVT、1篇IEEE WCL、1篇IEEE CL、1篇ICC、1篇WCNC)；在审1篇 (1篇IEEE WCL在审)


**-** **申请专利**

[1] 孙福辉; 张迁; 王晓燕; 邵明杰; 刘琚; RIS辅助的MIMO系统的和速率优化方法及装置. (发明专利，授权号：CN117176214B)

[2] 刘琚; 程学军; 张迁; 罗广惠; 焦钰辉; 一种实际智能超表面辅助RSMA系统波束成形方法. (发明专利，公开号：CN120110450A)

[3] 刘琚; 程学军; 罗广惠; 张迁; 董郑; 一种超对角智能超表面辅助NOMA系统波束成形方法. (发明专利，公开号：CN119051703A)

[4] 刘琚; 彭志颖; 王祥丞; 张迁; 高智超; 李紫宇; 一种多服务器MEC-D2D系统联合任务卸载与资源分配方法. (发明专利, 公开号：CN116456497A)

---

## 🏆 **荣誉奖励**

- 推荐免试攻读研究生资格（2020）
- 本科国家奖学金（2020、学院排名第一）
- 国家励志奖学金（2018、2019）
- 博士国家奖学金（2024、2025）
- 山东省优秀毕业生（2021）
- 山东大学优秀毕业生（2026）
- 山东大学学术之星（2026、学院唯一）
- 山东大学研究生优秀成果奖（2026、学院唯一）
- 博士中期考核优秀奖（排名第一）
- 本科一等学业奖学金（四年专业唯一）
- 博士优秀生源奖学金、新生一等奖学金

---

## 🤝 **招生与合作**

常年与新加坡南洋理工大学、山东大学、电子科技大学、西北工业大学、南京理工大学等国内外知名高校保持科研合作。
欢迎对无线通信、智能超表面、通感一体化、人工智能通信优化等方向感兴趣的本科生、硕士生及博士生联系交流。个人邮箱：zhangqian@neuq.edu.cn; zq869054246@163.com。

---

<div style="text-align: center; margin-top: 30px; font-size: 14px; opacity: 0.75;">
  👁️ 本站总访问量：
  <span id="busuanzi_site_pv">加载中...</span> 次
  &nbsp;&nbsp;|&nbsp;&nbsp;
  👤 本站总访客数：
  <span id="busuanzi_site_uv">加载中...</span> 人
</div>

<script src="https://cdn.busuanzi.cc/busuanzi/3.6.9/busuanzi.min.js" defer></script>
