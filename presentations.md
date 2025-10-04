---
layout: page
title: Research
permalink: /research/
---

<style>
  /* --- GRID: fixed columns so rows are consistent --- */
  .page-content .card-list{
    display:grid;
    gap: 1.25rem; /* space between cards */
  }
  /* Desktop: 3 equal columns */
  @media (min-width: 1024px){
    .page-content .card-list{ grid-template-columns: repeat(3, 1fr); }
  }
  /* Tablets: 2 columns */
  @media (min-width: 640px) and (max-width: 1023px){
    .page-content .card-list{ grid-template-columns: repeat(2, 1fr); }
  }
  /* Phones: 1 column */
  @media (max-width: 639px){
    .page-content .card-list{ grid-template-columns: 1fr; }
  }

  /* --- CARD: bigger, uniform height, text over faint bg image --- */
  .page-content .card{
    position: relative;
    overflow: hidden;
    border-radius: 12px;
    padding: 1.25rem;
    min-height: 260px;              /* bump to 300–320 if you want bigger cards */
    background: var(--bg);
    border: 1px solid var(--border);
    display: flex;
    flex-direction: column;
    justify-content: flex-end;
    text-decoration: none;
  }

  /* Background image behind content */
  .page-content .card .card-bg{
    position: absolute; inset: 0;
    width: 100%; height: 100%;
    object-fit: cover;
    opacity: .18;                   /* make .25–.3 if you want it stronger */
    filter: grayscale(100%);
    pointer-events: none;
    z-index: 0;
    border-radius: inherit;
  }

  /* Keep text above background */
  .page-content .card > *:not(.card-bg){ position: relative; z-index: 1; }
  .page-content .card h3{ margin: 0 0 .25rem 0; font-size: 1.125rem; }
  .page-content .card p{ margin: 0; }

  /* Optional: clamp desc to 2 lines for tidy rows */
  .page-content .card p{
    display: -webkit-box;
    -webkit-line-clamp: 2;
    -webkit-box-orient: vertical;
    overflow: hidden;
  }
</style>

{% include card_list.html collection=site.data.home.project_entries %}
