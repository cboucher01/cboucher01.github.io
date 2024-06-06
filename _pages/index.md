---
layout: page
title: Home
id: home
permalink: /
---

# Welcome!

<p style="padding: 1em 1em; background: #f5f7ff; border-radius: 4px;">
  This site is a work in progress.
</p>

My name is Cameron Boucher. I work as an [[Educational and Scholarly Technology Assistant]] at [[Bryn Mawr College]], where I provide support for educational technology systems and services, [[Digital Scholarship projects]], and Makerspace equipment. I have over 2 years of experience in digital scholarship and web development. I graduated from Bryn Mawr College with an A.B. in Russian and History, and I have a background in communications, film studies, and video editing.

If you're interested in my professional and academic career, take a look at my [[CV]] to get started on your exploration.

I've also written notes about my other [[hobbies]] and [[interests]], so feel free to explore!

<strong>Recently updated notes</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
