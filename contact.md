---
title: Contact Me
layout: page
---

<form id="contact-form" action="https://formspree.io/f/xblyvwov" method="POST" style="max-width:520px;margin:2em auto 2em auto;padding:2.5em 2em 2em 2em;background:#202225;border-radius:1.2em;box-shadow:var(--shadow);display:flex;flex-direction:column;gap:1.2em;" autocomplete="on" novalidate>
  <h1 style="margin-top:0;text-align:center;">Contact Me</h1>
  <input type="hidden" name="_subject" value="New message from mattsPortfolio.com">
  <!-- Honeypot anti-spam field -->
  <div style="display:none;">
    <label>Leave this field blank: <input type="text" name="_gotcha" tabindex="-1" autocomplete="off"></label>
  </div>
  <label for="name" style="color:var(--accent2);font-weight:700;">Name</label>
  <input type="text" id="name" name="name" required minlength="2" maxlength="60" style="padding:0.7em 1em;border-radius:1em;border:1.5px solid var(--accent2);background:#23272a;color:#fff;font-size:1.1em;" aria-required="true" aria-label="Name">

  <label for="email" style="color:var(--accent2);font-weight:700;">Your Email</label>
  <input type="email" id="email" name="email" required pattern="^[^@\s]+@[^@\s]+\.[^@\s]+$" maxlength="100" style="padding:0.7em 1em;border-radius:1em;border:1.5px solid var(--accent2);background:#23272a;color:#fff;font-size:1.1em;" aria-required="true" aria-label="Your Email">

  <label for="message" style="color:var(--accent2);font-weight:700;">Message</label>
  <textarea id="message" name="message" rows="5" required minlength="10" maxlength="2000" style="padding:0.7em 1em;border-radius:1em;border:1.5px solid var(--accent2);background:#23272a;color:#fff;font-size:1.1em;" aria-required="true" aria-label="Message"></textarea>

  <button type="submit" style="background:var(--accent2);color:#fff;padding:0.9em 2em;border-radius:2em;font-weight:700;font-size:1.1em;box-shadow:0 2px 8px var(--accent2);border:none;cursor:pointer;transition:background 0.2s;">Send Message</button>
  <div id="form-error" style="display:none;color:#ff4c60;text-align:center;margin-top:0.5em;font-size:1em;font-weight:600;"></div>
</form>
<div id="form-success" style="display:none;color:var(--accent);text-align:center;margin-top:1.5em;font-size:1.1em;font-weight:700;">Thank you! Your message has been sent.</div>
<script>
document.addEventListener('DOMContentLoaded', function() {
  var form = document.getElementById('contact-form');
  var errorDiv = document.getElementById('form-error');
  var successDiv = document.getElementById('form-success');
  if(form) {
    form.addEventListener('submit', function(e) {
      e.preventDefault();
      errorDiv.style.display = 'none';
      // Client-side validation
      var name = form.name.value.trim();
      var email = form.email.value.trim();
      var message = form.message.value.trim();
      var gotcha = form._gotcha.value;
      if(gotcha) return; // Honeypot
      if(name.length < 2) {
        errorDiv.textContent = 'Please enter your name.';
        errorDiv.style.display = 'block';
        form.name.focus();
        return;
      }
      var emailPattern = /^[^@\s]+@[^@\s]+\.[^@\s]+$/;
      if(!emailPattern.test(email)) {
        errorDiv.textContent = 'Please enter a valid email address.';
        errorDiv.style.display = 'block';
        form.email.focus();
        return;
      }
      if(message.length < 10) {
        errorDiv.textContent = 'Please enter a message (at least 10 characters).';
        errorDiv.style.display = 'block';
        form.message.focus();
        return;
      }
      // Submit via AJAX
      var data = new FormData(form);
      fetch(form.action, {
        method: 'POST',
        body: data,
        headers: { 'Accept': 'application/json' }
      }).then(function(response) {
        if(response.ok) {
          form.style.display = 'none';
          successDiv.style.display = 'block';
        } else {
          response.json().then(function(data) {
            errorDiv.textContent = (data.errors && data.errors[0] && data.errors[0].message) || 'There was a problem submitting your form. Please try again.';
            errorDiv.style.display = 'block';
          }).catch(function() {
            errorDiv.textContent = 'There was a problem submitting your form. Please try again.';
            errorDiv.style.display = 'block';
          });
        }
      }).catch(function() {
        errorDiv.textContent = 'There was a problem submitting your form. Please try again.';
        errorDiv.style.display = 'block';
      });
    });
  }
});
</script> 