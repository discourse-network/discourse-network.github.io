---
title: Team
permalink: /team/
layout: single
collection: team
entries_layout: list
classes: wide
author_profile: false
---

Here’s our team of digital research leaders:

{% for member in site.team %}
  <div>
    {% if member.profile_image %}
      <img src="{{ member.profile_image }}"
           style="border-radius: 50%;
                  float: left;
                  width: 96px;
                  margin-right: 15px;
                  margin-bottom: 10px;">
    {% endif %}
    <p><strong>
      {% if member.homepage %}
        <a href="{{ member.homepage }}" target="_blank">{{ member.name }}</a>
      {% else %}
        {{ member.name }}
      {% endif %}
    </strong></p>
    <p>{{ member.position }}</p>
    <p>{{ member.affiliation }}</p>
    {% if member.project_role %}
      <p><strong>Role:</strong> {{ member.project_role }}</p>
    {% endif %}
  </div>
  <div style="clear: both;">
    <p>{{ member.content | markdownify }}</p>
  </div>
  <hr>
{% endfor %}
