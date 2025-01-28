# Standard names

{% for name, attrs in standardnames.items() %}
## `{{name}}`
- _units_: {{attrs["units"]}}
{% if "tags" in attrs %}
- _tags: {{ ", ".join(attrs["tags"].split()) }}_
{% endif %}

{{ attrs["documentation"] }}
{% endfor %}
