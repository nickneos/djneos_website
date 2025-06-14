---
permalink: /contact/
title: "Contact"
classes: wide
---

Use the below form to get in touch, or email [contact@djneos.com.au](mailto:contact@djneos.com.au)

For booking enquiries, please include venue, date and number of guests in your message if you have these details.

<!-- <form action="https://formspree.io/f/xwplvlzl" method="POST">
    <input type="hidden" name="subject" value="[djneos.com.au] Contact Request" />
    <input type="text" name="name" placeholder="Your name" required>
    <input type="email" name="email" placeholder="Your email" required>
    <textarea name="message" rows="15" placeholder="Type your message" required></textarea>
    <input type="text" name="_gotcha" style="display:none" />
    <button type="submit">Send</button>
</form> -->

<form id="form1" action="https://api.web3forms.com/submit" method="POST">
    <input type="hidden" name="access_key" value="d21069d0-5662-489a-b981-095235c8ae3e">
    <input type="hidden" name="subject" value="[djneos.com.au] Contact Request" />
    <!-- Form Inputs. Each input must have a name="" attribute -->
    <input type="text" name="name" placeholder="Your name" required>
    <input type="email" name="email" placeholder="Your email" required>
    <textarea name="message" rows="15" placeholder="Type your message" required></textarea>
    <!-- Honeypot Spam Protection -->
    <input type="checkbox" name="botcheck" class="hidden" style="display: none;">
    <!-- Custom Confirmation / Success Page -->
    <input type="hidden" name="redirect" value="https://www.djneos.com.au/thanks/">
    <div class="h-captcha" data-captcha="true"></div>
    <button type="submit">Send</button>
</form>


<script src="https://web3forms.com/client/script.js" async defer></script>

<script>
const form = document.getElementById('form1');

form.addEventListener('submit', function(e) {

    const hCaptcha = form.querySelector('textarea[name=h-captcha-response]').value;

    if (!hCaptcha) {
        e.preventDefault();
        alert("Please fill out captcha field")
        return
    }
});
</script>