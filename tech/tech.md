---
title: Tech
permalink: /tech/
collection: tech
excerpt: "This is where you will find all Tech-related articles and essays."
---


{% capture written_label %}'None'{% endcapture %}

{% for collection in site.collections %}
    {% unless collection.output == false or collection.label == "posts" %}
        {% capture label %}{{ collection.label }}{% endcapture %}
    {% endunless %}
    {% assign documents = collection.docs | where_exp: "item", "item.category == 'tech'" %}
    {% for post in documents reversed limit:10 %}
        {% unless collection.output == false%}
            {% include archive-single.html %}
        {% endunless %}
    {% endfor %}
{% endfor %}