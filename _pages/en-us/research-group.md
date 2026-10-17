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
   Page container
   ========================================================= */

.ics-page {
  --ics-accent: var(--global-theme-color, #b509ac);
  --ics-text: var(--global-text-color, #222222);
  --ics-muted: var(--global-text-color-light, #6b7280);
  --ics-border: var(--global-divider-color, #e5e7eb);
  --ics-surface: var(--global-card-bg-color, var(--global-bg-color, #ffffff));

  --ics-shadow: 0 3px 12px rgba(0, 0, 0, 0.025);

  --ics-hover-shadow:
    0 14px 32px rgba(0, 0, 0, 0.12),
    0 0 0 1px var(--ics-accent);

  width: 100%;
  max-width: 1120px;
  margin: 0 auto;
  padding-bottom: 40px;

  color: var(--ics-text);
  line-height: 1.8;
  overflow-wrap: break-word;
  isolation: isolate;
}

/* Typography */

.ics-page,
.ics-page * {
  box-sizing: border-box;
  font-family: "Times New Roman", Times, serif !important;
}

.ics-page a {
  color: var(--ics-accent);
  text-decoration: none;
}

.ics-page a:hover {
  text-decoration: underline;
  text-underline-offset: 3px;
}

.ics-page a:focus-visible {
  outline: 2px solid var(--ics-accent);
  outline-offset: 4px;
}


/* =========================================================
   Shared card styles
   ========================================================= */

.ics-page .ics-hover-card {
  position: relative;
  z-index: 0;
  min-width: 0;

  border: 1px solid var(--ics-border);
  background: var(--ics-surface);
  box-shadow: var(--ics-shadow);

  transform: none;

  transition:
    transform 0.22s ease,
    border-color 0.22s ease,
    box-shadow 0.22s ease;
}


/* =========================================================
   Hero section
   ========================================================= */

.ics-page .ics-hero {
  display: grid;
  grid-template-columns: minmax(0, 1fr) minmax(220px, 300px);
  align-items: center;
  gap: 36px;

  margin: 8px 0 40px;
  padding: 32px;

  border-radius: 18px;
}

.ics-page .ics-hero-text {
  min-width: 0;
}

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

.ics-page .ics-hero-title {
  margin: 0 0 8px;
  font-size: clamp(1.7rem, 2.8vw, 2.15rem);
  font-weight: 700;
  line-height: 1.4;
}

.ics-page .ics-hero-subtitle {
  margin: 0 0 16px;
  color: var(--ics-muted);
  font-size: 1.02rem;
  line-height: 1.6;
}

.ics-page .ics-hero-lead {
  margin: 0 0 18px;
  font-size: 1rem;
  line-height: 1.9;
  text-align: left;
}

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
   Hero navigation buttons
   ========================================================= */

.ics-page .ics-hero-actions {
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
  margin-top: 22px;
}

.ics-page .ics-hero-actions .ics-hero-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;

  min-height: 42px;
  padding: 7px 20px;

  border: 1px solid var(--ics-accent);
  border-radius: 8px;

  background: transparent;
  color: var(--ics-accent);

  font-size: 0.94rem;
  font-weight: 700;

  text-decoration: none;
  box-shadow: none;
  cursor: pointer;

  transition:
    background-color 0.2s ease,
    color 0.2s ease,
    box-shadow 0.2s ease;
}


/* =========================================================
   General sections
   ========================================================= */

.ics-page .ics-section {
  margin: 42px 0 0;
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

.ics-page .ics-intro-box {
  padding: 26px 30px;
  border-radius: 15px;
}

.ics-page .ics-intro-box .ics-text:last-child,
.ics-page .ics-section > .ics-text:last-child {
  margin-bottom: 0;
}


/* =========================================================
   ICS core values
   ========================================================= */

.ics-page .ics-values {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 22px;
  margin-top: 24px;
}

.ics-page .ics-value-card {
  padding: 26px 22px;
  border-radius: 15px;
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

.ics-page .ics-value-desc {
  color: var(--ics-muted);
  font-size: 0.94rem;
  line-height: 1.8;
}


/* =========================================================
   Mission and goals
   ========================================================= */

.ics-page .ics-mission {
  margin-bottom: 22px;
  padding: 23px 27px;

  border-left: 4px solid var(--ics-accent);
  border-radius: 0 13px 13px 0;
}

.ics-page .ics-mission-main {
  margin: 0;
  font-size: 1.1rem;
  font-weight: 700;
  line-height: 1.9;
}


/* =========================================================
   Research areas
   ========================================================= */

.ics-page .ics-research-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 18px;
}

.ics-page .ics-research-item {
  padding: 20px 22px;
  border-radius: 12px;
}

.ics-page .ics-research-title {
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
   Collaborator cards
   ========================================================= */

.ics-page .ics-visitor {
  display: grid;
  grid-template-columns: 160px minmax(0, 1fr);
  align-items: center;
  gap: 28px;

  margin-bottom: 24px;
  padding: 24px;

  border-radius: 15px;
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
   Student cards
   ========================================================= */

.ics-page .ics-members {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  align-items: stretch;
  gap: 25px;
}

.ics-page .ics-member-card {
  padding: 24px 20px 0;
  overflow: hidden;
  border-radius: 15px;
  text-align: center;
}

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
   Footer
   ========================================================= */

.ics-page .ics-ending {
  margin: 54px 0 0;
  padding: 28px 15px 8px;

  border-top: 1px solid var(--ics-border);
  text-align: center;
}

.ics-page .ics-ending-en {
  margin-top: 5px;
  color: var(--ics-muted);
}


/* =========================================================
   Hover effects
   ========================================================= */

@media (any-hover: hover) {
  .ics-page .ics-hover-card:hover {
    z-index: 2;
    transform: translateY(-5px);
    border-color: var(--ics-accent);
    box-shadow: var(--ics-hover-shadow);
  }

  .ics-page .ics-hero-actions .ics-hero-button:hover {
    background: var(--ics-accent);
    color: #ffffff;
    border-color: var(--ics-accent);
    box-shadow: 0 5px 14px rgba(0, 0, 0, 0.12);
    text-decoration: none;
  }
}


/* =========================================================
   Tablet layout
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
   Mobile hero layout
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
   Small-screen layout
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
  .ics-page .ics-research-item,
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
   Reduced-motion accessibility
   ========================================================= */

@media (prefers-reduced-motion: reduce) {
  .ics-page .ics-hover-card,
  .ics-page .ics-hero-actions .ics-hero-button {
    transition: none;
  }

  .ics-page .ics-hover-card:hover {
    transform: none;
  }
}

</style>


<div class="ics-page" lang="en">


<!-- =========================================================
     Hero section
     ========================================================= -->

<section
  class="ics-hero ics-hover-card"
  aria-labelledby="ics-hero-title">

  <div class="ics-hero-text">

    <div class="ics-hero-badge">
      ICS Lab
    </div>

    <h2 class="ics-hero-title" id="ics-hero-title">
      Intelligent Cooperative Systems Laboratory
    </h2>

    <p class="ics-hero-subtitle">
      Intelligent Cooperative Systems Laboratory
    </p>

    <p class="ics-hero-lead">
      Centered on intelligent cooperation, we investigate the deep integration
      of communication, sensing, and control, with a focus on future intelligent
      wireless networks and unmanned systems.
    </p>

    <div class="ics-hero-tags" aria-label="Research topics">
      <span class="ics-hero-tag">Integrated Communication, Sensing, and Control</span>
      <span class="ics-hero-tag">Reconfigurable Intelligent Sur
