# Test Project

- created on github direct
- create new file `docs/index.markdown`
- write text
- create new file `docs/_posts/2020-07-06-test.markdown`
- write text
- settings
    - choose source `master branch /docs`
    - choose a theme
    

## Post

~~~~~~~~
---
title: "Test GitPages Post"
date: 2020-07-26 12:48:11 +0100
categories: demo
---

- Add post
~~~~~~~~

Post is at [/gitpagestest/demo/2020/07/26/test](/gitpagestest/demo/2020/07/26/test)

## Add list of posts to the front page

~~~~~~~~
<ul>
{% for post in site.posts %}   
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>
~~~~~~~~

<ul>
{% for post in site.posts %}   
    <li><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>
