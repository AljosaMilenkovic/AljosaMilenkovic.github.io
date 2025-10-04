---
layout: page
title: Research
permalink: /presentations/
---

<div class="card-grid">
{% raw %}{% for item in site.data.home.project_entries %}{% endraw %}
  <a class="card" href="{{ item.url | relative_url }}">
    <h3>{{ item.title }}</h3>
    <p>{{ item.desc }}</p>
    {% raw %}{% if item.highlight %}<span class="highlight">{{ item.highlight }}</span>{% endif %}{% endraw %}
  </a>
{% raw %}{% endfor %}{% endraw %}
</div>
