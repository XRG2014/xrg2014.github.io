---
layout: page
title: Desmos Art
description: My Desmos graphing calculator art
image: assets/images/desmos.jpg
nav-menu: true
---

<!-- Main -->
<div id="main" class="alt">

<!-- One -->
<section id="one">
	<div class="inner">
		<header class="major">
			<h1>Desmos Art</h1>
		</header>

<!-- Content -->
{% assign files = site.static_files | where: "path", "/_includes/desmos" %}
{% for file in files %}
  {% include html_snippets/{{ file.name }} %}
{% endfor %}
</div>
</section>
