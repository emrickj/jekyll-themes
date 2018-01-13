---
---
| Name | Description | CSS Framework | Actions |
| --- | --- | --- | --- |
{% for item in site.website_theme %} | {{ item.name | prepend: "theme" }} | {{ item.desc }} | {{ item.cssf }} | <a class="action" title="Download" href="{{ item.name | prepend: "theme" }}.php"><span class="download"></span></a> {% if item.pwfn != nil %} <a class="action" title="Preview" href="{{ site.preview_path | append: item.name }}.php?u={{ item.pwfn }}" target="_blank"><span class="preview"></span></a> {% endif %} |
{% endfor %}
