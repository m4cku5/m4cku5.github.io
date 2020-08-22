---
layout: page
title: Books / Reading
permalink: /books/reading/
---

<p>This is a list of books that I'm reading (in alphabetical order). Click <a href="/books">here</a> to see what I've read or <a href="/books/to-read">here</a> to see my to-read list.</p>

{% for book in site.books %}
  {% if book.status == 'reading' %}
  <ul>
    <li><!--<a href="{{ book.link }}">-->"<em>{{ book.title }}</em>"<!--</a>--> by {{ book.author }}</li>
  </ul>
  {% endif %}
{% endfor %}

