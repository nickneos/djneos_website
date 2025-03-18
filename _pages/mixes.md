---
title: Mixes by DJ Neos
permalink: /mixes/
read_time: false
---

<div class="entries-{{ entries_layout }}">

    {%- for post in site.posts -%}
        {% if post.tags contains 'mix' %}
            {%- unless post.hidden -%}
                {% include archive-single.html type="list" %}
            {%- endunless -%}
        {% endif %}
    {%- endfor -%}

</div>
