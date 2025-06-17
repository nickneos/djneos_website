---
permalink: /contact/
title: "Contact"
classes: wide
---

Use the below form to get in touch, or email [contact@djneos.com.au](mailto:contact@djneos.com.au)

For booking enquiries, please include venue, date and number of guests in your message if you have these details.

<form name="contact" method="POST" data-netlify="true" action="/thanks/" netlify-honeypot="gotcha">
    <input type="hidden" name="subject" value="[www.djneos.com.au] Contact Request (23%{submissionId})">
    <input type="text" name="name" placeholder="Your name" required>
    <input type="email" name="email" placeholder="Your email" required>
    <textarea name="message" rows="10" placeholder="Type your message" required></textarea>
    <input type="text" name="gotcha" style="display:none" />
    <button type="submit">Send</button>
</form>
