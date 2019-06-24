---
layout: default
title: Committee
order: 4

---


# Current committee



<ul>
{% for member in site.data.members %}
  <li>
  {% if member.officer%}
  {{member.role}}:
  {% endif %}
    <a href="https://github.com/{{ member.github }}">
      {{ member.name }} <!--({{member.university}})-->
    </a>
  </li>
{% endfor %}
</ul>

If you have an idea for a meeting on some aspect of statistics and the environment, please contact one of the committee members listed above.


# Joining the ESS committee

Committee membership runs for a calendar year, and members can serve for a maximum of four consecutive years (excluding years as officer).
If you would like to join the ESS committee please contact one of the officers.

