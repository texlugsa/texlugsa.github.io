---
layout: default
title: Building Standards
---

<div class="accordion" id="standardsAccordion">
    {% for standard in site.building_standards %}
    <div class="accordion-item">
        <h2 class="accordion-header" id="heading{{ forloop.index }}">
            <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapse{{ forloop.index }}" aria-expanded="true" aria-controls="collapse{{ forloop.index }}">
                {{ standard.title }}
            </button>
        </h2>
        <div id="collapse{{ forloop.index }}" class="accordion-collapse collapse" aria-labelledby="heading{{ forloop.index }}" data-bs-parent="#standardsAccordion">
            <div class="accordion-body">
              {{ standard.content }}
            </div>
        </div>
    </div>
    {% endfor %}
</div>
