---
layout: page
title: Home
id: home
permalink: /
---

# Welcome to my Digital Garden &#127793;

Here are my DIGM 5010 notes, sorted from least to most recently updated. For a list of notes in chronological order, check out the [Notes Archive](/archive).

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 20 %}
    <li>
      Updated {{ note.last_modified_at | date: "%b %d, %Y" }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
