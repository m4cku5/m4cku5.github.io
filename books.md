---
layout: page
title: Books
permalink: /books
---

<p>This is a list of books that I've read:</p>

{% assign sorted_books = site.books_read | reverse %}
{% for book in sorted_books %}
  <ul>
    <li>"<i>{{ book.title }}</i>" by {{ book.author }}</li>
  </ul>
{% endfor %}

Click <a href="">here</a> to see what I'm currently reading or <a href="">here</a> to see my to-read list.