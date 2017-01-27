---
layout: page
title: Archive
permalink: /archive/
---
Here's a list of all my posts. I'm a firm believer in owning your own online space so I only write on my own blog. If you would like to talk about a certain post, contact me on <a href="https://twitter.com/ndrwpw0">Twitter</a> or <a href="mailto:ndrwpw0@gmail.com">email</a>.

<ul class="">
    {% for post in site.categories.blog %}
    {% if post.external-url %}
    <li class="pt3">
        <a href="{{ post.external-url }}">{{ post.title }}</a>
        <time class="">{{ post.date | date: '%B %d, %Y' }}</time>
    </li>
    {% else %}
    <li class="pt3">
        <a href="{{ post.url }}">{{ post.title }}</a>
        <time class="">{{ post.date | date: '%B %d, %Y' }}</time>
    </li>
    {% endif %}
    {% endfor %}
</ul>
