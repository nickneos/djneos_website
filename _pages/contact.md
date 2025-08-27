---
permalink: /contact/
title: "Get in Touch"
header:
  overlay_image: /assets/images/dj_neos_banner_2.jpg
  overlay_filter: 0.3
  overlay_padding: 12.5em 0 1em
page_css:
  - /assets/css/contact_form.css
---
Shoot me a message via the form below or email [contact@djneos.com.au](mailto:contact@djneos.com.au)

Prefer to chat on the phone old school? [0468&nbsp;689&nbsp;700](tel:+61468689700)

*For booking enquiries, please include venue, date and number of guests in your message if you have these details.*

<form
  class="fs-form"
  target="_top"
  name="contact"
  method="POST"
  data-netlify="true"
  action="/contact/sent/"
  netlify-honeypot="gotcha"
  style="border-radius: 0.75rem"
>
  <input type="hidden" name="subject" value="[DJ Neos] Contact Request (Ref: 3%{submissionId})">
  <div class="fs-field">
    <label class="fs-label" for="name">Your Name</label>
    <input class="fs-input" type="text" id="name" name="name" required />
  </div>
  <div class="fs-field">
    <label class="fs-label" for="email">Your Email</label>
    <input class="fs-input" type="email" id="email" name="email" required />
  </div>
  <div class="fs-field">
    <label class="fs-label" for="message">Message</label>
    <textarea class="fs-textarea" id="message" name="message" rows="10" required></textarea>
  </div>
  <input type="text" name="gotcha" style="display:none" />
  <div class="fs-button-group">
    <button class="fs-button" type="submit">Submit</button>
  </div>
</form>
