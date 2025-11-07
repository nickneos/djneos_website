---
permalink: /contact/
title: "Get in Touch"
header:
  overlay_image: /assets/images/dj_neos_banner.jpg
  overlay_filter: 0.3
  overlay_padding: 16em 0 1em
page_css:
  - /assets/css/contact_form.css
---
For booking enquiries please use the form below or shoot an email to [contact@djneos.com.au](mailto:contact@djneos.com.au)

Prefer to chat on the phone old school? [0468&nbsp;689&nbsp;700](tel:+61468689700)

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
    <label class="fs-label" for="name">Name</label>
    <input class="fs-input" type="text" id="name" name="name" placeholder="Your name" required />
  </div>
  
  <div class="fs-field">
    <label class="fs-label" for="email">Email</label>
    <input class="fs-input" type="email" id="email" name="email" placeholder="Your email" required />
  </div>

  <div class="fs-field">
    <label class="fs-label" for="eventType">Event Type</label>
    <select class="fs-select" id="eventType" name="eventType" required>
      <option value="" disabled selected>Please Select...</option>
      <option value="wedding">Wedding</option>
      <option value="engagement">Engagement Party</option>
      <option value="brithday">Birthday Party</option>
      <option value="kids">Kids Party</option>
      <option value="corporate">Corporate Function</option>
      <option value="other">Other (provide further details in message)</option>
    </select>
  </div>

  <div class="fs-field">
    <label class="fs-label" for="location">Event Location</label>
    <input class="fs-input" type="text" id="location" name="location" placeholder="Venue name / Suburb" required />
  </div>

  <div class="fs-field">
    <label class="fs-label" for="eventDate">Event Date</label>
    <input class="fs-input" type="date" id="eventDate" name="eventDate" required />
  </div>

  <div class="fs-field">
    <label class="fs-label" for="startTime">Event Time</label>
    <input class="fs-input" type="text" id="startTime" name="startTime" placeholder="Include start and end time of event" required />
  </div>

  <div class="fs-field">
    <label class="fs-label" for="duration">Duration</label>
    <input class="fs-input" type="text" id="duration" name="duration" placeholder="Number of hours DJ required for" required />
  </div>

  <div class="fs-field">
    <label class="fs-label" for="guests">Number of Guests</label>
    <input class="fs-input" type="text" id="guests" name="guests" placeholder="Approximate number of guests" required />
  </div>

  <div class="fs-field">
    <label class="fs-label" for="message">Message</label>
    <textarea class="fs-textarea" id="message" name="message" rows="10" placeholder="Tell us more about your event" required></textarea>
  </div>

  <input type="text" name="gotcha" style="display:none" />

  <div class="fs-button-group">
    <button class="fs-button" type="submit">Submit</button>
  </div>

</form>
