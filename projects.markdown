---
layout: default
title: "Projects"
---
{%- include sort.html -%}

<div class="container-fluid" style="width: 92vw">
	<div class="row">
		<div class="col-lg-2 mt-lg-4">
            {%- include project-categories.html -%}
		</div>
		<div class="col-lg-10 post-content mt-4">
            <div class="row row-cols-1 row-cols-md-2 row-cols-xxl-3 g-4">
                {% for project in project_array %}
                    {%- include project-card.html card-height = '20rem' -%}
                {% endfor %}
            </div>
        </div>
    </div>
</div>
