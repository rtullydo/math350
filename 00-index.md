---
layout: page
title: "Math 350"
permalink: "index.html"
---



This is the public support page for a mathematical programming course, taught this quarter in Mathematica by [Ryan Tully-Doyle](https://rtullydo.github.io). As the course proceeds, I'll be posting lecture notes and exercises here, in the form of Mathematica .nb files. The course is taught in Mathematica 12. The associated textbook for the course is _Mathematica: A Problem Solving Approach_ by Roozbeh Hazrat (2010 edition), which is [available on SpringerLink](https://link.springer.com/book/10.1007/978-1-84996-251-3) for those with institutional access. 

The lectures are hosted on YouTube, located here: [RTD Math](https://www.youtube.com/playlist?list=PLd-yyEHYtIhKhXrzklfwupcbfe_LCcfoV).

  {% for post in site.posts %}
  <article>
    <h2>
      <a href="/math350/{{ post.url }}">
        {{ post.title }}
      </a>
    </h2>
    <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
    {{ post.content }}
  </article>
{% endfor %}
