---
layout: page
title: Books / To-Read
permalink: /books/to-read/
---

<p>This is my to-read list. Click <a href="/books">here</a> to see what I've read or <a href="/books/reading">here</a> to see what I'm reading.</p>

{% for book in site.books %}
  {% if book.status == 'to-read' %}
  <ul>
    <li>"<a href="{{ book.link }}"><i>{{ book.title }}</i></a>" by {{ book.author }}</li>
  </ul>
  {% endif %}
{% endfor %}
