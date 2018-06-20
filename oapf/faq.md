---
title: UI-OAPF FAQ
layout: faq
permalink: /oapf/faq/
---


{% for q in site.data.ui-oapf_faq %}
<div class="panel panel-default">
    <div class="panel-heading">
        <h3 class="panel-title">{{ q.question }}</h3>
    </div>
    <div class="panel-body">
        {{ q.answer }}
    </div>
</div>
{% endfor %}

