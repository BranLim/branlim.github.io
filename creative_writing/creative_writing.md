---
title: Creative Writing
permalink: /creativewriting/
collection: creative_writing
excerpt: "This is where you will find all my creative works."
---


{% capture written_label %}'None'{% endcapture %}

{% for collection in site.collections %}
    {% unless collection.output == false or collection.label == "posts" %}
        {% capture label %}{{ collection.label }}{% endcapture %}
    {% endunless %}
    {% assign documents = collection.docs | where_exp: "item", "item.category == 'creative_writing'" %}
    {% for post in documents reversed limit:10 %}
        {% unless collection.output == false%}
            {% include archive-single.html %}
        {% endunless %}
    {% endfor %}
{% endfor %}