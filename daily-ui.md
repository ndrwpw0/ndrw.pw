---
layout: page
title: Daily UI
permalink: /daily-ui/
---
This page lists all the <a href="http://dailyui.co/">Daily UI</a> projects I've completed. These are all visual and development comps only. There are no production projects here but I've enjoyed designing and coding all of these.

<div class="post-list">
    <ul>
      {% for post in site.categories.daily-ui %}
        {% if post.url %}
            <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                <time>{{ post.date | date: '%B %d, %Y' }}</time>
            </li>
        {% endif %}
      {% endfor %}
    </ul>
</div>