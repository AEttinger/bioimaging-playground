---
title: "Bioimaging playground"
description: "A (more or less) random collection of scripts and macros."
---
{% assign html_notebooks = site.notebooks %}
{% assign fiji = site.fiji %}
{% assign r = site.r %}

<main role="main" class="container">
  <div class="row">
    <div class="col-sm-10 blog-main">  
      <div class="embed-responsive embed-responsive-16by9">
      <iframe class="embed-responsive-item" src="https://aettinger.github.io/bioimaging-playground/test.html" name="code_frame"><p>Iframe not supported.</p></iframe>
      </div>
    </div>
  <aside class="col-sm-2 ml-sm-auto blog-sidebar">
    <div class="sidebar-module">
      <h4>Jupyter Notebooks</h4>
      <ol class="list-unstyled">
        {% for notebook in html_notebooks %}
          <li><a href="{{ notebook.path }}" target="code_frame">{{ notebook.name | capitalize }}</a></li>
        {% endfor %}
      </ol>
    </div>
    <div class="sidebar-module">
      <h4>Fiji</h4>
      <ol class="list-unstyled">
        {% for item in fiji %}
          <li><a href="{{ item.path }}" target="code_frame">{{ item.name | capitalize }}</a></li>
        {% endfor %}
      </ol>
    </div>
    <div class="sidebar-module">
      <h4>R</h4>
      <ol class="list-unstyled">
        {% for rscript in r %}
          <li><a href="{{ rscript.path }}" target="code_frame">{{ rscript.name | capitalize }}</a></li>
        {% endfor %}
      </ol>
    </div>
    </aside>
  </div>
</main>
