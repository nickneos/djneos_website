---
title: Mixes by DJ Neos
permalink: /mixes/
# classes: wide
layout: splash
# header:
#   image: /assets/images/dj_neos_banner_crop_2.jpg
---

Hear the range! My mixes below cover a vibrant spectrum of genres, from classic throwbacks to modern beats. Find your perfect groove and discover the sounds I love to spin. 🤘🔊

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
