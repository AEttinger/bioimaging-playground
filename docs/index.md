---
title: "Bioimaging playground"
description: "A (more or less) random collection of scripts and macros."
---
{% assign html_notebooks = site.html_pages %}

<main role="main" class="container">
  <div class="row">
    <div class="col-sm-8 blog-main">  
      <div class="embed-responsive">
      <iframe class="embed-responsive-item" src="" id="notebook"></iframe>
      </div>
    </div>
  <aside class="col-sm-3 ml-sm-auto blog-sidebar">
    <div class="sidebar-module">
      <h4>Jupyter Notebooks</h4>
      <ol class="list-unstyled">
        {% for item in html_notebooks %}
          <li><a href="{{ item.path }}" target="notebook">{{item.name | capitalize }}</a></li>
        {% endfor %}
      </ol>
    </div>
    </aside>
  </div>
</main>
