---
title: Software Engineering
permalink: /swe/
collection: swe
excerpt: "This is where you will discover information related to Software Engineering."
---

{% capture written_label %}'None'{% endcapture %}

{% for collection in site.collections %}
    {% unless collection.output == false or collection.label == "posts" %}
         {% capture label %}{{ collection.label }}{% endcapture %}
    {% endunless %}
    {% assign documents = collection.docs | where_exp: "item", "item.category == 'swe'" %}
    {% for post in documents reversed limit:10 %}
        {% unless collection.output == false %}
           {% include archive-single.html %}
        {% endunless %}
    {% endfor %}
{% endfor %}