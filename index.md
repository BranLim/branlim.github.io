---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: Software/Quality Engineer & Writer
excerpt: "Passionate about crafting quality software in adherence to Quality standards. Writing fiction/non-fiction when not coding."
header:
    overlay_filter: 0.42    
    overlay_image: /assets/images/unsplash-programming-1.jpg    
    caption: Photo by <a href="https://unsplash.com/@jstrippa?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">James Harrison</a> on <a href="https://unsplash.com/photos/black-laptop-computer-turned-on-on-table-vpOeXr5wmR4?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Unsplash</a>
    tagline: Software/Quality Engineer & Writer
    show_overlay_excerpt: true
layout: splash
intro:
  - title: Who am I? 
    excerpt: "<p>My name is Brandon Lim. I work as a full-stack Software Engineer with a focus on crafting software according to Quality standards. </p> <p>When I'm not coding, I will be writing both non-fiction/fiction content. <br/>And, I am based in Singapore.</p>"
---

{% include feature_row id="intro" type="left" %}

## Latest Posts

{% assign sweCollection = site.collections | where: "label", "swe" %}
{% assign creativeCollection = site.collections | where: "label", "creative_writing" %}
{% assign techCollection = site.collections | where: "label", "tech" %}
{% assign blogCollection = site.collections | where: "label", "blog" %}


{% if blogCollection.size == 0 %}
    No Blog Posts
{% else %}
    {% for post in blogCollection reversed limit:1 %}
        {% include posts_summary_single.html %}
    {% endfor %}
{% endif %}

{% if sweCollection.size == 0 %}
    No Software Engineering Posts
{% else %}
    {% for post in sweCollection reversed limit:1 %}
        {% include posts_summary_single.html %}
    {% endfor %}
{% endif %}

{% if techCollection.size == 0 %}
    No Tech Posts
{% else %}
    {% for post in techCollection reversed limit:1 %}        
        {% include posts_summary_single.html %}        
    {% endfor %}
{% endif %}
