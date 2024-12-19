---
layout: page
title: Archive
permalink: /archive
---

# Notes Archive

Here are my DIGM 5010 notes, sorted in chronological order from the date they were first created.

<ul>
  {% assign recent_notes = site.notes | sort: 'created' %}
  {% for note in recent_notes limit: 100 %}
    <li>
      Created {{ note.created | date: "%b %d, %Y" }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>