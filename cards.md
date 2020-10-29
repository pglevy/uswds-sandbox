---
title: Cards
layout: default
---

<h6 class="padding-bottom-2">Standard Layout</h6>
<ul class="usa-card-group">
{% for item in site.data.cards %}
  <li class="tablet:grid-col-4 usa-card">
    <div class="usa-card__container">
      <header class="usa-card__header">
        <h2 class="usa-card__heading">{{ item.title }}</h2>
      </header>
      <div class="usa-card__body">
        <p>{{ item.body }}</p>
      </div>
      <div class="usa-card__footer">
        <button class="usa-button">{{ item.CTA }}</button>
      </div>
    </div>
  </li>
  {% endfor %}
</ul>