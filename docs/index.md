---
title: "Bioimaging playground"
description: "A (more or less) random collection of scripts and macros."
---
{% assign html_notebooks = site.pages %}
{% for item in html_notebooks %}
<p>item.url</p>
<div class="embed-responsive">
  <iframe class="embed-responsive-item" source="{{ item.url | prepend: site.baseurl }}"></iframe>
</div>
{% endfor %}
