---
layout: page
title: Books / To-Read
permalink: books_to-read
---

<p>This is my to-read list. Click <a href="./books">here</a> to see what I've read or <a href="./books_reading">here</a> to see what I'm reading.</p>

{% assign sorted_books = site.books_to-read | reverse %}
{% for book in sorted_books %}
  <ul>
    <li>"<i>{{ book.title }}</i>" by {{ book.author }}</li>
  </ul>
{% endfor %}
