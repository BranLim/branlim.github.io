---
title: Blog
permalink: /blog/
collection: blog
excerpt: "This is where you will find my opinions, thoughts and any other random stuff I can think of."
header:
    overlay_color: "#000"
    overlay_filter: 0.55
    overlay_image: /assets/images/jeju-wind-turbines.jpeg
    show_overlay_excerpt: true
---


{% capture written_label %}'None'{% endcapture %}

{% for collection in site.collections %}
    {% unless collection.output == false or collection.label == "posts" %}
        {% capture label %}{{ collection.label }}{% endcapture %}
    {% endunless %}
    {% assign documents = collection.docs | where_exp: "item", "item.category == 'blog'" %}
    {% for post in documents reversed limit:10 %}
        {% unless collection.output == false %}
            {% include archive-single.html %}
        {% endunless %}
    {% endfor %}
{% endfor %}