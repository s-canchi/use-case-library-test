# {{ obj.title }}

<!-- **ID: {{ obj.ident }}** [(permalink)](...) -->
{% if obj.use_cases %}

Use cases that contain this requirement:

{% for uc in obj.use_cases %}
* {{ uc.ident }}: {{ uc.title }}
{% endfor %}

{% endif %}