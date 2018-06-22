---
title: UI-OAPF FAQ
layout: oldstyle
# permalink: /oapf/faq/
---

# Open Access Publishing Fund FAQs

{% assign cats = site.data.UI-OAPF_FAQ | map: "category" | uniq %}
{% for c in cats %}

### {{ c }}

{% assign section = site.data.UI-OAPF_FAQ | where: "category", c %}
{% assign id = forloop.index %}
{% for q in section %}
<div class="panel panel-default">
    <div class="panel-heading">
        <h3 class="panel-title">
            <a data-toggle="collapse" href="#collapse{{ id }}{{ forloop.index }}">{{ q.question }}</a>
        </h3>
    </div>
    <div id="collapse{{ id }}{{ forloop.index }}" class="panel-collapse collapse">
        <div class="panel-body">{{ q.answer }}</div>
    </div>
</div>
{% endfor %}
{% endfor %}

<div class="center">
    <a href="/services/oapf/eligibility.html" class="btn btn-default about-button" type="button"><span class="glyphicon glyphicon-list"></span> Eligibility</a>
    <a href="/services/oapf/apply.html" class="btn btn-default about-button" type="button"><span class="glyphicon glyphicon-ok"></span> Apply</a>
	<a href="mailto:jylisadoney@uidaho.edu" class="btn btn-default about-button" type="button"><span class="glyphicon glyphicon-user"></span> Contact</a>
</div>
<br>

