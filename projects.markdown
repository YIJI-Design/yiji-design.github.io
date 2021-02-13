---
layout: default
title: "Projects"
---

<div class="container-fluid" style="width: 92vw">
	<div class="row">
		<div class="col-lg-2 mt-lg-4">
            {%- include project-categories.html -%}
		</div>
		<div class="col-lg-10 post-content mt-4">
            <div class="row row-cols-1 row-cols-md-2 row-cols-xxl-3 g-4">
            </div>
        </div>
            {% for project in site.projects %}
                {% if project.category == category %}
                    {%- include project-card.html -%}
                {% endif %}
            {% endfor %}
    </div>
</div>
