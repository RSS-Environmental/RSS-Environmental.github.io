---
layout: default
title: Past events
order: 3
---

# Past events organised by the ESS


<ul class="posts">
{% assign curDate = site.time | date: '%s' %}

{% for post in site.posts %}
    {% if post.categories contains 'events' %}
    {% assign postStartDate = post.date | date: '%s' %}
    {% if postStartDate <= curDate %}
        <li>
        <a href="{{ post.url }}">{{post.date | date_to_string}} {{ post.title }}</a>
        <p>
        {{ post.excerpt | remove: '<p>' | remove: '</p>' }}</p>
        </li>
        {% endif %}        
    {% endif %}
{% endfor %}
</ul>
