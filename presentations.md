---
layout: page
title: Research
permalink: /presentations/
---
<style>
  .page-content .card, .page-content .entry { position:relative; overflow:hidden; }
  .page-content .card h3, .page-content .card p, .page-content .card .highlight,
  .page-content .entry h3, .page-content .entry p, .page-content .entry .highlight { position:relative; z-index:2; }
  .page-content .card .card-bg, .page-content .entry .card-bg{
    position:absolute; inset:0; width:100%; height:100%;
    object-fit:cover; opacity:.15; filter:grayscale(100%);
    pointer-events:none; z-index:1; border-radius:inherit;
  }
</style>

{% include card_list.html collection=site.data.home.project_entries %}
