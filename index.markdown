---
layout: default
title: 2late2nate
---
<h2>Blog</h2>
Welcome to my website. I'll be hosting all of my **blogposts** and **professional work** here. Enjoy your stay.

This website is a **Work-In-Progress**, so bear with me if some pages are unavailable.

---

Click on the title of a blogpost in order to view it.

<ul class="posts">
{% for post in site.posts %}
    <li>
        <section>
            <h2><a href="{{ post.url }}">{{ post.date | date_to_string | downcase }}: {{ post.title }}</a></h2>
            {{ post.excerpt }}
        </section>
    </li>
{% endfor %}
</ul>