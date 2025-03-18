---
title: Mixes by DJ Neos
permalink: /mixes/
author_profile: true
---

<div class="entries-{{ entries_layout }}">

    {%- for post in site.posts -%}
        {% if post.tags contains 'mix' %}
            {%- unless post.hidden -%}
                {% include archive-single.html type="grid" %}
            {%- endunless -%}
        {% endif %}
    {%- endfor -%}

</div>
