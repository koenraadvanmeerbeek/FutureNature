---
layout: page
title: Contact
permalink: /contact/
---
Feel free to reach out through the following channels:

<div class="contact-list">
  <div class="contact-item">
    <a href="#" onclick="window.location='mailto:' + ['koenraad.vanmeerbeek', 'kuleuven.be'].join('@')" class="contact-link">
      <span class="icon-envelop contact-icon"></span>
      <span class="contact-text">koenraad.vanmeerbeek[at]kuleuven.be</span>
    </a>
  </div>

  <div class="contact-item">
    <a href="https://bsky.app/profile/kvanmeerbeek.bsky.social" target="_blank" class="contact-link">
      <span class="icon-bluesky contact-icon"></span>
      <span class="contact-text">@kvanmeerbeek.bsky.social</span>
    </a>
  </div>

  <div class="contact-item">
    <a href="https://www.linkedin.com/in/koenraad-van-meerbeek-1b767b19/" target="_blank" class="contact-link">
      <span class="icon-linkedin2 contact-icon"></span>
      <span class="contact-text">LinkedIn Profile</span>
    </a>
  </div>

  <div class="contact-item">
    <a href="https://www.google.com/maps?q=Celestijnenlaan+200E,+3001+Leuven,+Belgium" target="_blank" class="contact-link">
      <span class="icon-location contact-icon"></span>
      <span class="contact-text">Celestijnenlaan 200E, 3001 Leuven, Belgium</span>
    </a>
  </div>
</div>

<style>
/* General container for the contact list */
.contact-list {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); /* Adjusts to 4, 2, or 1 column based on screen size */
  gap: 1rem; /* Space between items */
  justify-items: center; /* Centers items within the grid */
}

/* Individual contact item */
.contact-item {
  text-align: center; /* Center align icon and text */
}

/* Contact link to include both icon and text */
.contact-link {
  display: flex;
  flex-direction: column; /* Stack icon and text */
  align-items: center; /* Center content */
  text-decoration: none; /* Remove underline */
  color: inherit; /* Use inherited color */
  transition: transform 0.2s ease-in-out, color 0.2s ease-in-out; /* Add hover effect */
}

/* Icon styles */
.contact-icon {
  font-size: 40px; /* Size of the icon */
  margin-bottom: 0.5rem; /* Space between icon and text */
  color: #006871ff; /* Icon color */
  transition: transform 0.2s ease-in-out, color 0.2s ease-in-out; /* Hover effect */
}

/* Text styles */
.contact-text {
  font-size: 16px;
  color: #333; /* Default text color */
  transition: color 0.2s ease-in-out; /* Hover effect */
}

/* Hover effect */
.contact-link:hover .contact-icon {
  transform: scale(1.1); /* Slightly enlarge the icon */
  color: #007acc; /* Change color on hover */
}

.contact-link:hover .contact-text {
  color: #007acc; /* Change text color on hover */
}
</style>
