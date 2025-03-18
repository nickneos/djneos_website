---
title: DJ Mixes
permalink: /mixes/
author_profile: true
---

## Mixes By DJ Neos

{% assign entries_layout = page.entries_layout | default: 'list' %}
<div class="entries-{{ entries_layout }}">

    {%- for post in site.posts -%}
        {% if post.tags contains 'mix' %}
            {%- unless post.hidden -%}
                {% include archive-single.html type="grid" %}
            {%- endunless -%}
        {% endif %}
    {%- endfor -%}

</div>
