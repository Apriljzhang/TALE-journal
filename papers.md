---
title: Papers
---

# Papers

Below are published and forthcoming papers. Add or update entries in `_data/papers.yml` to keep this page current.

<ul class="papers-list">
  {% for paper in site.data.papers %}
    <li class="card-soft">
      <strong>{{ paper.title }}</strong><br />
      <span class="meta">{{ paper.authors }} · {{ paper.year }}</span><br />
      {% if paper.pdf_url and paper.pdf_url != "" %}
        <a href="{{ paper.pdf_url }}">Read PDF</a>
      {% else %}
        <span class="meta">PDF link coming soon</span>
      {% endif %}
    </li>
  {% endfor %}
</ul>
