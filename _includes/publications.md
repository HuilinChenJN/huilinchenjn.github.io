<h2 id="publications">Selected Publications</h2>
<div class="publications">
<ol class="bibliography">
{% for paper in site.data.publications.main %}
<li class="paper-entry{% if paper.image %} has-figure{% endif %}">
{% if paper.image %}
<a class="paper-figure" href="{{ paper.image }}" aria-label="View framework for {{ paper.title | escape }}">
<img src="{{ paper.image }}" alt="Framework of {{ paper.title | escape }}" loading="lazy">
{% if paper.conference_short %}<span class="paper-venue">{{ paper.conference_short }}</span>{% endif %}
</a>
{% endif %}
<div class="paper-details">
<div class="title">{% if paper.page or paper.code %}<a href="{{ paper.page | default: paper.code }}">{{ paper.title }}</a>{% else %}{{ paper.title }}{% endif %}</div>
{% if paper.authors %}<div class="author">{{ paper.authors }}</div>{% endif %}
<div class="periodical"><em>{{ paper.conference }}</em></div>
<div class="links">
{% if paper.pdf %}<a href="{{ paper.pdf }}" class="btn btn-sm z-depth-0">PDF</a>{% endif %}
{% if paper.page %}<a href="{{ paper.page }}" class="btn btn-sm z-depth-0">Paper</a>{% endif %}
{% if paper.code %}<a href="{{ paper.code }}" class="btn btn-sm z-depth-0">Code</a>{% endif %}
{% if paper.notes %}<span class="paper-note">{{ paper.notes }}</span>{% endif %}
</div>
</div>
</li>
{% endfor %}
</ol>
</div>
