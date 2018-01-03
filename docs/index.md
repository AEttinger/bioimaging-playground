---
title: "Bioimaging playground"
description: "A (more or less) random collection of scripts and macros."
---

{% assign notebooks = site.static_files %}
{% for note in notebooks %}
  {{ note.path }}
{% endfor %}
