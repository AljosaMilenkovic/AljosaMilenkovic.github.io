---
layout: page
title: Research
permalink: /research/
---

<style>
  /* responsive grid */
  .page-content .card-list{
    display:grid;
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    gap: 1rem;
  }
  /* card shell */
  .page-content .card{
    position:relative; overflow:hidden; border-radius:12px;
    padding:1rem; text-decoration:none;
    background: var(--bg); border: 1px solid var(--border);
    display:block;
  }
  .page-content .card h3{ margin:0 0 .25rem 0; }
  .page-content .card p{ margin:0; }
  /* background image */
  .page-content .card .card-bg{
    position:absolute; inset:0; width:100%; height:100%;
    object-fit:cover; opacity:.18; filter:grayscale(100%);
    pointer-events:none; z-index:0; border-radius:inherit;
  }
  .page-content .card > *:not(.card-bg){ position:relative; z-index:1; }
</style>

{% include card_list.html collection=site.data.home.project_entries %}
