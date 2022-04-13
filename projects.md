---
layout: default
title: Projects
---
# Portfolio

<div class="tabsWrapper clear" id="t0">
<ul class="tabs">
    <li>
        <a href="#current-projects">CURRENT PROJECTS</a></li>
    <li>
        <a href="#past-projects">PAST PROJECTS</a></li>
</ul>
</div>

Over the past five years in higher education, museums, and cultural institutions, I have helped produce a variety of projects to deepen public and scholarly engagement with digital materials. This portfolio shares a sampling of my current and past projects, from tools to exhibitions.

<!-- Exhibits -->
<div class="clear">
<h2><span id="t8"></span><a href="#t0"><i class="fa fa-chevron-up"></i></a> Projects</h2>

{% for title in site.data.projects %}
    {% if forloop.first == true %}
        <div class="one-fourth column-bottom clear subcat"><em>Projects</em></div>
    {% else %}
        <div class="one-fourth column-bottom clear subcat"></div>
    {% endif %}
        <div class="three-fourths column-last column-bottom clear">
            <a href="{{ title.url }}"><b>{{ title.title }}</b></a> • <a id="showExhibitions{{ forloop.index }}"><i class="fa fa-info-circle" aria-hidden="true"></i></a> • <small>{{ title.role }}. {{ title.date }}.</small>
            <div class="context" id="minorProject{{ forloop.index }}"><p>{{ title.context }}</p></div>
        </div>
{% endfor %}

</div>
