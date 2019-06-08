---
layout: page
title: Books
permalink: /books
---

<p>This is a list of books that I've read (sorted by most recent first). Click <a href="./books_reading">here</a> to see what I'm currently reading or <a href="./books_to-read">here</a> to see my to-read list.
</p>

{% assign sorted_books = site.books_read | reverse %}
{% for book in sorted_books %}
  <ul>
    <li>"<i>{{ book.title }}</i>" by {{ book.author }}</li>
  </ul>
{% endfor %}