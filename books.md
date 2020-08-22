---
layout: page
title: Books
permalink: /books/
---

<p>This is a list of books that I've read (recently), sorted by most recent first. Click <a href="./reading">here</a> to see what I'm currently reading or <a href="./to-read">here</a> to see my to-read list.</p>

{% assign sorted_books = site.books | reverse %}
{% for book in sorted_books %}
  {% if book.status == 'read' %}
  <ul>
    <li><!--<a href="{{ book.link }}">-->"<em>{{ book.title }}</em>"<!--</a>--> by {{ book.author }}</li>
  </ul>
  {% endif %}
{% endfor %}