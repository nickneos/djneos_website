---
permalink: /contact2/
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

<form action="https://script.google.com/macros/s/AKfycbwu7JclvReE3PEfRIBMoCippp4fsRFjg7pHV-oiIs4-m3UJB9KGLKUOLLONGEZBLSQm/exec" method="POST" id="myform">
    <input type="text" name="name" placeholder="Your name" required>
    <input type="text" name="email" placeholder="Your email" required>
    <textarea name="message" rows="15" placeholder="Type your message" required></textarea>
    <button type="submit">Send</button>
<p id="result"></p>
</form>

<!-- Place this script at the end of the body tag -->
<script>
const form = document.getElementById("myform");
const result = document.getElementById("result");

form.addEventListener("submit", function (e) {
  e.preventDefault();
  
  const formData = new FormData(form);
  const object = Object.fromEntries(formData);
  const json = JSON.stringify(object);
  
  result.innerHTML = "Please wait...";

  fetch("https://script.google.com/macros/s/AKfycbwu7JclvReE3PEfRIBMoCippp4fsRFjg7pHV-oiIs4-m3UJB9KGLKUOLLONGEZBLSQm/exec", {
    method: "POST",
    headers: {
      "Content-Type": "application/json",
      "Accept": "application/json",
    },
    body: json,
  })
    .then(async (response) => {
      let json = await response.json();
      if (response.status == 200) {
        result.innerHTML = json.message;
        result.classList.remove("text-gray-500");
        result.classList.add("text-green-500");
      } else {
        console.log(response);
        result.innerHTML = json.message;
        result.classList.remove("text-gray-500");
        result.classList.add("text-red-500");
      }
    });
});
</script>

<!-- 
<form action="https://api.web3forms.com/submit" method="POST">
    <input type="hidden" name="access_key" value="d21069d0-5662-489a-b981-095235c8ae3e">
    <input type="hidden" name="subject" value="[djneos.com.au] Contact Request" />
    <input type="text" name="name" placeholder="Your name" required>
    <input type="email" name="email" placeholder="Your email" required>
    <textarea name="message" rows="15" placeholder="Type your message" required></textarea>
    <input type="checkbox" name="botcheck" class="hidden" style="display: none;">
    <input type="hidden" name="redirect" value="https://www.djneos.com.au/thanks/">
    <button type="submit">Send</button>
</form> 
-->

