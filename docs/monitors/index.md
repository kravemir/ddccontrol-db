# Monitors

There's many of monitors supported. Currently, support of following monitors is technically documented:
<ul>
{% assign base_url = '/monitors/' %}
{% for page in site.pages %}
    {% if page.url contains base_url %}
        {% if page.url != base_url %}
            <li><a href='{{page.url}}'>{{page.title}}</a></li>
        {% endif %}
    {% endif %}
{% endfor %}
</ul>
