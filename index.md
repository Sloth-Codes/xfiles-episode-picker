---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: X-files episode picker
permalink: /
---

<p>This is a test.</p>

<div class="entry">
{% for season in site.data.seasons %}
    <h2>{{season.season-num}}</h2>
    <dl>
    {% for episode in season.episodes %}
        <dt>{{episode.title}}</dt>
        <dd>{{episode.description}}</dd>
    {% endfor %}
    </dl>

{% endfor %}
</div>
