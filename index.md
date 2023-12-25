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

<br/>

# Latest Posts

{% for collection in site.collections %}
    {% unless collection.output == false %}
        {% assign blogDocuments = collection.docs | where_exp: "item", "item.category == 'blog'" %}
        {% assign techDocuments = collection.docs | where_exp: "item", "item.category == 'tech'" %}
        {% assign sweDocuments = collection.docs | where_exp: "item", "item.category == 'swe'" %}
        {% assign creativeDocuments = collection.docs | where_exp: "item", "item.category == 'creative_writing'" %}

        {% for post in blogDocuments reversed limit:1 %}
            {% include posts_summary_single.html category='Blog' %}
        {% endfor %}

         {% for post in techDocuments reversed limit:1 %}
            {% include posts_summary_single.html category='Tech' %}
        {% endfor %}

        {% for post in sweDocuments reversed limit:1 %}
            {% include posts_summary_single.html category='Software Engineering' %}
        {% endfor %}
        
        {% for post in creativeDocuments reversed limit:1 %}
            {% include posts_summary_single.html category='Creative Writing' %}
        {% endfor %}
    {% endunless %}
{% endfor %}
