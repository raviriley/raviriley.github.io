---
title: Projects
permalink: /projects/
classes: wide
sidebar: 
  nav: "projects"
author_profile: true
---
<!-- adapted from http://www.menucool.com/ui/responsive-image-grid-with-hover-effect -->
<ul id="rig">
	{% if site.animated-gallery.links %}
      {% for link in site.animated-gallery.links %}
        {% if link.label and link.url %}
          <li><a class="rig-cell" href="{{ link.url }}"><img class="rig-img" src="{{ link.image }}"><span class="rig-overlay"></span><span class="rig-text">{{ link.label | markdownify }}</span></a></li>
        {% endif %}
      {% endfor %}
    {% endif %}
</ul>

<!-- turn this into something in _includes to later add to the theme - learn from gallery and feature row, mainly gallery -->