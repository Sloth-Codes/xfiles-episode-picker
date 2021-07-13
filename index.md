---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: X-files episode picker
permalink: /
season: 0
---

<p>This is a test.</p>

<div class="entry">
    
    {% for episode in site.data.episodes %}
        {% if episode.Season != season %}
            <h2>{{episode.Season}}</h2>
            {% assign season = episode.Season %}
        {% endif %}
        
        <p>{{episode.EpisodeTitle}}</p>
        <p>{{episode.AirOrderInSeason}}</p>
    {% endfor %}
    
</div>
