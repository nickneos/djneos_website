---
permalink: /contact/
title: "Get in Touch"
classes: wide
---

Use the below form or email [contact@djneos.com.au](mailto:contact@djneos.com.au)

For booking enquiries, please include venue, date and number of guests in your message if you have these details.

<form
  class="fs-form"
  target="_top"
  name="contact"
  method="POST"
  data-netlify="true"
  action="/thanks/"
  netlify-honeypot="gotcha"
>
  <input type="hidden" name="subject" value="[www.djneos.com.au] Contact Request (23%{submissionId})">
  <div class="fs-field">
    <label class="fs-label" for="name">Your Name</label>
    <input class="fs-input" type="text" id="name" name="name" required />
  </div>
  <div class="fs-field">
    <label class="fs-label" for="email">Email</label>
    <input class="fs-input" type="email" id="email" name="email" required />
  </div>
  <div class="fs-field">
    <label class="fs-label" for="message">Message</label>
    <textarea
      class="fs-textarea"
      id="message"
      name="message"
      required
    ></textarea>
  </div>
  <input type="text" name="gotcha" style="display:none" />
  <div class="fs-button-group">
    <button class="fs-button" type="submit">Submit</button>
  </div>
</form>
