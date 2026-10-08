---
layout: default
title: Contact
description: "Contact Saurabh Singh by email or connect on LinkedIn and GitHub."
permalink: /contact/
---

<p class="section-kicker">03 / CONTACT</p>

# Let's talk<span class="accent">.</span>

<p class="lead">Have something in mind? I'd like to hear from you.</p>

<div class="contact-options">
  <div class="contact-option">
    <span class="contact-label">EMAIL</span>
    {% if site.email != empty and site.email %}
      <a href="mailto:{{ site.email | escape }}">{{ site.email | escape }} <span aria-hidden="true">↗</span></a>
      <p>This opens your email app.</p>
    {% else %}
      <p><strong>Placeholder — email address:</strong> Add your public email to <code>_config.yml</code> to display a mailto link here.</p>
    {% endif %}
  </div>
  <div class="contact-option">
    <span class="contact-label">LINKEDIN</span>
    <a href="{{ site.linkedin_url | escape }}" rel="me">Connect with Saurabh Singh <span aria-hidden="true">↗</span></a>
  </div>
  <div class="contact-option">
    <span class="contact-label">GITHUB</span>
    <a href="https://github.com/{{ site.github_username | escape }}" rel="me">github.com/{{ site.github_username | escape }} <span aria-hidden="true">↗</span></a>
  </div>
</div>