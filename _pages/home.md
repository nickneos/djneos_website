---
title: DJ Neos
layout: splash
permalink: /
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/splash_img.jpg
  actions:
    - label: "Book Now"
      url: "/contact/"
feature_row:
  - image_path: /assets/images/feature_3.jpg
    alt: "about"
    # title: "About Me"
    # excerpt: "Everything from the menus, sidebars, comments, and more can be configured or set with YAML Front Matter."
    url: "/about/"
    btn_label: "About Me"
    btn_class: "btn--primary"
feature_row_2:
  - image_path: /assets/images/feature_1.jpg
    alt: "Mixes"
    url: "/mixes/"
    excerpt: "Listen to some of my mixes!"
    btn_label: "My Mixes"
    btn_class: "btn--primary"
feature_row_3:
  - image_path: /assets/images/feature_4.jpg
    alt: "contact"
    url: "/contact/"
    excerpt: "Get in touch for any enquries or bookings!"
    btn_label: "Contact Me"
    btn_class: "btn--primary"
---




{% include feature_row id="feature_row_1" type="left" %}

{% include feature_row id="feature_row_2" type="right" %}

{% include feature_row id="feature_row_3" type="left" %}

{% include video id="5yUA1EV0SS8" provider="youtube" %}
