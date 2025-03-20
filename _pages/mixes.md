---
title: Mixes by DJ Neos
permalink: /mixes/
---

Enjoy some of my mixes below!

For more mixes, checkout my [Mixcloud](https://www.mixcloud.com/n3os/) as well!

<!-- <div class="entries-{{ entries_layout }}">

    {%- for post in site.posts -%}
        {% if post.tags contains 'mix' %}
            {%- unless post.hidden -%}
                {% include archive-single.html type="list" %}
            {%- endunless -%}
        {% endif %}
    {%- endfor -%}

</div> -->
<ul>
    {% for post in site.posts %} 
        {% if post.tags contains "mix" %}
            <li><a href="{{post.url}}">{{ post.title }}</li> 
        {% endif %}
    {% endfor %}
</ul>