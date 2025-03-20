---
title: Mixes by DJ Neos
permalink: /mixes/code
classes: wide
---

Enjoy some of my mixes below! 🤘

Additional mixes can be found on my [Mixcloud](https://www.mixcloud.com/n3os/) page.

<div class="entries-{{ entries_layout }}">

    {%- for post in site.posts -%}
        {% if post.tags contains 'mix' %}
            {%- unless post.hidden -%}
                {% include archive-single.html type="grid" %}
            {%- endunless -%}
        {% endif %}
    {%- endfor -%}

</div>


<!-- <ul>
    {% for post in site.posts %} 
        {% if post.tags contains "mix" %}
            <li><a href="{{post.url}}">{{ post.title }}</li> 
        {% endif %}
    {% endfor %}
</ul> -->
