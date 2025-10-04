---
layout: page
title: Research
permalink: /presentations/
---

{% include card_list.html collection=site.data.home.project_entries %}

<style>
  /* make card backgrounds possible */
  .page-content .card{ position:relative; overflow:hidden; }
  .page-content .card h3,
  .page-content .card p,
  .page-content .card .highlight{ position:relative; z-index:2; }
  .page-content .card .card-bg{
    position:absolute; inset:0;
    width:100%; height:100%;
    object-fit:cover;
    opacity:.15;        /* faint/transparent */
    filter:grayscale(100%);
    pointer-events:none;
    z-index:1; border-radius:inherit;
  }
</style>

