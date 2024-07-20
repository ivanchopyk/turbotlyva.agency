---
layout: page
title: Про нас
permalink: /about
---

<img src="{{ site.baseurl }}/assets/IMG_1781.JPG"
	width="500" 
	radius="50%" />

## Привіт, мене звати Аня!

Моє життя тісно пов’язане з дітьми і я вирішила цей досвід втілити у щось більше, тому  створила Турботливу Агенцію Нянь.
  
Здобуваючи вищу педагогічну освіту, я мала великий досвід практики з дітьми вже з 2-го курсу. А на 3-му курсі мене запросили працювати у дитячий садок в невеликому місті.

Там я пропрацювала 2 роки, але дуже мріяла переїхати до Львова. А з переїздом змінився і мій вид діяльності — я стала нянею. 

Після 5-ти років роботи нянею я відчула, що моя місія — не тільки виховувати маленьких класних особистостей. Я також бажаю передати свій прекрасний та позитивний досвід іншим дівчатам, які люблять дітей і хочуть працювати з ними.

Водночас, моя Агенція не лише про дітей та нянь. Вона — про Вас, батьки, і про Ваш чаc. Час на відпочинок, на своє хоббі, на роботу та самореалізацію. Та й зрештою, на будь-що, що Вам потрібно!

І ми готові вам цей час подарувати ☀️


<div id="image">
    <side>
      <img src="{{ site.baseurl }}/assets/IMG_1781.JPG" />
      <div style="display: grid; grid-gap: 1em; grid-template-columns: repeat(1fr);">
      {% for backlink in page.backlinks %}
        <div class="backlink-box">
        <a class="internal-link" href="{{ site.baseurl }}{{ backlink.url }}{%- if site.use_html_extension -%}.html{%- endif -%}">{{ backlink.title }}</a><br>
        <div style="font-size: 0.9em">{{ backlink.excerpt | strip_html | truncatewords: 20 }}</div>
        </div>
      {% endfor %}
      </div>
      {% else %}
      <div style="font-size: 0.9em">
        <p>
          There are no notes linking to this note.
        </p>
      </div>
      {% endif %}
    </side>
  </div>