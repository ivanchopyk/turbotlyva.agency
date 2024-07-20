---
layout: page
title: Home
id: home
permalink: /
---

# Доброго дня! 🌱

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
  <b>Ми — агенція турботливих нянь. Працюємо у Львові для батьків та їхніх діток.</b> 
  
  Наша агенція — не лише про дітей та піклування за ними. Ми також турбуємось й про батьків, про їхній час. Зараз, під час відключень світла, батькам особливо важко справлятися з усіма хатніми обов’язками та доглядом за дітьми. Тому ми готові допомогти у складні моменти і зайняти наших маленьких клієнтів цікавими заняттями.
  
  Більше про нас можна почитати тут. 
  
  Take a look at <span style="font-style:italic; font-weight: bold">[[Your first note]]</span> to get started on your exploration.
</p>

This digital garden template is free, open-source, and [available on GitHub here](https://github.com/maximevaillancourt/digital-garden-jekyll-template).

The easiest way to get started is to read this [step-by-step guide explaining how to set this up from scratch](https://maximevaillancourt.com/blog/setting-up-your-own-digital-garden-with-jekyll).

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
