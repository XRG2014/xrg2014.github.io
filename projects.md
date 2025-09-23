---
title: Projects
layout: page
description: "My projects"
image: assets/images/pic07.jpg
nav-menu: true
---

<!-- Main -->
<div id="main" class="alt">

<!-- One -->
<section id="one">
	<div class="inner">
		<header class="major">
			<h1>Projects</h1>
		</header>

<!-- Content -->

<table class="table table-element">
  <tr>
    <th class="table-element">Name</th>
	<th class="table-element">Description</th>
	<th class="table-element">Type</th>
    <th class="table-element">Link</th>
  </tr>
  <tr>
	<td class="table-element">Yes for a-Shell</td>
	<td class="table-element" id="repo-desc1">Loading description…</td>
    <td class="table-element">Github repository (Archived)</td>
    <td class="table-element"><a href="https://github.com/SnurfTech/yes-a-shell/">https://github.com/XRG2014/yes-a-shell/</a></td>
  </tr>
  <tr>
    <td class="table-element">Node.js for a-Shell</td>
	<td class="table-element" id="repo-desc2">Loading description…</td>
    <td class="table-element">Github repository (Archived)</td>
    <td class="table-element"><a href="https://github.com/SnurfTech/node.js-a-shell/">https://github.com/XRG2014/node.js-a-shell/</a></td>
  </tr>
</table>

<script>
fetch("https://api.github.com/repos/SnurfTech/yes-a-shell")
  .then(r => r.json())
  .then(data => {
    document.getElementById("repo-desc1").textContent = data.description;
  })
  .catch(() => {
    document.getElementById("repo-desc1").textContent = "Failed to load description.";
  });

fetch("https://api.github.com/repos/SnurfTech/node.js-a-shell")
  .then(r => r.json())
  .then(data => {
    document.getElementById("repo-desc2").textContent = data.description;
  })
  .catch(() => {
    document.getElementById("repo-desc2").textContent = "Failed to load description.";
  });
</script>

</div>
</section>
