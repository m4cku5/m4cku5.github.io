---
layout: page
title: Books / Reading
permalink: /books/reading/
---

<p>This is a list of books that I'm reading (in alphabetical order). Click <a href="/books">here</a> to see what I've read or <a href="/books/to-read">here</a> to see my to-read list.</p>

<p><i>Note: As an Amazon Associate I earn from qualifying purchases.</i></p>

{% for book in site.books %}
  {% if book.status == 'reading' %}
  <ul>
    <li><a href="{{ book.link }}">"<i>{{ book.title }}</i>"</a> by {{ book.author }}</li>
  </ul>
  {% endif %}
{% endfor %}

