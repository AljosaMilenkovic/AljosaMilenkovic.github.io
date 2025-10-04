---
layout: page
title: Research
permalink: /research/
---

<style>
  /* background image support for Moonwalk cards */
  .page-content .entry,
  .page-content .entries a,
  .page-content .card {
    position: relative;
    overflow: hidden;
    border-radius: 12px;
  }
  .page-content img.card-bg {
    position: absolute; inset: 0;
    width: 100%; height: 100%;
    object-fit: cover;
    opacity: .18;
    filter: grayscale(100%);
    pointer-events: none;
    z-index: 0;
  }
  .page-content .entry h3, .page-content .entry p,
  .page-content .entries a h3, .page-content .entries a p,
  .page-content .card h3, .page-content .card p {
    position: relative; z-index: 1;
  }
</style>

{% include card_list.html collection=site.data.home.project_entries %}
