---
layout: page
title: Books / Reading
permalink: books_reading
exclude: true
---

<p>This is a list of books that I'm reading. Click <a href="./books">here</a> to see what I've read or <a href="">here</a> to see my to-read list.</p>

{% assign sorted_books = site.books_reading | reverse %}
{% for book in sorted_books %}
  <ul>
    <li>"<i>{{ book.title }}</i>" by {{ book.author }}</li>
  </ul>
{% endfor %}
