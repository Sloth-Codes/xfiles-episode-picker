# X-files episode generator

This is a test.

<ul>
{% for episode in site.data.episodes %}
    <li>
        {{episode.title}}
    </li>
{% endfor %}
</ul>