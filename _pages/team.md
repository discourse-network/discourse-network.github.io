---
title: DisCouRSE Team
permalink: /team
layout: splash
collection: team
entries_layout: list
classes: wide
author_profile: false
---

<h1>DisCouRSE Project Team</h1>

<section style="margin: 0.5em 0; padding: 0.75em; background-color: #e0e0e0; border-radius: 6px;">
  <h2 style="font-size: 1.2em; margin-top: 0;">Advisory Board</h2>
  <p style="margin: 0.5em 0;">
    The <strong>DisCouRSE Advisory Board</strong> provides independent oversight and strategic guidance to the project.
    <a href="/advisory-board">More information on the Advisory Board is here</a>.
  </p>
</section>


{% assign sorted_team = site.team | sort: "position" %}

{% for project_team_member in sorted_team %}
  <div class="team-member" style="overflow: auto; margin-bottom: 2em;">
    {% if project_team_member.profile_image and project_team_member.profile_image != "" %}
      <img src="{{ site.baseurl }}/assets/images/team/{{ project_team_member.profile_image }}"
    {% else %}
      <img src="{{ site.baseurl }}/assets/images/team/profile_placeholder.png"
    {% endif %}
          style="border-radius: 50%;
                 float: left;
                 width: 96px;
                 margin-right: 15px;
                 margin-bottom: 10px;">
    <p style="font-size: 0.9em; margin-bottom: 0;">
      <strong>
        {% if project_team_member.homepage %}
          <a href="{{ project_team_member.homepage }}" target="_blank" rel="noopener noreferrer">
            {{ project_team_member.name }}
          </a>
        {% else %}
          {{ project_team_member.name }}
        {% endif %}
      </strong>
    </p>
    <p style="font-size: 0.7em; margin-bottom: 0;">{{ project_team_member.affiliation }}</p>
    {% if project_team_member.project_role and project_team_member.project_role != "" %}
      <p style="font-size: 0.7em;"><strong>DisCouRSE Roles: </strong>{{ project_team_member.project_role }}</p>
    {% endif %}
    <div style="font-size: 0.7em; clear: both;">
      <p>{{ project_team_member.content | markdownify }}</p>
    </div>
  </div>
  <hr/>
{% endfor %}
