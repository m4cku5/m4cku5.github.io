---
layout: page
title: Books
permalink: /books/
---

<p>This is a list of books that I've read (recently), sorted by most recent first. Several years of my Org-Mode reading list are trapped on a dead phone, so I'll eventually post those if I'm able to recovery it. Click <a href="./reading">here</a> to see what I'm currently reading or <a href="./to-read">here</a> to see my to-read list.</p>

<p><em>Note: As an Amazon Associate I earn from qualifying purchases.</em></p>

{% assign sorted_books = site.books | reverse %}
{% for book in sorted_books %}
  {% if book.status == 'read' %}
  <ul>
    <li><a href="{{ book.link }}">"<em>{{ book.title }}</em>"</a> by {{ book.author }}</li>
  </ul>
  {% endif %}
{% endfor %}