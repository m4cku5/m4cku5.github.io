---
layout: page
title: Books / To-Read
permalink: /books/to-read/
---

<p>This is my to-read list. Click <a href="/books">here</a> to see what I've read or <a href="/books/reading">here</a> to see what I'm reading.</p>

<p><i>Note: As an Amazon Associate I earn from qualifying purchases.</i></p>

{% for book in site.books %}
  {% if book.status == 'to-read' %}
  <ul>
    <li>"<a href="{{ book.link }}"><i>{{ book.title }}</i></a>" (#ad) by {{ book.author }}</li>
  </ul>
  {% endif %}
{% endfor %}
