---
layout: mainpage
---


```vb
10 HOME
20 SWEET
30 GOTO 10
```

# Welcome

Thank you for visiting!  Here you will find posts related to my open source projects on GitHub.

<div class="posts">
  {% for post in site.posts %}
    <article class="post">
      <h2><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>

      <div class="entry">
        {{ post.content | strip_html | truncatewords:100 }}
      </div>

      <h4><a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a></h4>
    </article>
  {% endfor %}
</div>

