---
layout: default
title: Future ESS events
order: 1

---


# Events

We'll list forthcoming events here.

<ul class="posts">
{% assign curDate = site.time | date: '%s' %}
{% for post in site.posts %}
    {% assign postStartDate = post.date | date: '%s' %}
    {% if postStartDate >= curDate %}
    <li>
    <a href="{{ post.url }}">{{post.date | date_to_string}} {{ post.title }}</a>
    <p>
    {{ post.excerpt | remove: '<p>' | remove: '</p>' }}</p>
    </li>

    {% endif %}
{% endfor %}


</ul>
