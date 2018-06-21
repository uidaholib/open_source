---
title: UI-OAPF FAQ
layout: oldstyle
# permalink: /oapf/faq/
---

# Open Access Publishing Fund FAQs

{% for q in site.data.ui-oapf_faq %}
<div class="panel panel-default">
    <div class="panel-heading">
        <h3 class="panel-title">
            <a data-toggle="collapse" href="#collapse{{ forloop.index }}">{{ q.question }}</a>
        </h3>
    </div>
    <div id="collapse{{ forloop.index }}" class="panel-collapse collapse">
        <div class="panel-body">{{ q.answer }}</div>
    </div>
</div>
{% endfor %}
