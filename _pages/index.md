---
layout: page
title: Home
id: home
permalink: /
---

# Welcome to the Digital Bike Kitchen!

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">

This page is like a bike kitchen but digital, a digital-free space. It is a [[common garden]], that we all build and maintain together, you can change and add to it make it your own. 

This page will aggregate and formulate a knowledge base on [[bike repair]] and [[maintenance]], building [[Bike Kitchens]], [[horizontal education]]. 
    

</p>



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
